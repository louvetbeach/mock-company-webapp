
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   pipeline {
       agent any

       stages {
           stage('Build') {
               steps {
                   echo 'Building the project...'
                   // TODO: more
                   sh './gradlew assemble'
               }
           }
           stage('Test') {
               steps {
                   echo 'Running tests...'
                   // TODO: more
                   sh './gradlew test'
               }
           }
       }

       post {
           always {
               echo 'Cleaning up...'

           }
           success {
               echo 'Build and tests were successful!'
           }
           failure {
               echo 'Build or tests failed!'
           }
       }
   }

