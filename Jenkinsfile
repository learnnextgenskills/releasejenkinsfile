 stage('Release') {
        withMaven(maven: 'Maven 3') {
            
                releasedVersion = readFile('pom.xml') =~ '<version>(.+)-SNAPSHOT</version>')[0][1]
                
                    sh "git config user.email muralifmwdba@gmail.com && git config user.name Murali"
                    sh "mvn release:prepare release:perform -Dusername=${username} -Dpassword=${password}"
             
                           
        }
    }