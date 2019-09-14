pipeline{
agent any
stages{
stage('SCM'){
steps{git 'https://github.com/pandian3k/pro02.git'}
}
stage('BUILD'){
steps{bat label: '', script: 'mvn clean'
   bat label: '', script: 'mvn install'}
}
stage('Deploy'){
steps{bat label: '', script: 'xcopy /y "C:\\Program Files (x86)\\Jenkins\\workspace\\sample_pipe\\target\\pro02.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'}
}
}
}
