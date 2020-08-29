# executable-jar
### Step to make executable Jar (like shell)
1. make jar
  1. `javac Hello.java -d classes`
  2. `jar -c -v -f myjar.original.jar -e Hello -C classes .`
2. append `myjar.original.jar` to `run.sh`
  1.  `cat run.sh myjar.original.jar > myjar.jar`
  2. `chmod +x myjar.jar`
