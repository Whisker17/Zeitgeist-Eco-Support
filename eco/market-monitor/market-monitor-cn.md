整个项目是为链上数据的一个分析，做一个可视化的界面更直观的表现数据。

## 数据获取

1. 节点高度
2. 每个区块中的交易数量/总交易数量
3. 市场数量

### 节点高度

[demo](https://github.com/Whisker17/sdk-demo/blob/main/src/getBlockInfo.ts)

#### Details

定时刷新节点高度

### 市场数量

[demo](https://github.com/Whisker17/sdk-demo/blob/main/src/getMarketCount.ts)

#### Details

1. 定时刷新/Subscribe 的方式，由于出块时间是一定的，所以比较推荐使用定时查询的方案

### 市场详情

[demo](https://github.com/Whisker17/sdk-demo/blob/main/src/getMarketInfo.ts)

#### Details

1. 通过 id 查询市场详情
2. 通过 `tags` 这个标签进行分类
3. 在一个饼图中可以体现当前市场中比较流行的种类
3. 也可以针对不同状态的市场进行显示

### 质押总量

#### Details

1. 可以根据这个指标排列一个最受欢迎的市场榜单

## 存储

设计后端数据库，可以优化部分查询接口耗时

### Details

1. fetch 到市场后将市场信息进行整理，保存在后台数据库中