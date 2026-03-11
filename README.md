# java-log-config
Simple log4j2 log config for java applications
keep the log4j2-spring.xml file in resource folder, where application.properties lives.

In the Standalone tomcat server, log file will be created inside catalina.base/logs
on the local system log file will be created in the project directory ./logs/api-service.log  <<-- like this

# IMPORTANT
Add final name for jar/war file in pom.xml inside <build> section

  <build>
		<finalName>api-service</finalName>
		<resources>
			<resource>
				<directory>src/main/resources</directory>
				<filtering>true</filtering>
			</resource>
		</resources>
  <build/>
