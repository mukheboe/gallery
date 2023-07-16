pipeline {

  agent any

  stages {
    stage("Slack"){
            steps{
                slackSend message: 'Build_1 Successful'
            }
        }

    stage("Build_1"){

      steps{
        echo 'build successful'
      }

    }

    stage("Test stage"){

      steps{
        echo 'test Successful'
      }

    }

    stage("Deploy stage"){

      steps{
        echo 'deploying application'
      }

    }

  }
}
