node{
  stage('SCM Checkout'){
    git 'https://github.com/Mihran2996/cicd-java8'
    git branch: "main", url: 'https://github.com/Mihran2996/cicd-java8.git'
  }
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
