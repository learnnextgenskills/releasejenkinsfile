pipeline {
    agent any
	stages {
     stage('Release') {
      steps {
        withMaven(maven: 'mvn') {
                 
                    sh "git config user.email muralifmwdba@gmail.com && git config user.name Murali"
                    sh "mvn release:clean release:prepare release:perform -Dusername=learnnextgenskills -Dpassword=ramsai1919"
             
                           
        }
    }
	}
	}
}
	