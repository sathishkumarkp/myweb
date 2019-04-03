  node{
   stage('SCM Checkout'){
     git 'https://github.com/sathishkumarkp/myweb'
   }
   stage('Maven-Test'){
    
      def mvnHome =  tool name: 'MAVEN3', type: 'maven'   
      sh "${mvnHome}/bin/mvn test"
   }
    stage('Maven-Compile-Package'){
    
      def mvnHome =  tool name: 'MAVEN3', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
   }
   
}


