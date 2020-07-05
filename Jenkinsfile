pipeline
    node{
        stage('SCM Checkout') {
             git 'https://github.com/razzpothula/game-of-life.git'
        }
        stage('Compile'){
            //Get maven home path
            def mvnhome = tool name: 'mvn', type: 'maven'       
            sh "${mvnhome}/bin/mvn compile"
        }
    }
