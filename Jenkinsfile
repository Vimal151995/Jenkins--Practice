pipeline {
    agent any
    
    stages{
        stage ("Build") {
            steps {
                echo "This is build stage branch 2"
                echo "Code is Building"
            }
        }
        stage ("Test") {
			parallel {
				stage ("Unit Test") {
					steps {
						echo "This is test stage branch 2"
						echo "Unit Testing in progress"
						echo "Unit Testing completed"
					}
				
				}	
				stage ("Regression Test") {
					
					steps {
						echo "This is regression test stage branch 2"
						echo "Regression Testing in progress"
						echo "Regression Testing completed"
					}
				}
			}
		}
        stage ("Deploy") {
            steps {
                echo "This is deploy stage branch 2"
            }
        }
    }
}
