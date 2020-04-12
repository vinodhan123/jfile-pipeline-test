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
						echo "Hello again"
						}
					}
			stage('four')
				parallel {
					stage('unit test 1') {
						steps {
							echo "parallel test1 runnig...."
							}
						}
					stage('unit test2') {
						steps {
							echo "parallel test2 running..."
								}
						}
					}
		}
	}
