
# Traffic-Generator-OSCARS


----
**About Traffic Generator**

  A Simulator to generate traffic for Controller OSCARS to test and analyze the reservation possibilities for different types of traffics. More on OSCARS can be found [here](https://github.com/NetLab/oscars-newtech/%22here%22). This is a maven project built to run parallely with OSCARS only for research purposes (Not a software testing tool). 
  
**Setting up the Environment**
  Installation requirements
 1. [Java](https://www.java.com/en/%22Java%22) 1.8   
 2. [Maven](http://maven.apache.org/%22Maven%22) 3.1+

**Building the project**
Run the following commands in the project directory

     mvn -f package

If you want to skip tests

    mvn -f -DskipTests package
    
To start generating traffic (Make sure the OSCARS is started)
	   

    mvn -f ./oscar-trafficgenerator exec:java -Dexec.mainClass="com.acnl.oscartrafficgenerator.MainApp" -Dexec.args="$seed $totalrequest PALINDROME $numPaths $minnumflows $maxnumflows $arrival $holding $deviceproperties $bandwidth $bandwidthdeviation $failure oscarTrafficController NONE"

 A sample script **"script.sh"** file is uploaded with the project for reference.
 (Modify the script according to your requirements)
 
 To run the script,
  
   `./script.sh`
   
**More on Project Structure**

  Read the files in the **"doc"** folder for the architecture and project structure.





































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































































