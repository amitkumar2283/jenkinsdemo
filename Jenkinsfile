pipeline {
  agent any
  stages{
    stage('parallel execution'){
    parallel{
      stage ('compile'){
       steps{
        echo "Compiling..."
        echo "more compilation.."
       }
     }
     stage ('test'){
       steps{
        echo "testing..."
        echo "more testing.."
       }
     }
    }
    }
    stage ('Deploy'){
     steps{
       echo "deployment..."
       echo "deployment continues.."
     }
    }

  }
}
