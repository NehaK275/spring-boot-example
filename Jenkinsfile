pipeline{
    agent{
        label "master"
    }
   
    stages{
        stage("building"){
            steps{
                sh "mvn clean package"
            }
        }

    }
    post{
        //always{
        //    mail to: 'neha.singh@knoldus.com',
		//	subject: "Pipeline: ${currentBuild.fullDisplayName} is ${currentBuild.currentResult}",
		//	body: "${currentBuild.currentResult}: Job ${env.JOB_NAME} build ${env.BUILD_NUMBER}\n More info at: ${env.BUILD_URL}"
      //  }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
	

