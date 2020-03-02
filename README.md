## run on your local mach
	
	$ mvn clean package exec:java

## run on docker
	docker-compose up -d
	
## create new person
curl -H "Content-Type: application/json" -X POST -d "{\"first\": \"DevOps\",\"last\": \"KOÇ\",\"dateofbirth\": 381110400000,\"placeofbirth\": \"India\"}" "http://192.168.99.100:8080/people"

## list existing people in the database
curl -H "Content-Type: application/json" -X GET "http://192.168.99.100:8080/people"
