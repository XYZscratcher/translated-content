---
title: 中间人攻击（MitM）
slug: Glossary/MitM
---
中间人攻击（**Man-in-the-middle attack，**MitM）会在消息发出方和接收方之间拦截双方通讯。举例来说，路由器就可以被破解用来进行中间人攻击。

用日常生活中的写信来类比的话：你给朋友写了一封信，邮递员可以把每一份你寄出去的信都拆开看，甚至把信的内容改掉，然后重新封起来，再寄出去给你的朋友。朋友收到信之后给你回信，邮递员又可以拆开看，看完随便改，改完封好再送到你手上。你全程都不知道自己寄出去的信和收到的信都经过邮递员这个“中间人”转手和处理——换句话说，对于你和你朋友来讲，邮递员这个“中间人”角色是不可见的。

对于实际生活中的信件沟通和线上的信息交流来说，中间人攻击都是很难防范的，这里有一些小建议：

- 不要忽视浏览器弹出的证书警告！你可能访问的是钓鱼网站或者假冒的服务器；
- 公共网络环境下（例如公共 WiFi），没有 HTTPS 加密的敏感网站不要随便登录，一般不可信；
- 在任何网站上登录自己的账号前确保网址是走的 HTTPS 加密协议；

## 更多资料

- OWASP 文章：[Man-in-the-middle attack](https://www.owasp.org/index.php/Man-in-the-middle_attack)
- 维基百科：[Man-in-the-middle attack](https://en.wikipedia.org/wiki/Man-in-the-middle_attack)
- The {{HTTPHeader("Public-Key-Pins")}} header ({{Glossary("HPKP")}}) can significantly decrease the risk of MITM by instructing browsers to require a whitelisted certificate for all subsequent connections to that website.
