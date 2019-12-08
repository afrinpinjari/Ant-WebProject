

pipeline
{
	agent any
	stages
	{
		stage ('git clone')
		{
			steps
			{
				git 'https://github.com/afrinpinjari/Ant-WebProject.git'
			}
		}
		
    stage ('test my project')
		{
			steps
			{
				withAnt(installation: 'localAnt', jdk: 'localJDK') {
    sh 'ant build'}

    
			}
		}
	}	
	}
