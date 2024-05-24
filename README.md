# onvif方面知识交流
先说结果: 我查了半天onvif client方面的开源库, 发现数量很少, star数很少, 而且早已不更新, ***不建议使用这样的开源库.*** 如果你需要参考的话, 请参照下面链接:
https://github.com/hummatli/onvif-qt-server-client 8年前的东西了, 只有200多个star, ONVIF的标准最新的更新是***ONVIF Profile协议概述v3.0（2023年7月)***

### 原因分析:
1. 安防行业虽然技术门槛低, 但有着一颗并不开放的心. 在商业化的背景下，厂商更倾向于保护自己的技术和产品，而不是将其开源。这也限制了ONVIF开源项目的发展和热度。例如海康威视,从硬件到解决方案,一体化. 占领绝大多数市场, 其它的厂商跟着能喝点汤…… 它不开源, 它只是通过硬件占有率,占领市场. 当然,它也支持ONVIF, 只是这种支持, 更像是ONVIF为了让它支持而定义的标准.
2. ONVIF（Open Network Video Interface Forum）按名字翻译应该是“开放网络视频接口研讨会/论坛”. 听这名字就知道了, 它离“标准”还有一定的距离. 但实际上它只是推出了一系列功能点和接口名称, 以WSDL+XML的方式. 它的视频流则以RTP/RTSP来实现. so, 这里面没有一个是它原创的技术, 它只是一个行业规范. 其目的是“呼吁不同厂商所提供的产品，均可以通过一个统一的“语言”来进行交流。方便了系统的集成。”

### ONVIF方面的知识
1. https://zhuanlan.zhihu.com/p/552989716 《技术解码｜Onvif协议》
2. https://www.onvif.org/ch/profiles-add-ons-specifications/ 《ONVIF 官方的Profile文件、附加组件及规范》
3. https://www.onvif.org/wp-content/uploads/2018/08/ONVIF_Profile_-S_Specification_v1-2.pdf 如果是做视频监控系统,那么主要关注Profile S这个规范.
4. 在《技术解码｜Onvif协议》中提到了“ONVIF Device Test Tool” 这个工具, 下载地址是 https://www.onvif.org/profiles/conformance/device-test-2/ 但很可惜, 它要求注册的邮箱必须是公司邮箱.😂 我突然明白,为啥ONVIF这么冷门了……
