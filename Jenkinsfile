pipeline {
    agent any
    tools {
        maven "MAVEN3"
        jdk "OracleJDK8"
    }
    
    environment {
        NEXUS-USER = 'admin'
	    NEXUS-PASS = 'admin123'
	    RELEASE-REPO = 'vprofile-release'
	    CENTRAL-REPO = 'vpro-maven-central'
	    NEXUSIP = '172.31.40.10'
	    NEXUSPORT = '8081'
	    NEXUS-GRP-REPO = 'vpro-maven-group'
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