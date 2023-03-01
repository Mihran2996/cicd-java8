node{
  stage('SCM Checkout'){
    git 'https://github.com/Mihran2996/cicd-java8'
    git branch: "${main}"
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
