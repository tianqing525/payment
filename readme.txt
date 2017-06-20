一、工程结构

pay-common-parent      项目的Maven父配置工程

pay-common             公共工程，所有项目均可引用

pay-common-config      公共配置工程

pay-common-core        公共核心工程，service工程共用

pay-common-web         公共web工程，web工程共用

 

pay-api-merchant       商户API工程，商户对接支付平台时使用（如：模拟商城pay-web-shop）

 

pay-facade-account     账户服务接口

pay-facade-bank        银行管理服务接口

pay-facade-banklink    银行后置服务接口

pay-facade-boss        运营服务接口

pay-facade-cost        成本计算服务接口

pay-facade-fee         商户计费服务接口

pay-facade-limit       交易限制服务接口

pay-facade-notify      通知服务接口

pay-facade-payrule     支付规则服务接口

pay-facade-remit       打款服务接口

pay-facade-report      报表服务接口

pay-facade-settlement  结算服务接口

pay-facade-trade       交易服务接口

pay-facade-user        用户服务接口

 

pay-service-account    账户服务

pay-service-bank       银行管理服务

pay-service-banklink   银行后置服务

pay-service-boss       运营服务

pay-service-cost       成本计算服务

pay-service-fee        商户计费服务

pay-service-limit      交易限制服务

pay-service-notify     通知服务

pay-service-payrule    支付规则服务

pay-service-remit      打款服务

pay-service-report     报表服务

pay-service-settlement 结算服务

pay-service-trade      交易服务

pay-service-user       用户服务

 

pay-app-queue-notify   消息队列监听APP

 

pay-timer-report       报表分析定时任务

 

pay-web-bank-receive   银行回调请求信息接收

pay-web-boss           运营管理系统

pay-web-gateway        支付网关

pay-web-notify-receive 通知消息接收

pay-web-portal         门户系统

pay-web-trade          交易接口

 

pay-web-shop           模拟商城

 

二、系统简要功能演示

 

三、技术点介绍

FastDFS分布式文件系统的使用

ActiveMQ消息队列的使用

Redis分布式缓存的使用

admin/123456

运营管理/商户管理,会员管理
pay-service-user test.facade.user.DubboProvider
运营管理/交易管理
pay-service-trade wusc.edu.pay.trade.facade.test.DubboProvider
pay-service-* *.DubboProvider启动dubbo提供者


