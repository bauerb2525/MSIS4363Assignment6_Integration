pipeline{
  agent any
  stages{
    stage('Checkout Code'){
      steps{
        git 'https://github.com/bauerb2525/MSIS4363Assignment6_Integration'
      }
    }
    stage('Build'){
      steps{
        sh 'echo "building the app"'
      }
    }
    stage('Test'){
      steps{
        sh 'echo "Running Tests"'
      }
    }
    stage('Deploy'){
      steps{
        sh 'echo "deploying"'
      }
    }
  }
}
 
