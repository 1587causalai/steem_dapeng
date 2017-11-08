---
title: "Steemit 的新手们，你们考虑过数据隐私的问题吗"
author: dapeng
date: "2017-07-26 20:14:06"
slug: steemit
categories: [cn]
tags: 
  - cn
---

原文链接: [steemit](https://steemit.com/cn/@dapeng/steemit), [cnsteem](https://cnsteem.com/cn/@dapeng/steemit), [chainbb](https://chainbb.com/cn/@dapeng/steemit), [busy](https://busy.org/cn/@dapeng/steemit), [markdown](https://raw.githubusercontent.com/pzhaonet/steem_mirror/master/content/post/steemit.md)

不知大家来 Steemit 有没有意识到个人隐私问题。要知道，我们的一举一动，都是记录在案的，而这些数据是对所有人开放的。那么，别人到底能看见你的哪些信息呢？


下面，我们用 @tumutanzi 的公开数据(<https://steemdb.com/>, 采集时间 2017-07-26 22:06:46 CEST)，进行一点粗浅的展示，所用的工具是 R 语言。本文是第1部分。数据处理得比较仓促，连分析都算不上，如有错误，抱歉得很，请先原谅我，然后指正。


@tumutanzi 的粉丝有 319个ID，按照受欢迎程度（即他们各自被多少ID关注）排序的词云是这样的：


![unnamed-chunk-2-1.png](https://steemitimages.com/DQmY4qfoEu9XZzpYjg6aR52bVMpPvcfMXej56AKvmu46j1E/unnamed-chunk-2-1.png)



凡是看得清的，基本我都不认识。 @abit 大神在这里并不起眼。


按照发帖数排序是这样的：


![unnamed-chunk-3-1.png](https://steemitimages.com/DQmSBtokTVueC2qxCnBqxn7vU24HaiJzhCgFqSUQ257fFLG/unnamed-chunk-3-1.png)


@abit 和 @oflyhigh 两位大神似乎也并不显山露水。


按Vest（是什么？富有程度？）排序是这样的：


![unnamed-chunk-4-1.png](https://steemitimages.com/DQmcrddtPW9tH3HaFjAcEiMc9qFiwRt5ePe4AHGEfMxUBWc/unnamed-chunk-4-1.png)


吓死人了。 @abit，拥有 4077000000 Vests，鹤立鸡群，弄得别的ID都区分不出来了。这叫闷声发大财么？


我们把他踢出去再看看：



![unnamed-chunk-5-1.png](https://steemitimages.com/DQmTfss2wX94T9NjpQ74u4pXVd1E1gdT7tsvTZ6VMAt8cGS/unnamed-chunk-5-1.png)


@oflyhigh 和 @xiaohui 现身了。


另一方面，我们看看 @tumutanzi 都关注了谁。


@tumutanzi 关注的ID总数是 305（包含后来他取消关注的）。其中，有152个 ID 跟 @tumutanzi 是双向关注的，而153个ID 虽然被他关注，但却没有关注他。奈何明月照沟渠。可怜的 @tumutanzi，这些不搭理他的 ID 是：



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


反过来，关注了他却未被他关注的有：


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



奇怪， @abit 和 @justyy 明明在 @tumutanzi Steemit 的 following 名单里，但是在 [steemdb 里却没有](https://steemdb.com/@tumutanzi/following).


不管怎么样，坛子，在他们读到本帖之间，快去关注他们吧，免得被追杀……


如果你想要一份关于你自己 ID 的 follower 和 following 的类似报告，请访问我制作的[在线工具 steemr](https://pzhao.shinyapps.io/steemr/)。



*未完，待续......*
