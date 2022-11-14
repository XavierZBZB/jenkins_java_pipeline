String srcUrl = "${env.srcUrl}"
String branchName = "${branchName}"


pipeline{
    agent any
    
    stages{
        stage("check out"){
            steps{
                script{
                checkout([$class: 'GitSCM', branches: [[name: 'main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'https://github.com/XavierZBZB/jenkins_java_pipeline']]])
                }
            }
        }
    }
}
