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
Networkへの負荷も非常に小さい<br>
応答の悪いClientからの影響を小さくできる

### gRPC
HTTP2なので、バイナリを高速に配信でき、Proxyも通しやすい<br>
様々な言語に対応したライブラリやドキュメントが配布されている<br>
etcdに採用され、microserviceへの利用も増えている

[www.grpc.io](http://www.grpc.io)
