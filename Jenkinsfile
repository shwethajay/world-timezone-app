pipeline{

agent any

stages{

stage('Build Application'){

steps{


bat 'mvn clean install'

}

}

stage('Deploy Application'){



steps{

bat 'mvn package deploy -DmuleDeploy'
}

}

stage('Perform regression testing'){
steps{
bat 'C:\\Users\\Skanda\\AppData\\Roaming\\npm\\newman run D:\\Worldtimezone.postman_collection.json --disable-unicode'
}

}


}

}