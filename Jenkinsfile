pipeline{
		agent{

			label{
				label "built-in"
				customWorkspace "/mnt/test"

			}
		}

		stages{

			stage ('stage-1')  {


				steps{
					echo "Hello velocity"

				}
			}
			stage ('stage-2')  {

				steps{

					sh "yum install httpd -y"
					sh "service httpd start"
					sh "cp index.html /var/www/html/"
					sh "chmod -R 777 /var/www/html/index.html"
				}
			}
			
		}

}
