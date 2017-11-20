@Library('pipeline-library-demo')_
def mvnHome
    // checkout scm
    // sh ("git checkout master && git pull origin master")
        // Get the maven tool.
        // ** NOTE: This 'M3' maven tool must be configured
        // **       in the global configuration
        mvnHome = tool 'M3'

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