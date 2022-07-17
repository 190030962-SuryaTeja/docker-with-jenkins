pipeline
{
	agent any

	stages
	{
		stage('Pre Test')
		{
			steps
			{
				sh 'cd mavendemo'
				sh 'pwd'
				sh 'ls'
			}
		}
		
		
		stage('Pre Clean')
		{
			steps
			{
				sh 'mvn clean install -DskipTests'
				sh 'echo cleaning done'
			}
		}
		
		stage('Test')
		{
			steps
			{
				sh 'javac App.java'
				sh 'java App'
			}
		}
	}
}
