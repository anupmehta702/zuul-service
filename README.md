
Steps to run -
1) Run student app first on port 8085
mvn spring-boot:run -Dspring-boot.run.arguments=--server.port=8085
mvn spring-boot:run -Dspring-boot.run.arguments=--studentPort=8081

2) Run zuul app on port 8081
mvn spring-boot:run -Dspring-boot.run.arguments=--zuulPort=8081

3) Hit zuul api
http://localhost:8081/student/echoStudentName/Anup
it redirects to localhost:8085
