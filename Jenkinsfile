pipeline {

  agent any

  options { timestamps() }
 
  stages {

    stage('Checkout') { steps { checkout scm } }

    stage('Restore')  { steps { bat 'dotnet restore' } }

    stage('Build')    { steps { bat 'dotnet build --configuration Release --no-restore' } }

    stage('Test')     { steps { bat 'dotnet test --configuration Release --no-build --logger trx' } }

  }
 
  post {

    success { echo '✅ Build succeeded!' }

    failure { echo '❌ Build failed. Check logs.' }

  }

}

 
