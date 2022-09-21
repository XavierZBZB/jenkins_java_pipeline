String srcUrl = "${env.srcUrl}"
String branchName = "${branchName}"


pipeline{
    agent any
    
    stages{
        stage("check out"){
            steps{
                script{
                checkout([$class: 'GitSCM', branches: [[name: "${branchName}" ]], extensions: [], userRemoteConfigs: [[credentialsId: '06612214-df29-49c3-a66f-3a87df1f042e', url: '${srcUrl}']]])
                }
            }
        }
    }
}