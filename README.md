# executable-jar
### Step to make executable Jar (like shell)
1. make jar
      - `javac Hello.java -d classes`
      - `jar -c -v -f myjar.original.jar -e Hello -C classes .`
2. append `myjar.original.jar` to `run.sh`
      -  `cat run.sh myjar.original.jar > myjar.jar`
      - `chmod +x myjar.jar`

### Test
` ./myjar ` It should prinnt `Hello World'
