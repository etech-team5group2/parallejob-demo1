pipeline{
	agent any
		stages{
			stage('1-clone'){
				steps{
					checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '6a94cd96-5180-492d-b3ff-1f7d6d9a98f9', url: 'https://github.com/etech-team5group2/parallejob-demo1.git']])
				}
			}

			stage('2-Parallel-job-build'){
				parallel{
					stage('1-subjob1'){
						steps{
							sh'lsblk'			
				}
				}
				
			
			stage('2-subjob2-seccheck'){
				steps{
					sh'lscpu'
				}
			}
			stage('3-subjob3-deploy'){
				steps{
					sh 'sudo systemctl status jenkins'
				}
				
			}
			
		}
	}
}
}
