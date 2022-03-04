pipeline {
			agent none
			stages {
				  stage('Build') {
				         agent { label 'node1' }
  	                                         steps {
                                          		sh 'sleep 15; echo "This is a Build stage"'			
					                 }
				                 }

				  stage('Test'){
                                           agent { label 'node2' }
				 	          steps {
					
                                                 sh '''
							sleep 15
							echo "This is a Test stage"
                                    		    '''
					                }
				               }

				  stage('Deploy'){
                                             agent { label 'node1' }
					          steps {
               					        sh 'sleep 15; echo "This is a deploy stage"'
 
					                }
				                 }

				  stage('My-stage'){
					           agent { label 'master' }
                                                  steps {
					              sh '''
                                                           sleep 15
                                                            echo "This is a master stage"
                                                          '''					                }
				                   }	
			        }
		}
