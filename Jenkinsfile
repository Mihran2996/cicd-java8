node{
  stage('SCM Checkout'){
    git 'https://github.com/Mihran2996/cicd-java8'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
