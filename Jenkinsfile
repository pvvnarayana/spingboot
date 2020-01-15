node{
    stage('SCM Checkout'){
        git url:'https://github.com/pvvnarayana/spingboot.git'
    }
    stage('Mvn Package'){
        def mvnHome = tool name: 'maven', type: 'maven'
        def mvnCMD = "${mvnHome}/bin/mvn"
        sh "${mvnCMD} clean package"
    }
}
