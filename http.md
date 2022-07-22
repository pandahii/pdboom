#HTTP
### http 响应类型（Content-Type:）类别：
1. 常见的媒体格式类型如下：
- text/html ： HTML格式
- text/plain ：纯文本格式      
- text/xml ：  XML格式
- image/gif ：gif图片格式    
- image/jpeg ：jpg图片格式 
- image/png：png图片格式
2. 以application开头的媒体格式类型：
- application/xhtml+xml ：XHTML格式
- application/xml     ： XML数据格式
- application/atom+xml  ：Atom XML聚合格式    
- application/json    ： JSON数据格式
- application/pdf       ：pdf格式  
-  application/msword  ： Word文档格式
- application/octet-stream ： 二进制流数据（如常见的文件下载）
- application/x-www-form-urlencoded ：form表单数据被编码为key/value格式发送到服务器（表单默认的提交数据的格式）
- multipart/form-data ： 需要在表单中进行文件上传时，就需要使用该格式

3. packetbrat 配置过滤
```
include_body_for: ["text/html", "text/plain", "text/xml", "image/gif", "image/jpeg", "image/png", "application/xhtml+xml", "application/xml", "application/atom+xml", "application/json", "application/pdf", "application/msword", "application/octet-stream", "application/x-www-form-urlencoded",]
```