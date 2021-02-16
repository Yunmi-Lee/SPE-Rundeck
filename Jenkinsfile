pipeline {
   agent any

   stages {
      stage('Deploy on Node') {
      steps {
        script {
          step([
            $class: "RundeckNotifier",
            includeRundeckLogs: true,
            rundeckInstance: "Rundeck server",
            jobId: "fc18873a-0894-4f90-a5d9-23c12764f75c",
            shouldWaitForRundeckJob: true,
            shouldFailTheBuild: true,
            tailLog: true
          ])
        }
      }
    }
   }
}
