### application.properties  
Current Favourite:  
```bash
logging.pattern.console=%clr(%5p) %t --- %logger{36} --- %clr(%m) %n
```  


1. **%5p**: **Log Level** (e.g., INFO, ERROR, DEBUG, WARN).
   - **Example**: `INFO`, `ERROR`

2. **%t**: **Thread Name** (name of the thread that generated the log message).
   - **Example**: `main`, `restartedMain`

3. **%thread**: **Thread Name** (same as `%t`).
   - **Example**: `main`

4. **%logger**: **Logger Name** (the name of the logger, usually the class name).
   - **Example**: `com.example.MyClass`

5. **%logger{length}**: **Logger Name (truncated)** (same as `%logger`, but truncated to the specified number of characters).
   - **Example**: `%logger{10}` for first 10 characters.

6. **%m**: **Log Message** (the message itself, logged by the application).
   - **Example**: `Started ParkingBayApplication in 2.811 seconds`

7. **%M**: **Method Name** (the name of the method that logged the message).
   - **Example**: `main()`

8. **%line**: **Line Number** (the line number where the log statement was generated).
   - **Example**: `42`

9. **%n**: **Newline** (line break between log entries).

10. **%date**: **Timestamp** (date and time of the log entry).
    - **Example**: `2024-12-24T15:53:50.137+05:30`

11. **%d{pattern}**: **Formatted Date** (timestamp with a custom date format).
    - **Example**: `%d{yyyy-MM-dd HH:mm:ss}`

12. **%X{key}**: **Mapped Diagnostic Context (MDC) Value** (value from MDC with the specified key).
    - **Example**: `%X{user}` (prints the value of MDC attribute `user`)

13. **%ex**: **Exception** (prints the exception stack trace).
    - **Example**: `java.lang.NullPointerException: ...`

14. **%replace**: **Pattern Replacement** (replaces part of the log message using a regular expression).
    - **Example**: `%replace(%m){'foo','bar'}` (replaces "foo" with "bar" in the message)

15. **%env**: **Environment Variable** (prints environment variables).
    - **Example**: `%env{HOME}`

16. **%r**: **Relative Time** (prints the time elapsed since the application started).
    - **Example**: `123ms` (123 milliseconds)

17. **%f**: **File Name** (file name where the log statement was made).
    - **Example**: `MyClass.java`

18. **%class**: **Class Name** (the name of the class that generated the log message).
    - **Example**: `com.example.MyClass`

19. **%p**: **Log Level** (shorthand for `%5p`).
    - **Example**: `INFO`

20. **%c**: **Logger Category** (same as `%logger`).

21. **%t**: **Thread ID** (the identifier of the thread that generated the log message).
    - **Example**: `1`