pipeline{
	agent any
	environment{
		PATH = "C:\\WINDOWS\\SYSTEM32;C:\\Program Files\\Java\\jdk1.8.0_121\\bin"
	}
	stages{
		stage("Compile"){
			steps{
				bat 'javac hello.java'
			}
		}
		
		stage("Run"){
			steps{
				bat 'java hello'
			}
		}
		
		stage("Publish checks"){
			steps{
				recordIssues aggregatingResults: true, enabledForFailure: true, tools: [java(reportEncoding: 'UTF-8')]
			}
		}
	}
}
