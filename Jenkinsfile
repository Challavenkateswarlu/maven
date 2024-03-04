pipeline
	{
	agent any
		stages
			{
			stage("GIT")
				{
				steps
					{
					git "https://github.com/Challavenkateswarlu/maven.git"
					}
				}
			stage("Run")
				{
				steps
					{
					sh "java Demo.java"
					}
				}
			}
	}
