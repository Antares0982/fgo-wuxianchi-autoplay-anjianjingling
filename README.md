# fgo无限池按键精灵脚本
fgo无限池按键精灵全自动爆肝脚本（能力较差，只能做到这个程度请大佬体谅）。

仅限安卓Mumu模拟器，其他模拟器如果有需要请自行修改代码段。

正赛之后的脚本要等开始之后再写。大概到时候会是狂兰绿卡队配置。

如果是第一次使用按键精灵，请按照下面步骤做一次：

1. 右键，点击兼容性疑难解答
2. 点击疑难解答程序
3. 点击 程序已打开，但未正确显示
4. 点击 当选择较大的字体设置时程序无法正确显示
5. 点击测试程序，然后关闭按键精灵
6. 在兼容性疑难解答中点击 是，为此程序保留这些设置

### 全局注意事项

* 只吃铜苹果。可以在最后位置改掉
* 防止使用到没打技能本的助战，脚本只会选取好友的助战

### 更新日记

**10月6日** 

加入了助战选择的新逻辑，主要体现在可以判断第二位助战是谁、选择第二位助战以及缩短刷新列表的时间（孔明挂的人太少了，难受）。加入了一个自动解决结算界面死循环的模块，可能没什么用还会导致更多bug。

**10月7日**

在昨天的自动解决结算界面死循环的位置，加入了自动排错机制。如果在某一步触发了自动排错，那么必然此时游戏逻辑已经走到助战选择位置。将助战30次刷新不到判断为需要排错。排错机制完成之后将会回到脚本最最开始的界面。

**12月4日**

新增了满羁绊时获得羁绊礼装的退出判断，减少了刷新助战的等待时间

## 圣诞枪本

目前可以使用的配置（站位顺序从左到右）（会持续更新）：

* 小达芬奇（不满破宝石翁，三宝，100级，10-1-10）+花嫁尼禄（90级，10-10-1+强化本）+玉藻前（90级10-1-10+强化本）+助战孔明（23技能10）+换人服
* 狂兰（满破加成礼装，三宝，80级，1-10-10）+CBA（90级，10-10-10）+助战CBA（同前）+孔明（90级，23技能10）+换人服

## 自动刷冰

在五个急救箱挑战的关卡刷永远结冰，没有材料掉落时第三回合自动退出战斗。

* 小达芬奇（不满破宝石翁，三宝，100级，10-1-10）+花嫁尼禄（90级，10-10-1+强化本）+玉藻前（90级10-1-10+强化本）+助战孔明（23技能10）+换人服

### 注意事项

* 不同电脑像素格位置不一样

* 这次的脚本已经修改了上一代的毛病，对自己的设备，前面的参数全部都得自己用抓抓来选择，不只是像素点颜色，像素点位置也要根据自己的设备自己抓！


* firstappleY和firstappleY2也是非常重要的需要自改的部分！这两个参数要保证在体力>=40的时候，不会点击到好友的助战。
* pyframeYdiff是两个助战框的Y轴距离。要注意，每个助战框的绿色好友标志对应位置颜色*居然*不是一样的。

