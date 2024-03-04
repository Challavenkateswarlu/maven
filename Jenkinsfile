pipeline
	{
	agent any
		stages
			{
			stage("GIT")
				{
				steps
					{
					git ""
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
