node {
	stage ('SCM checkout'){
		git "https://github.com/sunil848/selenium-Jenkinspipeline"
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
