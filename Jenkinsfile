node {
	stage ('SCM checkout'){
		git "https://github.com/rushtojp/selenium-Jenkinspipeline-1.git"
		}
	stage ('Build'){
    	dir("comtest") {
	   sh "mvn clean install"
       }
	}
    stage ('test') {
    	sh "java -jar comtest/target/com.test-1.0-SNAPSHOT.jar"
    }
}
