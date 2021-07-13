aws ecr get-login-password --region us-east-2 | sudo docker login --username AWS --password-stdin 693675909033.dkr.ecr.us-east-2.amazonaws.com


sudo docker build -t 693675909033.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER .


sudo docker push 693675909033.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER