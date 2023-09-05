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
}
}