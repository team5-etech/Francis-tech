pipeline{
	    agent any
	    stages{
	         stage('1-cloning'){
                 checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-id', url: 'https://github.com/team5-etech/Francis-tech.git']])
                 
                 }

             }
             stage('2-saada1-contribution'){
             steps{
                 sh 'lscpu'
                 sh 'sudo systemctl status jenkins

                 }

              }
              stage('3-Nellyblues-contribution'){
                 steps{
                     sh 'lscpu'
                     sh 'sudo systemctl status jenkins'

                 }
             }
             stage('4-Fancis-contribution'{
                 steps{
                     sh 'df -h'
                     sh 'sudo systemctl status jenkins'

                 }
             }

          }

       }
