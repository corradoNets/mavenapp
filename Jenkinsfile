pipeline 
{
    agent 
    {
        docker 
        {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages 
    {
        stage('Build') 
        {
            steps 
            {
                sh 'mvn -B -DskipTests clean package'
            }
           steps 
           {
            script 
               {
                openshift.withCluster() 
                   {
                    openshift.newBuild("--name=mapit", "--image-stream=redhat-openjdk18-openshift:1.1", "--binary")
                    } 
               }
           }
        }       
    }
}
