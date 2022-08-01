pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

    stage('Print Java') {

      steps {

        sh 'java -version'

      }

    }
    stage('cat README') {

      when {
            branch "source1"
          }
      steps {
         sh 'cat README.md'
      }

    }
    stage('Saying Hello') {
      when {
        branch "source2"
      }
      steps {
      echo "hello motherfu***r"
            }
    }
    
    stage('Greeting') {
    
    when {
        branch "source1"
      }
  
    steps {
      echo "Surprise Motherf***r"
      }
    
   }
 
 }

}
