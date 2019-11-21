# Mysql 技巧记录

#### 1、解析查询json里面内容（5.7版本以上才ok）
例如：{"order_receive_remind":{"options":{"value":"3"},"type":"options","value":"1"}}<br>
解答：SELECT * FROM purchaser_rule_config where exec_rule_value -> '$.order_receive_remind.value' = '1';

#### 2、mysql 优化为何有用？（逻辑架构）
1、客户端发送消息，服务单响应数据，某刻只有一段在进行，数据大小也有限制;<br>
