node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/bapushembade/hello-world-war.git']]])
    }
    stage('build'){
        sh 'mvn clean package'
    }
}
