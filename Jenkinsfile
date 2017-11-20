@Library('pipeline-library-demo')_
stage('Build') {
        if ('isUnix()') {
            sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore clean package"
        } else {
            bat "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore clean package"
        }
    }
stage('Demo') 
{  
echo 'Hello World'
sayHello 'Dave'

}