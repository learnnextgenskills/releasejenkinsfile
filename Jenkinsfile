pipeline {
    agent any
	stages {
     stage('Release') {
      steps {
        withMaven(maven: 'mvn') {
                 dir('app') {
                    sh "git config user.email muralifmwdba@gmail.com && git config user.name Murali"
                    sh "mvn release:prepare release:perform -Dusername=${username} -Dpassword=${password}"
             }
                           
        }
    }
	}
	}
}
	