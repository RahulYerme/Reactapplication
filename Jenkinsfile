def str
pipeline{
  agent any
   tools{
     maven 'Apache Maven 3.3.9'
    }
  stages{
    stage("Version Creation" ){
      steps{
        script{
          str = "&{env.GIT_BRANCH}"+++"${env.GIT_BUILD_NUMBER}"
          echo "${str}"
        }
      }
    }
    stage("Build Using Maven Tool"){
      steps{
        script{
           sh "mvn clean package"
        }
      }
    }
  }
}
