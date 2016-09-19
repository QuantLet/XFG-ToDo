# yamldebugger - test package

### Qualifying of the given Qs


# History of Qs in this Repo validated by 'yamldebugger' (Version 0.5.0) :

## [XFG-ToDo](https://github.com/QuantLet/XFG-ToDo) : 12.09.2016
```r
> qnames = yaml.debugger.get.qnames(d_init$RootPath)
[1] "12 Q folder(s) found:"
 [1] "StandardNormalCharf" "XFGcofi"             "XFGdist"             "XFGexc"              "XFGRsquared"         "XFGSPDcb"           
 [7] "XFGSPDcom"           "XFGSPDoneday"        "XFGSPDonemonth"      "XFGSummary2"         "XFGVaRcharfDGtest"   "XFGVaRestMC"        
> d_results = yaml.debugger.run(qnames, d_init)
[1] "1: StandardNormalCharf"
[1] "--------------------------------------------------------------------"
[1] "2: XFGcofi"
[1] "--------------------------------------------------------------------"
[1] "3: XFGdist"
[1] "--------------------------------------------------------------------"
[1] "4: XFGexc"
[1] "--------------------------------------------------------------------"
[1] "5: XFGRsquared"
[1] "--------------------------------------------------------------------"
[1] "6: XFGSPDcb"
[1] "--------------------------------------------------------------------"
[1] "7: XFGSPDcom"
[1] "--------------------------------------------------------------------"
[1] "8: XFGSPDoneday"
[1] "--------------------------------------------------------------------"
[1] "9: XFGSPDonemonth"
[1] "--------------------------------------------------------------------"
[1] "10: XFGSummary2"
[1] "--------------------------------------------------------------------"
[1] "11: XFGVaRcharfDGtest"
[1] "--------------------------------------------------------------------"
[1] "12: XFGVaRestMC"
[1] "--------------------------------------------------------------------"
> OverView = yaml.debugger.summary(qnames, d_results, summaryType = "mini")
> OverView
      Q Names               Missing Style Guide fields Descriptions stats             Keywords stats               
 [1,] "StandardNormalCharf" ""                         "12 word(s), 83 Character(s)"  "NA: 3 (standard), NA (new)" 
 [2,] "XFGcofi"             "Author"                   "11 word(s), 73 Character(s)"  "NA: 2 (standard), NA (new)" 
 [3,] "XFGdist"             "Keywords"                 "5 word(s), 34 Character(s)"   "NA: NA (standard), NA (new)"
 [4,] "XFGexc"              "Keywords"                 "7 word(s), 42 Character(s)"   "NA: NA (standard), NA (new)"
 [5,] "XFGRsquared"         ""                         "56 word(s), 282 Character(s)" "NA: 10 (standard), NA (new)"
 [6,] "XFGSPDcb"            ""                         "61 word(s), 328 Character(s)" "NA: 13 (standard), NA (new)"
 [7,] "XFGSPDcom"           ""                         "23 word(s), 117 Character(s)" "NA: 17 (standard), NA (new)"
 [8,] "XFGSPDoneday"        ""                         "94 word(s), 518 Character(s)" "NA: 14 (standard), NA (new)"
 [9,] "XFGSPDonemonth"      ""                         "72 word(s), 369 Character(s)" "NA: 14 (standard), NA (new)"
[10,] "XFGSummary2"         "Author"                   "51 word(s), 245 Character(s)" "NA: 8 (standard), NA (new)" 
[11,] "XFGVaRcharfDGtest"   ""                         "30 word(s), 142 Character(s)" "NA: 2 (standard), NA (new)" 
[12,] "XFGVaRestMC"         ""                         "33 word(s), 189 Character(s)" "NA: 2 (standard), NA (new)"
```


## [XFG-ToDo](https://github.com/QuantLet/XFG-ToDo) : 16.09.2016
```r
> qnames = yaml.debugger.get.qnames(d_init$RootPath)
[1] "13 Q folder(s) found:"
 [1] "XFGELESC"             "XFGexp_rtn_ES_2d"     "XFGIndustryBreakdown" "XFGqDGtest"           "XFGRegionsBreakdown"  "XFGriskaversion"     
 [7] "XFGriskaversion2"     "XFGRsquared"          "XFGSPDcb"             "XFGSPDcom"            "XFGSPDoneday"         "XFGSPDonemonth"      
[13] "XFGSummary2"         
> 
> d_results = yaml.debugger.run(qnames, d_init)
[1] "1: XFGELESC"
[1] "--------------------------------------------------------------------"
[1] "2: XFGexp_rtn_ES_2d"
[1] "--------------------------------------------------------------------"
[1] "3: XFGIndustryBreakdown"
[1] "--------------------------------------------------------------------"
[1] "4: XFGqDGtest"
[1] "--------------------------------------------------------------------"
[1] "5: XFGRegionsBreakdown"
[1] "--------------------------------------------------------------------"
[1] "6: XFGriskaversion"
[1] "--------------------------------------------------------------------"
[1] "7: XFGriskaversion2"
[1] "--------------------------------------------------------------------"
[1] "8: XFGRsquared"
[1] "--------------------------------------------------------------------"
[1] "9: XFGSPDcb"
[1] "--------------------------------------------------------------------"
[1] "10: XFGSPDcom"
[1] "--------------------------------------------------------------------"
[1] "11: XFGSPDoneday"
[1] "--------------------------------------------------------------------"
[1] "12: XFGSPDonemonth"
[1] "--------------------------------------------------------------------"
[1] "13: XFGSummary2"
[1] "--------------------------------------------------------------------"
> 
> OverView = yaml.debugger.summary(qnames, d_results, summaryType = "mini")
> OverView
      Q Names                Missing Style Guide fields Descriptions stats             Keywords stats               
 [1,] "XFGELESC"             ""                         "13 word(s), 81 Character(s)"  "NA: 12 (standard), NA (new)"
 [2,] "XFGexp_rtn_ES_2d"     ""                         "20 word(s), 111 Character(s)" "NA: 6 (standard), NA (new)" 
 [3,] "XFGIndustryBreakdown" ""                         "25 word(s), 131 Character(s)" "NA: 6 (standard), NA (new)" 
 [4,] "XFGqDGtest"           ""                         "3 word(s), 19 Character(s)"   "NA: 8 (standard), NA (new)" 
 [5,] "XFGRegionsBreakdown"  ""                         "25 word(s), 129 Character(s)" "NA: 6 (standard), NA (new)" 
 [6,] "XFGriskaversion"      ""                         "31 word(s), 180 Character(s)" "NA: 6 (standard), NA (new)" 
 [7,] "XFGriskaversion2"     ""                         "13 word(s), 62 Character(s)"  "NA: 6 (standard), NA (new)" 
 [8,] "XFGRsquared"          ""                         "56 word(s), 282 Character(s)" "NA: 10 (standard), NA (new)"
 [9,] "XFGSPDcb"             ""                         "61 word(s), 328 Character(s)" "NA: 13 (standard), NA (new)"
[10,] "XFGSPDcom"            ""                         "23 word(s), 117 Character(s)" "NA: 17 (standard), NA (new)"
[11,] "XFGSPDoneday"         ""                         "94 word(s), 518 Character(s)" "NA: 14 (standard), NA (new)"
[12,] "XFGSPDonemonth"       ""                         "72 word(s), 369 Character(s)" "NA: 14 (standard), NA (new)"
[13,] "XFGSummary2"          ""                         "51 word(s), 245 Character(s)" "NA: 8 (standard), NA (new)"

```

to be continued...
