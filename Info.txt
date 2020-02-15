
1)Install the agent from New Relic UI
  Log in to New Relic
  From the account dropdown in the New Relic UI, select Account settings
  In the right sidebar, download the agent for your platform
2)open newrelic.yml file and edit the following properties
  license_key: 'NewRelicLicenseKey'      (give your NewRelic LicenseKey)
  app_name: SpringMVC                    (give your Applicatin Name)
3)copy this downloaded newrelic folder into Tomcat root foler   (E:\apache-tomcat-8.0.36)
4)add the following entry in E:\apache-tomcat-8.0.36\bin\catalina.bat
  set "JAVA_OPTS=%JAVA_OPTS% -javaagent:E:\apache-tomcat-8.0.36\newrelic\newrelic.jar"
5)start the Tomcat
6)Test the application
7)Go to New Relic and check the Dashboard