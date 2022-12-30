pipeline
{

agent any
stages {
stage('Compile') {
steps{
sh 'mvn clean compile'
}
}
stage('UnitTest') {
steps{
sh 'mvn clean test'
}
}
stage('QA') {
steps{
sh 'mvn pmd:pmd'
}
}
stage('Package') {
steps{
sh 'mvn package'
}
}
}
}
