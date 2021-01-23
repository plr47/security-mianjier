# security-mianjier（安全面🐔儿）

> 就在刚刚我在写第一段话的时候，不知不觉的写了一段脱口秀，然后把它删了，因为最近心里比较脆弱，比较敏感，不太承受的起吐槽的后果。言归正传，马上就要春招面试了，刷面经一定也是很重要的一个环节，当时自己刷了好多师傅面经，帮助还是很大的，本文就整理一下一些看见过的质量比较高的面经，供今年需要参加春招战场的师傅们有个参考
>
> PS：
>
> 1.  排名不分先后
>
> 		  2. 偏WEB方向的同学	
>    		  3. 不是说你把这些刷完就完了，我是觉得刷完这些然后自己去发散去整理。。毕竟刷面经是个方法，这和刷面试题是有本质区别的，安全能靠刷题变成yyds吗。



## LIST

- 我的好同桌，阿里安全黑盒第一人的维森师傅写给新生们的一封信

  http://blog.wils0n.cn/

- Y1r0nz' blog 分享的一篇面经

  https://yangrz.github.io/blog/2016/12/15/mianshi/

- protosil师傅分享的一篇面经

  https://prontosil.me/posts/ddd168ac/

- 404notfound'blog 分享的一篇面经（我不认识这个师傅，是我组里的师兄强推我，看了他博客文章，确实非常牛X）

  https://4o4notfound.org/index.php/archives/183/

- yulige 传闻中被人打印出来全篇背诵的长亭面经

  http://yulige.top/?p=685

- Decade 师傅的面经，当时我刷面经的时候被很多师傅安利过这篇面经

  https://www.notion.so/offer-md-84a18d453d224adcda10b45e73f7cba7d

- 0xffff'blog 分享的一篇面经

  https://0xffff.one/d/575

- b1cx分享的一篇面经

  https://boluochuixue.top/2020/03/27/%E4%B8%80%E4%BA%9B%E7%94%B2%E6%96%B9%E5%92%8C%E4%B9%99%E6%96%B9%E7%9A%84%E9%9D%A2%E7%BB%8F/



## My thought

个人认为的话，收集的这几篇文章大多都是甲方安全的文章，甲方安全和乙方安全面试可能问到的问题不一样的程度可能有些准备面试的师傅没有意识到，因为我自己是面试的甲方安全的应用安全团队，所以我说一些我个人遇到的，认为的，甲方安全面试中需要比乙方安全面试的时候更加注意的东西。

ps：甲方的蓝军，我还是不随便总结了。

- 做甲方的安全部门的话，问题中可能不会涉及非常多的骚操作，譬如一个SQL注入问题，你需要知道的是原理和防御的手法，在乙方安全的面试中或者是研究性的团队中更深一步的问题可能是各种骚操作、Mysql特殊版本的安全性，不同的数据库引擎可用的一些函数、姿势；乙方可能就会问：“说说真预编译和假编译的区别”（这个问题我师兄问倒了很多人。）
- 面试中可能会更加注重XSS、CSRF、SSRF这种在甲方业务中遇见到非常多的漏洞。
- 不要随便面试大厂的研究团队，各种实验室（例如阿里前沿安全研究团队、腾讯科恩、腾讯玄武、长亭的安全研究等），如果准备面还是要充分的做准备防止浪费面试机会，另外这里也有要说的话
  - 不同大厂对于本科生的态度也不同，例如阿里的前沿安全研究团队基本对学历上是有硬性规定的（非211，985硕士我不能说不可能进，但是几乎不行吧）
  - 要选择去研究团队之前也考虑一下自己的志向以及你真正热爱的东西，如果不是学术研究、技术研究，还是选择去做业务吧，各自发光发热，不是非得所有人都去做研究的，我当时也信誓旦旦说我要做研究，然后面试中我也很矫情的问了：“您觉得阿里安全的工作中（指本组的工作）业务性更强一点还是研究性更强一点”。
- 不同公司、团队对CTF的态度也不一样。听师傅说，腾讯的实验室团队对CTF人才还是很看重的，但我也听说有个师傅面我司的时候，面试官对着他简历上其实真的还不错的好几排奖项说道：“我也很多年没有参加竞赛了，现在的这些比赛含金量我都不太知道”。我司安全部实习生培训上，我数了数所有实习生里面打过CTF的同学，应该是手指头能数过来的。（这里想说明的其实是，安全除了CTF还有好多东西，毕竟你单靠着CTF不能让所有的公司从中创造利润？）。但CTF是一定要打的。。。它不仅帮助你学好基础，也会让你脑子里不断积累trick，都是你自己的知识。
- 技术栈上我们一般有更多的要求，红队能力，SRC有良好的排名、挖过有质量的CVE（CNVD其实说实在的好像。。。面试官很无所谓，甚至不会问下去）、有大会的演讲经历、写过黑盒扫描器（熟悉启发式爬虫，能够有思路解决一系列的web2.0时代带来的爬不下去的问题），写过白盒扫描器（懂得程序分析，编译原理，污点传播，等等这些关键词）等
- 语言栈上的话，除了PHP至少要会一个吧，大家也都知道，***fastjson***没见过基本判死刑了吧，另外如果语言栈是偏向JAVA的话，Structs2，weblogic，fastjson，Common-collections，Dubbo，Hessian，kyro，readObject，这些关键词还是要熟悉的吧。。。另外一个比较重要的建议<span style="color:red">非常建议使用p神的docker环境进行漏洞复线，但是我更加建议自己去搭建环境然后debug</span>
- 代码审计，不只是找到敏感函数那么简单，CMS的审计也只是代码审计的一小小小小小小小小部分。



## 写在后面

- 谨代表个人想法
- 欢迎师傅补充面经以及想法
- 祝师傅们面试愉快，过个好年，拿了offer，毕业季好好找个妹妹逛逛自己大学的城市。

