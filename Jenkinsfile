pipeline{
	agent any
	stages{
		stade('1-clonecode'){
			steps{
				sh 'checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'team7', url: 'https://github.com/eric-prosper001/My-work1.git']])'
			}
		}
		stage('2-artifactbuild'){
			steps{
				sh 'df -h'
			}
		}
		stage('3-unitest'){
			steps{
				sh 'lscpu'
			}
		}
	} 
		
	}
}