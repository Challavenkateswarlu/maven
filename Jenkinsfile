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
   }
  }
  stage("build")
  {
      steps
      {
          git branch: 'feature', url: 'https://github.com/Challavenkateswarlu/maven.git'
          sh "bash shell.sh"
   }
   stage("jenkins")
  {
      steps
      {
          git branch: 'feature1', url: 'https://github.com/Challavenkateswarlu/maven.git'
   }
}
 }
}
