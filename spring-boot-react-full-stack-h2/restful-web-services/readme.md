# Full Stack Application with Spring Boot and React


## Authentication

POST to http://localhost:5000/authenticate

```
{
  "username":"in28minutes",
  "password":"dummy"
}
```

Response
```
{
"token": "eyJhbGciOiJIUzUxMiJ9.eyJzdWIiOiJpbjI4bWludXRlcyIsImV4cCI6MTU2MjIzNDM1OSwiaWF0IjoxNTYxNjI5NTU5fQ.yvkFtYAp8yGClDo7D5wtXyPSnUPtxu8A7A9YCl9FJdjR0di_yAaPcSTR6liN5bIu1SnOJuSZp94pYSYzU_BNEw"
}
```


## Hello World URLS

- http://localhost:5000/hello-world


## Final Plugin Configuration
```
			<plugin>
				<groupId>com.microsoft.azure</groupId>
				<artifactId>azure-webapp-maven-plugin</artifactId>
				<version>1.7.0</version>
				<configuration>
					<schemaVersion>V2</schemaVersion>
					<!-- ServicePlan763a680f-840a-4de0 -->
					<resourceGroup>rest-api-full-stack-rg</resourceGroup>
					<appName>rest-api-full-stack-in28minutes</appName>
					<pricingTier>P1v2</pricingTier>
					<region>westeurope</region>
					<appSettings>
						<property>
							<name>JAVA_OPTS</name>
							<value>-Dserver.port=80</value>
						</property>
					</appSettings>
					<runtime>
						<os>linux</os>
						<javaVersion>java11</javaVersion>
						<webContainer>java11</webContainer>
					</runtime>
					<deployment>
						<resources>
							<resource>
								<directory>${project.basedir}/target</directory>
								<includes>
									<include>*.jar</include>
								</includes>
							</resource>
						</resources>
					</deployment>
				</configuration>
			</plugin>

```