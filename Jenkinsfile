pipeline {
    agent any
    stages {
        stage('GET_COMPONENT') {
            steps {
                bat 'gradlew.bat getComponent -P component=PopCommerce'
            }
        }
	      stage('LOAD'){
		        steps {
			          bat 'gradlew.bat load'
            }
	      }
        stage('BUILD') {
            steps {
                bat 'gradlew.bat clean build'
            }
        }
}
}
