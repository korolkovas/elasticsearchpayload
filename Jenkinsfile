pipeline {
    agent { label 'master' } 
    stages {
        stage('Example Build') {
            steps {
                sh "curl -H 'X-Status: Awesome2' https://enn5ozjlow7n.x.pipedream.net/"
                sh 'sleep 1'
            }
        }
    }
}