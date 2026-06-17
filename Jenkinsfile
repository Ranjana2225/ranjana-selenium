pipeline{
  agent any{
    tools{
      maven 'Maven'
    }
    stages{
      stage('Checkout'){
        steps{
          git 'https://github.com/Ranjana2225/ranjana-selenium.git'
        }
      }
      stage('compile'){
        steps{
          sh 'mvn compile'
        }
      }
      stage('Test'){
        steps{
          sh 'mvn test'
        }
      }
      stage('Run'){
        steps{
          sh 'mvn exec:java -Dexec.mainClass="com.example.App"'
        }
      }
    }
  }
