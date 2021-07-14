//echo "this is for all Env"
node {
        def GradleHome = tool name: 'Gradle', type: 'gradle'
    def gradle = "${GradleHome}/bin/gradle"
        def mavenHome = tool name: 'maven', type: 'maven'
    def maven = "${mavenHome}/bin/mavan"
        stage('checkout') {
git branch: 'main', credentialsId: 'git-creds', url: 'https://github.com/suresha10/newclass.git'
            }
        stage('build'){
            sh "${gradle} clean deploy "    
        }
        
}

        

