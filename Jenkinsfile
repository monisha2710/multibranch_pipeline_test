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
				publishChecks detailsURL: 'https://github.com/monisha2710/multibranch_pipeline_test', name: 'Jenkins', summary: 'Jenkins checks testing', text: 'Check  1 completed', title: 'Check1'
			}
		}
	}
}
