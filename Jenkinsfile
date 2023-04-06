pipeline{
	agent any
		stages{
			parallel{
				stage('1-clone'){
				steps{ 
					checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '6a94cd96-5180-492d-b3ff-1f7d6d9a98f9', url: 'https://github.com/etech-team5group2/parallejob-demo1.git']])
					sh'action1'
				}
			}

			stage('2-build'){
				steps{
					sh'action2'			
				}
			}	
			}
			stage('3-seccheck'){
				steps{
					sh'action3'
				}
			}
			
		}

}
