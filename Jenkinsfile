pipeline {
    agent any
    stages {
        stage('configure jobs') {
            steps {
                jobDsl ignoreMissingFiles: true, failOnMissingPlugin: true, removedConfigFilesAction: 'DELETE', removedJobAction: 'DELETE', removedViewAction: 'DELETE', targets: 'jobs/**/*.groovy', unstableOnDeprecation: true
            }
        }
    }
}
