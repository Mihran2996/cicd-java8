node{
  stage('SCM Checkout'){
    git 'https://github.com/Mihran2996/cicd-java8'
  }
  stage('Compile-Package'){
    git branch: "main", url: 'https://github.com/Mihran2996/cicd-java8.git'
    //Get maven home path
    def mvnHome = tool name: 'maven 3.9.0', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email-Notification'){
    //for this i created App Password in gmail and puted it jenkins config
    mail bcc: '', body: '''Hi Mihran, Welcome To Jenkins.
    Your job has started. Thanks!''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'maruqyanmihran@gmail.com'
  }
}
