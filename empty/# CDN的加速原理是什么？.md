# CDN的加速原理是什么？

![CDN节点有缓存场景](https://res-static.hc-cdn.cn/SEO/CDN%E8%8A%82%E7%82%B9%E6%9C%89%E7%BC%93%E5%AD%98%E5%9C%BA%E6%99%AF.jpg)

HTTP请求流程：

1、用户在浏览器输入要访问的网站域名，向本地DNS发起域名解析请求。

2、域名解析的请求被发往网站授权DNS服务器。

3、网站DNS服务器解析发现域名已经CNAME到了www.example.com.c.cdnhwc1.com。

4、请求被指向CDN服务。

5、CDN对域名进行智能解析，将响应速度最快的CDN节点IP地址返回给本地DNS。

6、用户获取响应速度最快的CDN节点IP地址。

7、浏览器在得到速度最快节点的IP地址以后，向CDN节点发出访问请求。

8、CDN节点将用户所需资源返回给用户。



![CDN节点无缓存场景](https://res-static.hc-cdn.cn/SEO/CDN%E8%8A%82%E7%82%B9%E6%97%A0%E7%BC%93%E5%AD%98%E5%9C%BA%E6%99%AF.jpg)

HTTP请求流程：

1、用户在浏览器输入要访问的网站域名，向本地DNS发起域名解析请求。

2、域名解析的请求被发往网站授权DNS服务器。

3、网站DNS服务器解析发现域名已经CNAME到了www.example.com.c.cdnhwc1.com。

4、请求被指向CDN服务。

5、CDN对域名进行智能解析，将响应速度最快的CDN节点IP地址返回给本地DNS。

6、用户获取响应速度最快的CDN节点IP地址。

7、浏览器在得到速度最快节点的IP地址以后，向CDN节点发出访问请求。

8、CDN节点回源站拉取用户所需资源。

9、将回源拉取的资源缓存至节点。

10、将用户所需资源返回给用户。



参考

[https://www.huaweicloud.com/zhishi/cdn001.html](https://www.huaweicloud.com/zhishi/cdn001.html)

[https://segmentfault.com/q/1010000004556003](https://segmentfault.com/q/1010000004556003)

