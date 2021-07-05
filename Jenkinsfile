node { 

  stage 'checkout scm'
  checkout scm

  stage 'Deploy'
  sh("ssh ubuntu@3.142.73.43 sh /home/ubuntu/deploy.sh")

}