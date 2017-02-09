# Virtualization for pre-deployment testing

###Application Development Optimization:
 * Cucumber can be used with SpringBoot application for effectively implementing various testing strategies (like BehaviourDrivenDevelopment and TestDrivenDevelopment)
 * Mockito can be used for mocking the services and verifying if any flow is called with right parameters while testing.
 * Service virtualization avoids the need of altering the application behaviour during integration testing done at pre deployment stage.
   * Use "Fongo" libraies for virtualizing MongoDB (Eg: https://github.com/ravikalla/springboot-mongo-fongo)
   * Use "Hoverfly" libraries for API virtualization
 * Use "CA Service Virtualization" or "SoapUI NG Pro" for Post deployment service virtualization
 * Limit the number of regression test cases in post deployment testing to 10% of overall test cases. Everything should be tested in pre-deployment stage
 * Implement CI/CD pipeline with help of Github, Jenkins, Sonar, Artifactory and Docker on cloud(like AWS)
 * Use continuous communication channel (With tools like Gitter, Mattermost, Yammer, Slack) though which entire team will be notified immediately when CI/CD pipeline fails
 * Use tools to monitor delivery pipeline (Eg: https://github.com/capitalone/Hygieia)
