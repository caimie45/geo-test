pipeline{
    agent any
    stages{
        stage('maven clean'){
            steps{
                sh '/opt/maven/binmvn clean'
            }
        }
        stage('maven install'){
            steps{
                sh 'mvn install'
            }
        }
        stage('maven package'){
            steps{
                sh 'mvn package'
            }
        }

    }
}