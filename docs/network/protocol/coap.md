### Constrained Application Protocol

CoAP 是受限制的应用协议(Constrained Application Protocol)的缩写。在 IoT 物联网场景，为了让小设备可以接入互联网，CoAP 协议被设计出来。CoAP 是一种应用层协议，它运行于 UDP 协议之上而不是像 HTTP 那样运行于 TCP 之上。CoAP 协议非常小巧，最小的数据包仅为 4 字节。

CoAP 是一种面向网络的协议，采用了与 HTTP 类似的特征，核心内容为资源抽象、REST 式交互以及可扩展的头选项等。为了克服 HTTP 对于受限环境的劣势，CoAP 既考虑到数据报长度的最优化，又考虑到提供可靠通信。

一方面，CoAP 提供 URI，REST 式的方法如 GET，POST，PUT 和 DELETE，以及可以独立定义的头选项提供的可扩展性。

另一方面，CoAP 基于轻量级的 UDP 协议，并且允许 IP 多播。为了弥补 UDP 传输的不可靠性，CoAP 定义了带有重传机制的事务处理机制。并且提供资源发现机制，并带有资源描述。

![image](https://user-images.githubusercontent.com/13718575/125593184-743d87ff-e640-45e5-9f85-3771ea9660e1.png)

#### [维基百科](https://www.wikiwand.com/en/Constrained_Application_Protocol)

#### [RFC List](https://datatracker.ietf.org/doc/search?name=coap&sort=&rfcs=on&by=group&group=) 

![image](https://user-images.githubusercontent.com/13718575/125595713-dcee8f1c-8a45-4ff0-af19-7606f12dfb98.png)

比较成熟且活跃的实现：

- [https://github.com/plgd-dev/go-coap](https://github.com/plgd-dev/go-coap)
- [https://github.com/Covertness/coap-rs](https://github.com/Covertness/coap-rs)
- [https://github.com/obgm/libcoap](https://github.com/obgm/libcoap)

社区网站：

- [https://coap.technology/](https://coap.technology/)
