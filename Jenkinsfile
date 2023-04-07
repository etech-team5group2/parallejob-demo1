pipeline{
	agent any
		stages{
			stage('1-clone'){
				steps{ 
						sh'action1'
				}
			}

			stage('2-Parallel-job-build'){
				parallel{
					stage('1-subjob1'){
						steps{
							sh'action2'			
				}
				}
				
			
			stage('2-subjob2-seccheck'){
				steps{
					sh'action3'
				}
			}
			stage('3-subjob3-deploy'){
				steps{
					'sh action 3'
				}
				
			}
			
		}
	}
}
}