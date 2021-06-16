node ('slave-10.1.110.52')
    {
         env.PATH = "/opt/maven3/bin/:$PATH"
    stage('Hello')
    {
        echo 'Hello World'
    }
    stage('Code sync') 
    {
        git branch: 'master', url: 'https://github.com/aksinha0908/maven-project.git'
    }
    stage('Build')
    {
            sh 'mvn clean'
            sh 'mvn package'
    }
    stage('Test')
    {
        mvn 'test'
    }
    stage('Deploy')
    {
        echo 'Deploy'
    }
}
