pipeline {
    agent any 
    stages {
        stage('Build') { 
	    agent any
            steps {
                sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
// Script //
node {
  stage('Build') {
      sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
  }
}

