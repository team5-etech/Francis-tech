pipeline{
	agent any
	stages{
	    stage('1-clone'){
	        steps{
	           checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-id', url: 'https://github.com/team5-etech/Francis-tech.git']])
	         }

	    }
	    stage('2-systemcheck'){
	        steps{
	            sh 'sudo systemctl status jenlins'
	        }
	    }
	    stage('3-diskcheck'){
	        steps{
	            sh 'df -h'
	        }
	    }
	    stage('4-blockcheck'){
	        steps{
	            sh 'lsblk'
	        }
	    }
        stage('5-ops-check'){
            steps{
                sh 'cat /etc/os-release'
            }
        }
        stage('6-scriptcontrol'){
            steps{
                sh 'bash -x /var/lib/jenkins/workspace/Francis-demo/script.sh'

                }

            }
         
        }
               
    }           


      
    
	  
 
