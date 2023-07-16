pipeline {

  agent any
  tnode {
  def nodeHome = tool name: 'node-5.10.1', type: 'jenkins.plugins.nodejs.tools.NodeJSInstallation'
  sh "${nodeHome}/bin/node -v"
}
  
  stages {
    stage("Slack"){
            steps{
                slackSend message: 'Build_1 Successful; Heroku link>https://git.heroku.com/mukheboe/gallery.git'
            }
        }

    stage("Build_1 stage"){

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
    stage('Deploy to Heroku') {
  steps {
    withCredentials([usernameColonPassword(credentialsId: 'heroku', variable: 'HEROKU_CREDENTIALS' )]){
      sh 'git push https://${HEROKU_CREDENTIALS}@git.heroku.com/mukheboe/gallery.git master'
    }
  }
} 

  }
}
