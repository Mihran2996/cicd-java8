node{
  stage('SCM Checkout'){
    git 'https://github.com/Mihran2996/cicd-java8'
  }
  stage('Compile-Package'){
    git branch: "main", url: 'https://github.com/Mihran2996/cicd-java8.git'
    sh 'mvn package'
  }
}
