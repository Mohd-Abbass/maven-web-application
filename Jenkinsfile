node
{
def mavenHome = tool name: "maven3.6.2"

 stage('CheckoutCode')
 {
 git branch: 'development', credentialsId: '5eeba78c-d71f-4b28-9ea7-43117dca14ed', url: 'https://github.com/Mohd-Abbass/maven-web-application.git'
 }
    
 stage ('Build')
 {
 sh "${mavenHome}/bin/mvn clean package"
 }
/*
 stage ('ExecuteSonarqubeReport')
 {
 sh "${mavenHome}/bin/mvn sonar:sonar"
 }
 
 stage ('UploadArtifactIntoNexus')
 {
 sh "${mavenHome}/bin/mvn deploy"
 }
 
 stage ('DeploAppIntoTomcat')
 {
 sshagent(['75468f81-9342-485d-b37f-3eefeddf2c7b']) 
 {
 sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@3.108.196.60:/opt/apache-tomcat-9.0.56/webapps/"
 }
 }
 
 stage ('SendEmailNotification')
 {
 mail bcc: '', body: '''Build over

Regards
Mohd Sohail''', cc: 'mohammed.abbas0332@gmail.com', from: '', replyTo: '', subject: 'Build Over', to: 'mohammed.sohail5010@gmail.com'
 }
*/
}


 
