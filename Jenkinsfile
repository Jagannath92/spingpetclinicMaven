node {
parameters {
        booleanParam(defaultValue: true, description: '', name: 'userFlag')
    }

   stage('SCM') {
      // git clone
	  git 'https://github.com/Neelimapayasamgit/spingpetclinicMaven.git'
   }
   
   stage ('build the packages') {
      // mvn package
//	  sh 'mvn package'
echo "entered build and package uild"
   }

   
   
   stage ('archival') {
     // archiving artifacts
//	 archive 'target/*.jar'
echo "entered archive stage"

   }
stage ('paracheck') {
 echo "entered param section"
steps {
                echo "flag: ${params.userFlag}"
            }
}
}
