pipeline{
    agent any
    stages{
        stage('mvn clean'){
        steps{
            sh '/opt/maven/bin/mvn clean'
        }
    }
    stage('maven install'){
        steps{
            sh '/opt/maven/bin/mvn install'
            sh '/opt/maven/bin/echo hi'
        }
    }
    stage('maven package'){
        steps{
            sh '/opt/maven/bin/mvn package'
        }
    }
}
}