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
}
