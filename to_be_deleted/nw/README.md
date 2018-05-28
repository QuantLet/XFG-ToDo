[<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/banner.png" width="888" alt="Visit QuantNet">](http://quantlet.de/)

## [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/qloqo.png" alt="Visit QuantNet">](http://quantlet.de/) **nw** [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/QN2.png" width="60" alt="Visit QuantNet 2.0">](http://quantlet.de/)

```yaml

Name of QuantLet: nw

Published in: Applied Quantitative Finance

Description: nw computes the Nadaraya-Watson Estimator

Keywords: Nadaraya Watson, nonparametric, estimation, kernel, univariate

Author: Awdesch Melzer

See also: XFGIBT03

Submitted: Thu, January 17 2013 by Awdesch Melzer
```

### MATLAB Code
```matlab

function sker=nw(x, vecX, vecY, h, K)   %Nadaraya-Watson Estimator
    vx   = size(x);
    vY   = size(vecY);
    vX   = size(vecX);
    vh   = size((vecX-x)/h');

    sker = 1/h*kernel((vecX-x)./h,K)'*vecY;
```

automatically created on 2018-05-28