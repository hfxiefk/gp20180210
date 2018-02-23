http://www.55188.com/viewthread.php?tid=6127812&page=1&extra=page%3D1#pid127307242

佩服你的执着  把下面源码加到主图源码最后

REF(H,BARSLAST(CURRBARSCOUNT=CONST(BARSLAST(XG=1))+1));

回复 46楼 @冷妞妞 的帖子
@冷妞妞 老师你好，周末快乐！请你把一根大阳线或者中阳线突破前期高点时做一个选股！
具体条件描述：
1.前期高点必须是一根光头阴k线。
2.出现高点后必须有一个连续的下跌走势。
3.某日突破该高点时做选股！


主图画线图标
YY:=IF(C<O,H,-999);
HH:=HHVBARS(YY,60);
A:DRAWLINE(HH=0 AND O=H,O,REF(HH=0 AND O=H,1),REF(O,1),1),COLORYELLOW,LINETHICK2;
TJ:=C>A AND O<A;
XG:=COUNT(TJ,HH+1)=1 AND TJ;
DRAWICON(XG AND HH>5,L*0.98,1);
选股
YY:=IF(C<O,H,-999);
HH:=HHVBARS(YY,60);
A:=DRAWLINE(HH=0 AND O=H,O,REF(HH=0 AND O=H,1),REF(O,1),1);
TJ:=C>A AND O<A;
XG:=COUNT(TJ,HH+1)=1 AND TJ;
XG AND HH>5;

大师可以帮忙写一个分时主图吗
5分钟ＭＡＣＤ底背买1　　5分钟ＫＤＪ的Ｊ值-10以下　买2
5分钟ＭＡＣＤ顶背卖1　　5分钟ＫＤＪ的Ｊ值110以上　卖2
5日线　10线　30线画线

DRAWTEXT_FIX(ISLASTBAR ,0.20,0.01,1,DYBLOCK),COLORYELLOW;
DRAWTEXT_FIX(ISLASTBAR ,0.30,0.01,1,HYBLOCK),COLORYELLOW;
DRAWTEXT_FIX(ISLASTBAR ,0.50,0.10,1,GNBLOCK),COLORWHITE;
这是个行业板块指标   妞妞老是能不能帮我把这个规整下     在最上方一字显示    免得看上去太乱