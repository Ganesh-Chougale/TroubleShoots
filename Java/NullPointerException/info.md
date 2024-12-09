`NullPointerException`  
is an error occurs when we assign null value to instance & perform methods on it.    
```java  
		Hello obj = null;
		obj.message();
```  
```bash  

2024-12-06T16:01:59.485+05:30  INFO 15480 --- [noWeb] [           main] com.example.noWeb.NoWebApplication       : Started NoWebApplication in 2.318 seconds (process running for 3.324)
Exception in thread "main" java.lang.NullPointerException: Cannot invoke "com.example.noWeb.Hello.message()" because "obj" is null
	at com.example.noWeb.NoWebApplication.main(NoWebApplication.java:12)

Process finished with exit code 1
```