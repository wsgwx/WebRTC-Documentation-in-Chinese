## 9.2 媒体流

### 9.2.1 id

`MediaStream`指定的id属性返回了对流唯一的id，这样`RTCPeerConnection API`的远程端就可以识别媒体流。

当媒体流被创建用来表示从远程对等体获得的流时，id属性是通过远程源提供的信息初始化的。

> NOTE:MediaStream对象的id对于流的源是唯一的，但这并不意味着不可能以重复项结束。例如，本地生成的流的轨道可以使用`RTCPeerConnection`从一个用户代理发送到远程对等体，然后以相同的方式发送回原始用户代理，在这种情况下，原始用户代理将得到具有相同id的多条流（本地生成的id和从远程对等体发送的id）。



