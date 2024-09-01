pipeline {
	agent{
	label 'mitz-label'
	}
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh 'JAVA_HOME=/home/mitz/slavedir1/jdk-11.0.24 /home/mitz/slavedir1/apache-maven-3.9.8/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			sh 'cp target/Project10.war /home/mitz/slavedir1/apache-tomcat-9.0.93/webapps'
			}}	
}}
			
