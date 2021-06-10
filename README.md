# SecureGrpcFuzzer
A Tool for fuzzing GRPC over TLS

## Idea
Only support server-side authentication for now.
1. Dump SSLKEYLOG for decrypt grpc traffic
2. Get server cert
3. Dump proto files
4. Forge payload & wait for crashes

## Tools
* pbtk
  * a great tool to dump proto files 
* grpcurl
  * seems a good tool to re-develop for fuzzing purpose
* grpc python
  * Easy to implement
  
## TODO
mutated payload: crash detect
  -> no response ?
  -> response anomaly?
