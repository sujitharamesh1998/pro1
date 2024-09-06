node{
stage
  {
   git url: "https://github.com/sujitharamesh1998/pro1"
   sh 'mvn clean package"
  }
stage("docker build")
  {
   sh "docker build -t project1 ."
  }
}


