learn from http://www.cnblogs.com/woodk/p/5817755.html

##前后端分离导致跨域问题

###使用node开一个本地服务器，然后通过http-proxy设置代理
原理：
node作为中间层先去请求接口，然后再返回数据给本地

node会判断请求  

- 如果请求中有固定字段，比如 “api/”  则为接口，跨域请;
- 如果没有，则返回本地文件;