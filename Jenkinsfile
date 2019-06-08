pipeline {
agent any
stages("one"){
steps{
Echo"Hello from jenkins"
}
}
stages("Two"){
Steps{
input("Do you want to proceed?")
}
}
Stages("Three"){
Steps{
when{
no{
branch"master"
}
}
Step {
Echo"Hello"
}
}
Stages("Four"){
parallel{
stages("Unit Test")
Step{
Echo "Unit Test is in porogress")
}
}
Stages("Intgration Test"){
agent{
docker{
rusenode false
image "ubuntu"
}
}
Steps{
echo "Integration test is in progress"
}
}
}
}
}
}
}

