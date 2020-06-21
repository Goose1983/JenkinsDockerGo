pipeline {
    agent any
    //tools {
    //    'org.jenkinsci.plugins.docker.commons.tools.DockerTool' 'docker_latest'
    //}
    // environment {
    //     DOCKER_CERT_PATH = credentials('id-for-a-docker-cred')
    // }
    stages{
        stage ('Checkout'){
            steps{
                git branch: 'master', credentialsId: 'aa4b9591-3ec7-4550-8193-53afbb0d4252', url: 'https://github.com/Goose1983/JenkinsDockerGo.git'
            }
        }
        stage('Test docker') {
            steps {
                sh 'docker version'
            }
        }
    }
}
