node{
stage
  {
   echo "git checkout started"
   git url: "https://github.com/sujitharamesh1998/pro1"
   echo "checkout is done"
stage{
   echo "clean package is started"
   sh 'mvn clean package'
   echo "clean package is completed"
  }
stage("docker build")
  {
   echo "docker build is started"
   sh "docker build -t project1 ."
   echo " docker build is comleted image is created"
  }
stage
  {
   echo " docker login collecting details"
   withCredentials([string(credentialsId: 'dockerhubpass', variable: 'dockerhub')]) {
   sh " docker login -u sujitha202301 -p ${dockerhub} "
  }
  }
}    


