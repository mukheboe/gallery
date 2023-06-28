pipeline {

  agent any

  stages {

    stage("Istall dependacies"){

      steps{
        sh 'npm install'
      }

    }

    stage("Build"){

      steps{
        echo 'testing application'
      }

    }

    stage("Deploy to Render"){

      steps{
        echo 'deploying application'
      }

    }

  }

}
