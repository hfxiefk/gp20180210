http://www.55188.com/viewthread.php?tid=4223776&extra=&highlight=&page=39
通达信自带就有，副图的话http://www.55188.com/thread-3890410-1-4.html，在二楼
大智慧副图的在http://www.55188.com/thread-4233927-1-1.html



http://www.55188.com/thread-4269250-1-1.html

http://www.55188.com/viewthread.php?tid=4268705&extra=&highlight=&page=8

附上薛丝突破上轨选股指标，可以用来预警，突破薛丝上轨的股票预警后，开始关注能否封涨停板突破买入。
我只有大智慧版本的指标。
突破薛丝：VAR2:=CLOSE*VOL;
VAR3:=EMA((EMA(VAR2,3)/EMA(VOL,3)+EMA(VAR2,6)/EMA(VOL,6)+EMA(VAR2,12)/EMA(VOL,12)+EMA(VAR2,24)/EMA(VOL,24))/4,13);
SUP:=1.06*VAR3;
SDN:=VAR3*0.94;
VAR4:=EMA(CLOSE,9);
LUP:=EMA(VAR4*1.14,5);
薛斯选股:CROSS(CLOSE,LUP );


其实大智慧和通达信公式大部分都是通用的：
VAR2:=CLOSE*VOL;
VAR3:=EMA((EMA(VAR2,3)/EMA(VOL,3)+EMA(VAR2,6)/EMA(VOL,6)+EMA(VAR2,12)/EMA(VOL,12)+EMA(VAR2,24)/EMA(VOL,24))/4,13);
SUP:=1.06*VAR3;
SDN:=VAR3*0.94;
VAR4:=EMA(CLOSE,9);
LUP:=EMA(VAR4*1.14,5);
薛斯选股:CROSS(CLOSE,LUP );