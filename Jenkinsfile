pipeline {

  agent any

  stages {

    stage("Istall dependacies"){

      steps{
        echo 'install dependacies'
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
   post{
        always("Slack"){
            steps{
                slackSend message: 'test message'
            }
        }
    }

}
