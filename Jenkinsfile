def jobs = ["JobA", "JobB", "JobC"]

pipeline {
     agent any 
     stages {
         stage('parallel stage') {
             steps {
                 script{
                    for (job in jobs){
                        stage ('complie') {
                             echo "${job} complie."
                        }
                        stage('build') {
                               echo "${job} build."
                        }
                    }                    
                 }
             }
         }
     }
 }
