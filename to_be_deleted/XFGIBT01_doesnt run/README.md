[<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/banner.png" width="888" alt="Visit QuantNet">](http://quantlet.de/)

## [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/qloqo.png" alt="Visit QuantNet">](http://quantlet.de/) **XFGIBT01** [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/QN2.png" width="60" alt="Visit QuantNet 2.0">](http://quantlet.de/)

```yaml


Name of Quantlet: XFGIBT01 

Published in: Applied Quantitative Finance

Description: 'XFGIBT01 Outputs implied binomial trees computed by DK and BC algorithm of stock prices, transition probabilities and Arrow-Debreu prices, respectively, with a parabolic implied volatility (see IBTimpliedvola). Require IBTblackscholes.m, IBTdk.m, IBTbc.m, IBTimpliedvola.m, IBTresort.m, IBTcrr.m'

Keywords: implied, binomial tree, blackscholes, options

See also: IBTbc, IBTblackscholes, IBTcrr, IBTdk, IBTimpliedvola, IBTresort, XFGLSK, XFGSPDcb2, XFGSPDcom

Author: Jun Zheng, Alena Mysickova

Submitted: 2012-07-27 by Dedy Dwi Prastyo

Datafiles: XFGIBT01.asv

Example: 'Run the program with following values for Price of underlying asset, Interest rate, Time to expiration and Number of steps, respectively: [100, 0.03, 3, 3]'

```

### MATLAB Code
```matlab

%% CODE

disp('Please input Price of Underlying Asset s0, Riskless Interest Rate per Year r');
disp('Time to Expiration (Years) t, Number of steps n');
disp('as: [100, 0.03, 5, 5]');
disp(' ') ;
para=input('[s0, r, t, n]=');
while length(para) < 4
  disp('Not enough input arguments. Please input in 1*4 vector form like [100, 0.03, 5, 5]');
  disp(' ') ;
  para=input('[s0, r, t, n]=');
end

s0=para(1);                             % Stock price
r=para(2);                              % Riskless interest rate   
t=para(3);                              % Time to expiration
n=para(4);                              % Number of intervals format short
[St, AD, P, LV] = IBTdk(s0,r,t,n,[]);      % DK algorithm with parabolic implied volatility
[St2, AD2, P2, LV2] = IBTbc(s0,r,t,n,[]);  % BC algorithm with parabolic implied volatility

%% Resorting

resort the matrices    
Stree = IBTresort(St);                  
ADtree = IBTresort(AD);
Ptree = IBTresort(P);
Stree2 = IBTresort(St2);
ADtree2 = IBTresort(AD2);
Ptree2 = IBTresort(P2);
'implied stock tree D&K'
disp(Stree);
'implied stock tree B&C'
disp(Stree2);
'transition probability tree D&K'
disp(Ptree);
'transition probability tree B&C'
disp(Ptree2);
'arrow debreu price tree D&K'
disp(ADtree);
'arrow debreu price tree B&C'
disp(ADtree2);
```

automatically created on 2018-05-28