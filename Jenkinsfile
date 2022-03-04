pipeline {
  
                        agent { label 'pipe1' }
   
                           stages {

				  stage('Build') {
  	                                         steps {
                                          		sh 'sleep 15; echo "This is a Build stage"'			
					                 }
				                 }

				  stage('Test'){
				 	          steps {
					
                                                 sh '''
							sleep 15
							echo "This is a Test stage"
                                    		    '''
					                }
				               }

				  stage('Deploy'){
					          steps {
               					        sh 'sleep 15; echo "This is a deploy stage"'
 
					                }
				                 }

				  stage('My-stage'){
                                                  steps {
					              sh '''
                                                           sleep 15
                                                            echo "This is a My-stage"
                                                          '''					                
                                                        }		
		                                   }	
			        }
		}
