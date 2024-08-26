pipeline{
	agent any
	stages{
		stage(checkout){
			steps{
			git 'https://github.com/mitali-08/Project10.git'
			}
		}
		stage(build){
			steps{
			sh 'mvn install'
			}
		}
		stage(deploy){
			steps{
			sh 'cp target/Project10.war /home/mitali/Documents/devops/apache-tomcat-9.0.93/webapps'
			}
		}
	}
}

			
