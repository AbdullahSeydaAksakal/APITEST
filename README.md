# ApiIntegrationTest
This project is an integration test project that checks the result (http status) of the JSON API request.   <br /><br />
## Project Features
* It is a project for API integration automation in Java with Rest-Assured.
* Url: http://generator.swagger.io
* Selected Endpoint: /api/gen/clients
* Request methods in the project: POST and GET
* JUnit library is used for Assertion.
* The project prints the Response status code and response information as output.
* If the Response Status code is not 200, it fails and gives "Assertion Error".

## Task Requests

-Write an integration test that checks the result (http status) of the JSON API request. <br />
(Sample url: http://generator.swagger.io)  <br />
-If the Http status code for each GET and POST endpoint selected by you gives 200, it should be reported as successful, otherwise it should be reported as unsuccessful.

## Test Output

RESULT WITH INCORRECT POST DATA  <br />
```
Response POST Body is =>  {"code":500,"type":"unknown","message":"something bad happened"}
Response POST Status Code =>  500

java.lang.AssertionError: 
Expected :200
Actual   :500
<Click to see difference>


	at org.junit.Assert.fail(Assert.java:89)
	at org.junit.Assert.failNotEquals(Assert.java:835)
	at org.junit.Assert.assertEquals(Assert.java:647)
	at org.junit.Assert.assertEquals(Assert.java:633)
	at IntegrationTest.PostClients(IntegrationTest.java:73)
  .
  .
  .

Response GET Body is =>  ["ada","akka-scala","android","apex","bash","clojure","cpprest","csharp","csharp-dotnet2","cwiki","dart","dart-jaguar","dynamic-html","eiffel","elixir","elm","erlang-client","flash","go","groovy","haskell-http-client","html","html2","java","javascript","javascript-closure-angular","jaxrs-cxf-client","jmeter","kotlin","lua","objc","perl","php","powershell","python","qt5cpp","r","ruby","rust","scala","scala-gatling","scalaz","swagger","swagger-yaml","swift","swift3","swift4","swift5","tizen","typescript-angular","typescript-angularjs","typescript-aurelia","typescript-fetch","typescript-inversify","typescript-jquery","typescript-node"] 
Response GET Status Code =>  200 

```

RESULT WITH CORRECT POST DATA  <br />

```

Response POST Body is =>  {"code":"02157b40-9d4e-4e73-b335-61781ea342ce","link":"https://generator.swagger.io/api/gen/download/02157b40-9d4e-4e73-b335-61781ea342ce"} 
Response POST Status Code =>  200 
Response GET Body is =>  ["ada","akka-scala","android","apex","bash","clojure","cpprest","csharp","csharp-dotnet2","cwiki","dart","dart-jaguar","dynamic-html","eiffel","elixir","elm","erlang-client","flash","go","groovy","haskell-http-client","html","html2","java","javascript","javascript-closure-angular","jaxrs-cxf-client","jmeter","kotlin","lua","objc","perl","php","powershell","python","qt5cpp","r","ruby","rust","scala","scala-gatling","scalaz","swagger","swagger-yaml","swift","swift3","swift4","swift5","tizen","typescript-angular","typescript-angularjs","typescript-aurelia","typescript-fetch","typescript-inversify","typescript-jquery","typescript-node"] 
Response GET Status Code =>  200 


```
