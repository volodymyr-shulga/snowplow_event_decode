Module content:
 * file with raw snowplow events copied from S3 
 ```2017-05-23-49573334505487429614427513964717871542635044026141638658-49573334505487429614427513964720289394274273284491051010.gz```
 * unarchived file ```2017-05-23-49573334505487429614427513964717871542635044026141638658-49573334505487429614427513964720289394274273284491051010```
 * _collector_payload.thrift_ with thrift events schema
 * java class generated by _collector_payload.thrift_ with thrift version 0.10 and command ```thrift -out . --gen java collector_payload.thrift```
 * _EventDecoder_ class reading events with ElephantBird lib 
 
Elephant bird requires thrift9 profile (greater versions than 0.9 are provided via thrift9 maven profile)
 
To run code from command line use:
 ```mvn exec:java -Pthrift9```
 