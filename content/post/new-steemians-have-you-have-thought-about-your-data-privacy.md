---
title: "New Steemians, have you ever thought about your data privacy?"
author: dapeng
date: "2017-07-26 20:56:21"
slug: new-steemians-have-you-have-thought-about-your-data-privacy
categories: [steemit]
tags: 
  - steemit
  - steem
  - r-language
  - introduceyourself
---

原文链接: [steemit](https://steemit.com/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy), [cnsteem](https://cnsteem.com/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy), [chainbb](https://chainbb.com/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy), [busy](https://busy.org/steemit/@dapeng/new-steemians-have-you-have-thought-about-your-data-privacy), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/new-steemians-have-you-have-thought-about-your-data-privacy.md)

If  you are a new Steemian, I was wondering if you are aware of your data privacy. If not, you'd better know it in advance. Here I display @tumutanzi's public data (<https://steemdb.com/>,  sampled at  2017-07-26 22:06:46 CEST) in an easy way with R language. This is Part I. This is an English version of the [original post in Chinese](https://steemit.com/cn/@dapeng/steemit).



@tumutanzi has 319 followers. The word cloud according to the number of their followers is like this:


![unnamed-chunk-2-1.png](https://steemitimages.com/DQmY4qfoEu9XZzpYjg6aR52bVMpPvcfMXej56AKvmu46j1E/unnamed-chunk-2-1.png)


A larger ID means more followers.


It can be plotted by the number of posts as well:


![unnamed-chunk-3-1.png](https://steemitimages.com/DQmSBtokTVueC2qxCnBqxn7vU24HaiJzhCgFqSUQ257fFLG/unnamed-chunk-3-1.png)


or by the number of Vests:


![unnamed-chunk-4-1.png](https://steemitimages.com/DQmcrddtPW9tH3HaFjAcEiMc9qFiwRt5ePe4AHGEfMxUBWc/unnamed-chunk-4-1.png)


@abit is scary, who has 4077000000 Vests. Let's kick him out:



![unnamed-chunk-5-1.png](https://steemitimages.com/DQmTfss2wX94T9NjpQ74u4pXVd1E1gdT7tsvTZ6VMAt8cGS/unnamed-chunk-5-1.png)



Now let's see those whom @tumutanzi is following.


@tumutanzi follows/followed 305 ID in total, in which 152 IDs interact with @tumutanzi bidirectionally, while 153 IDs do not follow him, including:



    ##   [1] "ace108"          "act"             "adm"            

    ##   [4] "adoal"           "adsactly"        "alice"          

    ##   [7] "anwenbaumeister" "arcurus"         "arhag"          

    ##  [10] "azazqwe"         "batel"           "ben"            

    ##  [13] "birds90"         "bitcube"         "blocktrades"    

    ##  [16] "blueorgy"        "bob"             "brothermic"     

    ##  [19] "btsabc"          "bziing"          "candiceji"      

    ##  [22] "ceciliali"       "chinadaily"      "cnfund"         

    ##  [25] "coldhair"        "cornelia"        "cqf"            

    ##  [28] "created"         "cybercodetwins"  "damarth"        

    ##  [31] "dan"             "dantheman"       "databass"       

    ##  [34] "davidyuan"       "deadlinefarmer"  "dek"            

    ##  [37] "dixonloveart"    "dmilash"         "ekitcho"        

    ##  [40] "elfkitchen"      "engagement"      "everittdmickey" 

    ##  [43] "feelapi"         "flysaga"         "freedom"        

    ##  [46] "frostfan"        "fuzzyvest"       "fyrstikken"     

    ##  [49] "gaoduzhu"        "gavvet"          "gefa"           

    ##  [52] "glitterfart"     "goku1"           "guyverckw"      

    ##  [55] "haster"          "hendrikdegrote"  "hingman"        

    ##  [58] "holabebe"        "huaji"           "icedream"       

    ##  [61] "incrediblesnow"  "ivanba12"        "j-bex"          

    ##  [64] "jademont"        "jaewoocho"       "jamesc"         

    ##  [67] "jamesc1"         "jasonmcz"        "jeicko19"       

    ##  [70] "jholdsworthy"    "jinbo"           "kawaiiiiiiii030"

    ##  [73] "kenchung"        "kitcat"          "krischy"        

    ##  [76] "laodr"           "laoyao"          "lcb"            

    ##  [79] "lief"            "linuslee0216"    "logic"          

    ##  [82] "lukestokes"      "matrix"          "miacats"        

    ##  [85] "michael-a"       "michael-b"       "microluck"      

    ##  [88] "minfon"          "minority-report" "monkimo"        

    ##  [91] "morten"          "mottler"         "ned"            

    ##  [94] "nextgen622"      "nicolemoker"     "nuagnorab"      

    ##  [97] "orientaledu"     "papa-pepper"     "penguinpablo"   

    ## [100] "peterpan"        "pfunk"           "pharesim"       

    ## [103] "pilgrimtraveler" "pipertomcat"     "pistox"         

    ## [106] "pkhope"          "project11"       "proskynneo"     

    ## [109] "publicworker"    "puffin"          "ranchorelaxo"   

    ## [112] "rawnetics"       "rayphu"          "rea"            

    ## [115] "recursive"       "renohq"          "riverhead"      

    ## [118] "roadscape"       "robrigo"         "rok-sivante"    

    ## [121] "rook"            "safari"          "scorpion"       

    ## [124] "sean1980"        "smooth"          "someone"        

    ## [127] "stan"            "steem"           "steemed"        

    ## [130] "steemit"         "steemitblog"     "stellabelle"    

    ## [133] "str11ngfello"    "sunnyray"        "susanlo"        

    ## [136] "tamim"           "teamsteem"       "thecryptofiend" 

    ## [139] "thejohalfiles"   "trafalgar"       "transisto"      

    ## [142] "val-a"           "val-b"           "wackou"         

    ## [145] "wanbin"          "waterflier"      "webclerk"       

    ## [148] "witness.svk"     "wjm"             "wjs2634"        

    ## [151] "wongshiying"     "xeldal"          "zoef"


On the other hand, those who follow him but he does not follow (yet) are:


    ##   [1] "abit"            "abusalam"        "acrich"         

    ##   [4] "adraaz"          "alexieong"       "alfredchen"     

    ##   [7] "aniksh"          "artsyppl"        "asskick"        

    ##  [10] "aster"           "atc"             "atrix"          

    ##  [13] "avilsd"          "avinger"         "babasikandar"   

    ##  [16] "baixu1018"       "bajeheart"       "bassemm"        

    ##  [19] "bbkivines"       "beautifulbella"  "benou"          

    ##  [22] "berke"           "biddle"          "bilalhaider"    

    ##  [25] "bindu"           "bocaiwen"        "brianchen"      

    ##  [28] "britt.the.ish"   "carinewhy"       "carolynseymour" 

    ##  [31] "catwomanteresa"  "chumhumnews"     "cryptochamo"    

    ##  [34] "danishali"       "danm2017"        "davidad"        

    ##  [37] "daxiblog"        "dcc"             "deanliu"        

    ##  [40] "diablocro"       "diaohuijun"      "dimidrolshina"  

    ##  [43] "dinsha"          "dobro88888888"   "dominicmi"      

    ##  [46] "dragos0897"      "dtworker"        "fitinfun"       

    ##  [49] "frankbuse"       "gamemusic"       "gatmi"          

    ##  [52] "goaln"           "gowldie"         "gribtertong"    

    ##  [55] "grildrig"        "hamzaoui"        "harttwohartllc" 

    ##  [58] "hebro"           "hilarski"        "hofffman"       

    ##  [61] "hongmeng"        "hoof"            "hqfzone"        

    ##  [64] "imagediet"       "imako"           "initnas"        

    ##  [67] "investlimestone" "iqbalbireuen"    "irphotography"  

    ##  [70] "ishaq"           "istox"           "iszarl"         

    ##  [73] "itan05"          "itissimple"      "jackmiller"     

    ##  [76] "jamal83"         "jason-donovan"   "jhonnight"      

    ##  [79] "jones420"        "joseburgos"      "jukas"          

    ##  [82] "junyi"           "justyy"          "kabindra"       

    ##  [85] "katythompson"    "khairulmuammar"  "kishore1988"    

    ##  [88] "krasotka"        "kristjannacaj"   "landeberg"      

    ##  [91] "lautenglye"      "ledygaga25"      "lemooljiang"    

    ##  [94] "liangfengyouren" "lifeofkly"       "lifishake"      

    ##  [97] "lilywang"        "liufeng"         "luckerme"       

    ## [100] "lykencrypto"     "lynx"            "marianpancu"    

    ## [103] "mehdioraki3973"  "minknsa"         "mkotibabu"      

    ## [106] "monalishabiswas" "mydarlings2"     "myfirst"        

    ## [109] "mytamilabiz"     "natashahall"     "nationalpark"   

    ## [112] "nawar93"         "newsagg"         "notregme"       

    ## [115] "oflyhigh"        "ohammedfelahi"   "patricksanlin"  

    ## [118] "phyohtetpaing"   "powerfj"         "qipashuo"       

    ## [121] "redje"           "renua"           "revolusi"       

    ## [124] "riansteem"       "rifattb"         "robi8888"       

    ## [127] "rodneyaspiras"   "rogerwilson"     "sbamsoneu"      

    ## [130] "secora"          "securetalk"      "sequentialvibe" 

    ## [133] "shaheer001"      "shankhunsam"     "shengjian"      

    ## [136] "sheval"          "showoff"         "skynyc"         

    ## [139] "somebody"        "stackin"         "steem.engine"   

    ## [142] "steemitguide"    "sthitaprajna"    "suitup"         

    ## [145] "sunnyjolly"      "superhardness"   "swssmarketing"  

    ## [148] "tastetwist"      "themessengers"   "toninux"        

    ## [151] "trevis"          "vax-rambo"       "vishal1088"     

    ## [154] "walkman90"       "warrkin"         "whydowork"      

    ## [157] "worldwidetravel" "xiaohui"         "xiaokongcom"    

    ## [160] "xjb"             "yellowkersie"    "ygern"          

    ## [163] "yuxi"            "zerozero777"     "zhijun"         

    ## [166] "zhuqiankun"      "zwal"



It is weird that  @abit and @justyy are in   @tumutanzi Steemit's following list, but not in the list of  [steemdb](https://steemdb.com/@tumutanzi/following).


Anyway, I would suggest @tumutanzi should follow them before they read this post. Hurry!


If you would like to have a similar report about your ID's followers and following, please  visit the online tool [steemr](https://pzhao.shinyapps.io/steemr/).


*To be continued......*
