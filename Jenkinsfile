pipeline{
  agent any
  stages {
    stage('One') {
      steps {
        echo 'Hi, this is kelvin Duan'
      }
    }
    
    stage('Two') {
      steps {
        input('Do you want to proceed?')
      }
    }
    
    stage('Three') {
      when {
        not {
          branch "master"
        }
      }
      
      steps {
        echo "Hello"
      }
    }
  }
}
