pipeline{
  agent any
  stages{
    stage('Compile stage'){
      steps{
        maven(maven : 'Maven_3.8.1'){
          bat 'mvn clean compile'
        }
      }   
    }
    stage('Testing stage'){
      steps{
        maven(maven : 'Maven_3.8.1'){
          bat 'mvn test'
        }
      }
    }
    stage('Deployment stage'){
      steps{
        maven(maven : 'Maven_3.8.1'){
          bat 'mvn deploy'
        }
      }
    }
  }
}
