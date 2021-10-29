# 消息轨迹

消息轨迹是指一条消息从生产到被消费经过所有节点的链路信息，包括生产与消费轨迹信息，用户可根据消息轨迹获取消息相关链路信息进行相关的业务分析。

## 基本信息

基本消息指消息自身的基本消息，包括所属Topic、Key、Tag、消费状态等信息；

## 生产信息

包括生产者地址、消息发送时间、消息发送耗时、消息发送状态等信息；

## 消费信息

单条消息可能被多个消费组的多个消费者消费，消费消息包括每个消费该条消息消费者的客户端地址、消费状态、消费耗时及投递时间等信息；

## 接入方式

每个用户URocketMQ实例服务端默认已开启消息轨迹属性，客户端需要设置消息轨迹才可使用消息轨迹功能。

[JAVA版本客户端设置消息轨迹示例](https://github.com/apache/rocketmq/tree/rocketmq-all-4.7.1/example/src/main/java/org/apache/rocketmq/example/tracemessage)