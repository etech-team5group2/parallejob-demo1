pipeline{
	agent any
		stages{
			parallel{
				stage('1-clone'){
				steps{
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
