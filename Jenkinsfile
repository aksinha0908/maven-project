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
            sh 'mvn -B -DskipTests clean package'
    }
    stage('Test')
    {
        echo 'Code Test'
    }
    stage('Deploy')
    {
        echo 'Deploy'
    }
}
