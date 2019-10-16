pipeline {
    agent { label 'master' } 
    stages {
        stage('Example Build') {
            steps {
                sh "curl -H 'X-Status: Awesome2' https://enn5ozjlow7n.x.pipedream.net/"
                sh 'printenv'
            }
        }
    }
    post { //post deployment tasks
        always{
            deleteDir()
        }
        success {echo '''\033[1;42mSUCCESS!!!\033[0m'''}
        failure {echo '''\033[1;41mFAILURE!!!\033[0m'''}
    }
}