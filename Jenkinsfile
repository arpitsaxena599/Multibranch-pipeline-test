pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {

    stage('Print Java') {

      steps {

        sh 'mvn -version'

      }

    }
    stage('cat README') {

      when {
            branch "source1"
          }
      steps {
         sh 'cat Jenkinsfile'
      }

    }
    stage('Saying Hello') {
      when {
        branch "source2"
      }
      steps {
      echo "hello motherfu***r, i am here kill me"
            }
    }
    
    stage('Greeting') {
    
    when {
        branch "source1"
      }
  
    steps {
      echo "hy Surprise Motherf***r"
      }
    
   }
 
 }

}
