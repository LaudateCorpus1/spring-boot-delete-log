# spring-boot-delete-log
This is to try to address the question at here
the https://stackoverflow.com/questions/56305269/how-to-get-log-file-deletion-to-work-with-spring-boot-starter-log4j2

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v2.0.0.RELEASE)

2019-05-25 09:38:33.756  INFO WINDOWS-ESDA5FC --- [           main] c.e.SpringBootDeleteLogApp               : Starting SpringBootDeleteLogApp on WINDOWS-ESDA5FC with PID 17236 (C:\Users\dotha\IdeaProjects\spring-boot-delete-log\target\classes started by dotha in C:\Users\dotha\IdeaProjects\spring-boot-delete-log)
2019-05-25 09:38:33.760  INFO WINDOWS-ESDA5FC --- [           main] c.e.SpringBootDeleteLogApp               : No active profile set, falling back to default profiles: default
2019-05-25 09:38:33.798  INFO WINDOWS-ESDA5FC --- [           main] s.c.a.AnnotationConfigApplicationContext : Refreshing org.springframework.context.annotation.AnnotationConfigApplicationContext@338fc1d8: startup date [Sat May 25 09:38:33 CDT 2019]; root of context hierarchy
2019-05-25 09:38:33,802 main TRACE DefaultRolloverStrategy.purge() took 3.0 milliseconds
2019-05-25 09:38:33,804 main DEBUG RollingFileManager executing synchronous FileRenameAction[logs\log4j2-demo.log to logs\log4j2-demo-2019-05-25-2.log, renameEmptyFiles=false]
2019-05-25 09:38:33,805 main TRACE Renamed file C:\Users\dotha\IdeaProjects\spring-boot-delete-log\logs\log4j2-demo.log to C:\Users\dotha\IdeaProjects\spring-boot-delete-log\logs\log4j2-demo-2019-05-25-2.log with Files.move
2019-05-25 09:38:33,806 main DEBUG RollingFileManager executing async CompositeAction[DeleteAction[basePath=logs, options=[], maxDepth=1, conditions=[IfFileName(glob:log4j2-demo-*.log), IfLastModified(age=PT1M)]]]
2019-05-25 09:38:33,806 main DEBUG Now writing to logs/log4j2-demo.log at 2019-05-25T09:38:33.806-0500
2019-05-25 09:38:33,807 Log4j2-TF-2-RollingFileManager-3 DEBUG Starting DeleteAction[basePath=logs, options=[], maxDepth=1, conditions=[IfFileName(glob:log4j2-demo-*.log), IfLastModified(age=PT1M)]]
2019-05-25 09:38:33,809 Log4j2-TF-2-RollingFileManager-3 DEBUG DeleteAction complete in 0.001881032 seconds
2019-05-25 09:38:33,810 Log4j2-TF-2-RollingFileManager-3 TRACE Sorted paths:
2019-05-25 09:38:33,810 Log4j2-TF-2-RollingFileManager-3 TRACE logs\log4j2-demo.log (modified: 2019-05-25T14:38:33.807885Z)
2019-05-25 09:38:33,812 Log4j2-TF-2-RollingFileManager-3 TRACE logs\log4j2-demo-2019-05-25-2.log (modified: 2019-05-25T14:38:33.803895Z)
2019-05-25 09:38:33,812 Log4j2-TF-2-RollingFileManager-3 TRACE logs\log4j2-demo-2019-05-25-1.log (modified: 2019-05-25T14:36:13.862034Z)
2019-05-25 09:38:33,812 Log4j2-TF-2-RollingFileManager-3 TRACE IfFileName REJECTED: 'glob:log4j2-demo-*.log' does not match relative path 'log4j2-demo.log'
2019-05-25 09:38:33,812 Log4j2-TF-2-RollingFileManager-3 TRACE Not deleting base=logs, relative=log4j2-demo.log
2019-05-25 09:38:33,812 Log4j2-TF-2-RollingFileManager-3 TRACE IfFileName ACCEPTED: 'glob:log4j2-demo-*.log' matches relative path 'log4j2-demo-2019-05-25-2.log'
2019-05-25 09:38:33,813 Log4j2-TF-2-RollingFileManager-3 TRACE IfLastModified REJECTED: log4j2-demo-2019-05-25-2.log ageMillis '9' < 'PT1M'
2019-05-25 09:38:33,813 Log4j2-TF-2-RollingFileManager-3 TRACE Not deleting base=logs, relative=log4j2-demo-2019-05-25-2.log
2019-05-25 09:38:33,813 Log4j2-TF-2-RollingFileManager-3 TRACE IfFileName ACCEPTED: 'glob:log4j2-demo-*.log' matches relative path 'log4j2-demo-2019-05-25-1.log'
2019-05-25 09:38:33,813 Log4j2-TF-2-RollingFileManager-3 TRACE IfLastModified ACCEPTED: log4j2-demo-2019-05-25-1.log ageMillis '139951' >= 'PT1M'
2019-05-25 09:38:33,813 Log4j2-TF-2-RollingFileManager-3 TRACE Deleting logs\log4j2-demo-2019-05-25-1.log
