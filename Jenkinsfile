node {
    stage('git') {
        git branch: 'exam', credentialsId: 'docker-hub-hyunilshin', url: 'https://github.com/hyunil-shin/JenkinsPipelineTraining'
    
    }
    
    stage('set unstable') {
        try{
            sh 'exit 2'
        } catch (Exception e) {
           unstable("UNSTABLE")
        }
    } 

    stage('set failure') {
        try{
            sh 'exit 2'
        } catch (Exception e) {
           currentBuild.result = "Success"
        }
    }  

    stage('exectue script') {
        sh 'ls'
    }  
    

    stage('exectue script') {
        sh 'ls'
    }  
}

