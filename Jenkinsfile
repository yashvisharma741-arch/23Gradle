pipeline{
  agent any
    tools{
      gradle 'Gradle'
      jdk 'JDK'
      }
    stages{
      stage('Checkout'){
        steps{
          git branch:'main', url:'https://github.com/yashvisharma741-arch/23Gradle.git'
          }
          }
      stage('Build'){
        steps{
          sh 'gradle build'
          }
          }
      stage('Test'){
        steps{
          sh 'gradle test'
          }
          }
      stage('Run application'){
         steps{
           sh 'gradle run'
           }
           }
           }
     post{
       success{
         echo 'success'
         }
       failure{
         echo 'fail'
         }
         }
         }
                   
