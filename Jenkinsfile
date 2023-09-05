pipeline{
    agent any
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
}
}