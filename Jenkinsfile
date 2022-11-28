@Library('mylibrary')_
pipeline
{
    agent any
    stages
    {
        stage("Continuous Download_Dev")
        {
            steps
            {
                script
                {
                    cicd.newGit('https://github.com/yallamanda/28-Multi.git' )


                }

            }
        }

        stage("Continuous Build_Dev")
        {
            steps
            {
                script
                {
                    sh 'mvn package'


                }

            }
        }

        


    }




}

