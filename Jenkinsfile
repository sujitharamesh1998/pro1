node{
    stage (" git checkout"){
        echo "git checkout started"
        git url: "https://github.com/sujitharamesh1998/pro1"
        echo "checkout is done"
       }
    stage (" build "){
        echo "maven build started"
        sh "mvn clean package"
        echo " maven build is completed" 
       }
    stage (" create image"){
        echo " docker image is creating"
        sh " docker build -t project ."
        echo " image is created"  
       }
}
