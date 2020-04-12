pipeline {
	agent any
		stages {
			stage('one') {
				steps {
					echo "Hi... this is my first test piepline by vino"
					}
			}
			stage('two') {
				steps {
					input("do you want to proceed ?")
					}
			}
			stage('three') {
					when {
						not {
							branch "master"
							}
						}
					steps {
						echo "Hello there agaie"
						}
					}
			stage('four') {
				steps {	
					echo "test reached stage 4"

					}
				}
		}
	}
					
