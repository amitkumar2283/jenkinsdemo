pipeline {
  agent any
  stages{
    stage('parallel execution'){
    parallel{
      stage ('compile'){
       agent {  label 'node1'}
       steps{
        echo "Compiling..."
        echo "more compilation.."
       }
     }
     stage ('test'){
       agent {  label 'master'}
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
