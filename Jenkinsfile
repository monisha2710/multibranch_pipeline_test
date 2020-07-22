pipeline{
	agent any
	environment{
		PATH = "C:\\WINDOWS\\SYSTEM32;C:\\Program Files\\Java\\jdk1.8.0_121\\bin"
	}
	stages{
		stage("Compile"){
			steps{
				bat 'javac HelloWorld.java'
			}
		}
		
		stage("Run"){
			steps{
				bat 'java HelloWorld'
			}
		}
	}
}
