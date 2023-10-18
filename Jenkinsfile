pipeline{
	agent any
	stages{
		stage('1-clonecode'){
			steps{
				sh 'checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'team7', url: 'https://github.com/eric-prosper001/My-work1.git']])'
			}
		}
		parallel{
			stage('2-1-paralleljob1'){
				steps{
					echo "Ation1"
				}
			}
			stage('2-2-paralleljob2'){
				steps{
					echo "Ation2"
				}
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