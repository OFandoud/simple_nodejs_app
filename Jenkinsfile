
pipeline {
    agent any

    stages {
        
        stage('Pukking Repo Files') {
            steps {
             git branch: 'main', credentialsId: 'Github-access-token', url: 'https://github.com/OFandoud/simple_nodejs_app.git'
            }
        }
        
        stage('Stage 1') {
            steps {
                sh ''' 
                echo omar fandoud
                    ls
                    cal
                '''
            }
        }
        
    }
}
