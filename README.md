# TICK-pub/sub

## 構成

Producer - (multi cast) - Server - (gRPC) - Client

### Producer

Tickをmulti castで配信<br>

### gRPC Server

Tickをmulti castで受信<br>
gRPCでClientへ配信

### gRPC Client

TickをgRPCで受信

## Protocol

### multi cast

Producer, Serverを手軽に増設できる<br>
Networkの負荷が小さい<br>
応答の悪いClientからの影響を受けたServerを分離しやすい

### gRPC

etcdに採用され、microserviceへの利用も増えている<br>
HTTP2なので、バイナリを高速に配信でき、Proxyも通しやすい<br>
Protocol Buffers(IDL)でinterfaceを定義し、様々な言語で実装できる

[www.grpc.io](http://www.grpc.io)
