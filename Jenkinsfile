@Library('mylibrary')_
pipeline
{
    agent any
    stages
    {
        stage("Continuous Download_Master")
        {
            steps
            {
                script
                {
                    cicd.newGit('https://github.com/yallamanda/multibranch.git' )


                }

            }
        }

        stage("Continuous Build_Master")
        {
            steps
            {
                script
                {
                    sh 'mvn package'


                }

            }
        }

        stage("Continuous Deploy_Master")
        {
            steps
            {
                script
                {
                   cicd.newDeploy("lib-4","172.31.85.85","testapp")


                }

            }
        }


    }




}
