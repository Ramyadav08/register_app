pipeline{
	agent {label 'jenkins-agent'}
	tools{
		jdk 'java17'
		maven 'maven3'
	}
	stages{
		stage("cleanwork space"){
			steps{
				cleanWs()
		}
		
	}
		stage("Checkout from SCM"){
                steps {
                    git branch: 'main', credentialsId: 'github', url: 'https://github.com/Ashfaque-9x/register-app'
                }
        }

}
}
