node {
   def mvnHome
    // checkout scm
    // sh ("git checkout master && git pull origin master")

    stage ('start') {
        // Get the maven tool.
        // ** NOTE: This 'M3' maven tool must be configured
        // **       in the global configuration
        mvnHome = tool 'M3'
    }
    stage ('Build') {
        if ('isUnix()') {
            sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore compile"
        } else {
            bat "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore compile"
        }
    }
    
stage('Demo') 
{  
echo 'Hello World'
sayHello 'Dave'
}
}