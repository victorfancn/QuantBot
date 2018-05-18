# QuantBot

最近研究量化交易，学习了很好的一个项目：[Samaritan](https://github.com/miaolz123/samaritan)

可惜这个项目已经很久很久没有更新過了，另外项目中也有一些BUG，其中最致命的BUG就是在实现javascript并发任务这个功能的时候没有考虑资源冲突的处理，导致程序无法正常工作，所以对这些部分进行了一些修改，使其可以正常工作，并且更新了文档，另外原有的一些交易所接口也因为各种原因失效了，所以这里也重新更新了部分交易所接口，并且更新了文档，然后给项目重新改了个更直观的名字。

最后感谢原作者开发了这么好的项目让大家学习，再次附上原项目地址：https://github.com/miaolz123/samaritan

[更新的文档](http://www.quartbot.org/#/)

## 编译

直接运行build.sh进行编译，需要用到xgo和Docker，可以同时编译出多个平台下的可执行文件，如果不需要多平台支持，可以直接用go编译，推荐使用LiteIDE。

## 支持的交易所

| 交易所 | 货币类型 |
| -------- | ----- |
| okex | `BTC/USDT`, `ETH/USDT`, `EOS/USDT`, `ONT/USDT`, `QTUM/USDT`, `ONT/ETH` |
| 火币网 | `BTC/USDT`, `ETH/USDT`, `EOS/USDT`, `ONT/USDT`, `QTUM/USDT` |
| 比特儿国际 | `BTC/USDT`, `ETH/USDT`, `EOS/USDT`, `ONT/USDT`, `QTUM/USDT` |
| 币安 | `BTC/USDT`, `ETH/USDT`, `EOS/USDT`, `ONT/USDT`, `QTUM/USDT` |
| poloniex | `ETH/BTC`, `XMR/BTC`, `BTC/USDT`, `LTC/BTC`, `ETC/BTC`, `XRP/BTC`, `ETH/USDT`, `ETC/ETH`, ... |
| okex 期货 | `BTC.WEEK/USD`, `BTC.WEEK2/USD`, `BTC.MONTH3/USD`, `LTC.WEEK/USD`, ... |