pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
               withAWS(region:'us-east-2', credentials:'aws-static') {
                    s3Upload( file:'index.html', bucket:'static-udacity12221', path:'index.html')
                }
             }
         }
     }
}
