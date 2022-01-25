# Getting Started
##
## Linux

### Compile, Test, Jar Code
* gradle build

### Run Jar
* Local:      gradle bootRun 
* Background: 

### Testing Application
* Abrir navegador: http://localhost:9010/rest/mscovid/test?msg=testing 

# Using Docker to test this app.
## Docker in Linux
```bash
### Compile, Test, Jar Code
docker run -it --rm -v $(pwd):/code --workdir /code gradle clean build
### test
### Run Jar
docker run -it --rm -p 8081:8081  -v $(pwd):/code --workdir /code gradle bootRun
```
