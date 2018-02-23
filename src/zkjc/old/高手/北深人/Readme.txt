http://www.55188.com/viewthread.php?tid=4539470&page=1&authorid=1274227
http://www.55188.com/viewthread.php?tid=4446825&extra=&page=8

有感于老师的为人，献上自己胡乱做的小指标，还望大家和老师指点、不要笑话哦。用这个指标来发现主力逆市吸筹还是有点用滴。源码如下：
Var1:=(c-ref(c,1))/ref(c,1)*100;
Var2:=(INDEXC-REF(INDEXC,1))/REF(INDEXC,1)*100;
个股强弱:Var1,coloryellow,LINETHICK0 ;
大盘强弱:Var2,colorgreen,LINETHICK0 ;
强弱:个股强弱-大盘强弱,coloryellow,LINETHICK0;
强弱2:=Var2<=-1.5 and Var1>=-1 and Var1<=5.5 ;
STICKLINE(大盘强弱<=-1,0,大盘强弱,8.10,0),colorgreen;
STICKLINE(强弱2,0,强弱,8.10,0),COLOR0000CC;
量比:V/(REF(MA(V,5),1)),LINETHICK0,colorgreen;
0,colorwhite;


http://www.55188.com/blog.php?tid=4655336

