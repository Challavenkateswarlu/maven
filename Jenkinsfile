pipeline {
    agent any

    stages {
  stage("git")
  {
   steps
   {
    git branch: 'main', url: 'https://github.com/Challavenkateswarlu/maven.git'
   }
  }
  stage("run")
  {
   steps
   {
    sh "mvn clean"
    sh "mvn install"
    sh "bash shell.sh"
   }
  }
 }
}
