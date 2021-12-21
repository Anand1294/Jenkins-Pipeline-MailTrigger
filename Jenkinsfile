pipeline {
    agent any
    stages {
        stage ('Mail Test') {
            steps {
                error('Crashing the pipeline')
            }
        }
    }
    post {
        always {
                mail body: "This is Jenkins Mail \n Run display URL ${env.RUN_DISPLAY_URL} ",
                subject: "Mail Jenkins",
                to: "shubhamanand1203@gmail.com" 
                /*mail bcc: '', body: "<b>Example</b><br>Project: ${env.JOB_NAME} " +
                "<br>Build Number: ${env.BUILD_NUMBER} <br> URL: ${env.BUILD_URL}",
                cc: '', charset: 'UTF-8', from: '', mimeType: 'text/html',
                replyTo: '',*/
        }
    }
}
