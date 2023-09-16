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
                sh '/opt/maven/bimvn install'
            }
        }
        stage('maven package'){
            steps{
                sh '/opt/maven/bimvn package'
            }
        }
        stage('upload artifact'){
        steps{
            sh 'curl --upload-file target/bioMedical-0.0.2-SNAPSHOT.jar -u admin:devops -v http://198.58.119.40:8081/repository/prof-repo/'

    }
}
    }
}