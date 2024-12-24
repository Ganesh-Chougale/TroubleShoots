### Analogy of spring STS Console  

<span style="color: white;">**Timestamp**</span>
<span style="color: yellow;">**Log Level**</span>
<span style="color: purple;">**Thread ID**</span>
<span style="color: white;">**---**</span>
<span style="color: grey;">**[Thread Name]**</span>
<span style="color: white;">**[Thread Type]**</span>
<span style="color: skyblue;">**Logger Name**</span>
<span style="color: white;">**:**</span>
<span style="color: grey;">**Log Message**</span>

1) Timestamp	: 2024-12-24T15:53:50.137+05:30
2) Log Level	: <span style="color: green;">Debug</span> | <span style="color: red;">ERROR</span> | <span style="color: green;">Info</span> | <span style="color: yellow;">Warn</span>     
3) Thread ID 	: 956
4) Separator 	: "---"
5) Thread Name	: [Project Name]
6) Thread Type	: [Thread Type]
7) Logger Name	: Classfile Name Generating The Log
8) Separator	: ":"
9) Log Message	: Actual Log Message by the application

Example :
```bash
2024-12-24T15:53:50.137+05:30 INFO 956 --- [ParkingBay] [restartedMain] c.PB.ParkingBay.ParkingBayApplication Started ParkingBayApplication in 2.811 seconds (process running for 1680.005)
```  

<span style="color: white;">Timestamp</span> : <span style="color: white;">**2024-12-24T15:53:50.137+05:30**</span>   
<span style="color: yellow;">Log Level</span> : <span style="color: yellow;">**INFO**</span>   
<span style="color: purple;">Thread ID</span> : <span style="color: purple;">**956**</span>  
<span style="color: white;">---</span> : <span style="color: white;">**---**</span>  
<span style="color: grey;">[Thread Name]</span> : <span style="color: grey;">**[ParkingBay]**</span>  
<span style="color: white;">[Thread Type]</span> : <span style="color: white;">**[restartedMain]**</span>  
<span style="color: skyblue;">Logger Name</span> : <span style="color: skyblue;">**c.PB.ParkingBay.ParkingBayApplication**</span>  
<span style="color: white;">:</span> : <span style="color: white;">**:**</span>  
<span style="color: grey;">Log Message</span> = <span style="color: grey;">**Started ParkingBayApplication in 2.811 seconds (process running for 1680.005)**</span>  