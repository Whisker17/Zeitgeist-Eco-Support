# User Data Monitor

该项目旨在做一个用户友好度高的个人市场数据显示程序

### 链接钱包

https://polkadot.js.org/docs/extension/usage

### My Markets

显示自己参与的市场情况，需要根据市场状态进行分类

Todo：

1. 需要一个可以根据地址获得参加过的市场的 ID 的接口
2. 问题是即使进行了交易也有可能已经卖出所有的 shares 了，就不该出现在 My Markets 界面中了，目前 app 中的解决方案是采用一个后端的 DB 记录，用户的每一笔操作都会写入 DB 中

### 推荐市场

根据市场的参与情况，对用户进行市场推荐

### 收益情况

需要根据 APY 和投资组合收益进行分类