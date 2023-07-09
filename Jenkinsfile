pipeline {

  agent any

  stages {
    stage("Slack"){
            steps{
                slackSend message: 'Build_1 Successful'
            }
        }

    stage("Istall dependacies"){

      steps{
        echo 'install dependacies'
      }

    }

    stage("Build_1"){

      steps{
        echo 'Build Successful'
      }

    }

    stage("Deploy to Render"){

      steps{
        echo 'deploying application'
      }

    }

  }
}
