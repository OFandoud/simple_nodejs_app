pipeline {
    agent { label 'Slave-machine1' }

    stages {
        
        stage('Pukking Repo Files') {
            steps {
             git branch: "${GIT_BRANCH}", credentialsId: 'Github-access-token', url: 'https://github.com/OFandoud/simple_nodejs_app.git'
            }
        }
        
        stage('Stage 1') {
            steps {
                catchError(buildResult: 'SUCCESS' , stageResult: 'FAILURE'){ 
                sh ''' 
                echo omar fandoud
                    ls /var
                    
                '''
                }
            }
        }
        
         stage('Stage2') {
            steps {
                catchError(buildResult: 'SUCCESS' , stageResult: 'FAILURE'){ 
                sh ''' 
                echo omar fandoud
                   
                    
                '''
                }
            }
        }
    }
}
