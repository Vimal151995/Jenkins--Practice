pipeline {
    agent any
    
    stages{
        stage ("Build") {
            steps {
                echo "This is build stage in branch1"
            }
        }
        stage ("Test") {
			parallel {
				stage ("Unit Test") {
					steps {
						echo "This is test stage in branch 1"
						echo "Unit Testing in progress"
						echo "Unit Testing completed"
					}
				
				}	
				stage ("Regression Test") {
					
					steps {
						echo "This is regression test stage in branch 1"
						echo "Regression Testing in progress"
						echo "Regression Testing completed"
					}
				}
			}
		}
        stage ("Deploy") {
            steps {
                echo "This is deploy stage in branch 1"
            }
        }
    }
}
