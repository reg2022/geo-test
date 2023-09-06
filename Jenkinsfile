pipeline{
    agent any
    tools{
        maven 'M2_HOME'
    }
    stages{
        stage('mvn clean'){
        steps{
            sh 'mvn clean'
        }
    }
    stage('maven install'){
        steps{
            sh 'mvn install'
            sh 'echo hi'
        }
    }
    stage('maven package'){
        steps{
            sh 'mvn package'
        }
    }
    stage('upload artifact'){
    steps{
        sh 'curl --upload-file target/bioMedical-0.0.1-SNAPSHOT.jar -u admin:devops -v http://ec2-3-84-85-220.compute-1.amazonaws.com:8081/repository/maven-nexus-repo/'
    }
    }
}
}