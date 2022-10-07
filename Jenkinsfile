pipeline {
    agent any
    tools {
        maven "MAVEN3"
        jdk "OracleJDK8"
    }
    
    environment {
<<<<<<< HEAD
        NEXUS-USER = 'admin'
	    NEXUS-PASS = 'admin123'
	    RELEASE-REPO = 'vprofile-release'
	    CENTRAL-REPO = 'vpro-maven-central'
	    NEXUSIP = '172.31.40.10'
	    NEXUSPORT = '8081'
	    NEXUS-GRP-REPO = 'vpro-maven-group'
=======
        SNAP-REPO = 'vprofile-snapshot'
	NEXUS-USER = 'admin'
	NEXUS-PASS = 'admin123'
	RELEASE-REPO = 'vprofile-release'
	CENTRAL-REPO = 'vpro-maven-central'
	NEXUSIP = '172.31.40.10'
	NEXUSPORT = '8081'
	NEXUS-GRP-REPO = 'vpro-maven-group'
>>>>>>> 0da286261db58f7b29e688b055ccdebc8896a00d
        NEXUS-LOGIN = 'nexuslogin'
    }

    stages {
        stage('Build'){
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}
