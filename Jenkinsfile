pipeline {
    agent any
    stages {
        stage('GET_COMPONENT') {
            steps {
                bat 'gradlew.bat getComponent'
            }
        }
	      stage('LOAD'){
		        steps {
			          bat 'gradlew.bat load'
            }
	      }
        stage('Three') {
            steps {
                bat 'gradlew.bat clean build'
            }
        }
}
}
