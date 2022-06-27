
# Set-up of local standalone instance of Apache Spark (3.1.2 version)

#### First Install Java 

Step 1: Download the Java JDK from "https://www.oracle.com/java/technologies/downloads/"

step 2: Once the download is done, Install the Java JDK.

step 3: Open the environment variable on the laptop by typing it in the windows search bar.


Now Click on Environment Variables.

![image](https://user-images.githubusercontent.com/74622153/175880519-7932ee80-10c1-43f2-88cb-5ba5e85ca53b.png)

Click on New. 

![image](https://user-images.githubusercontent.com/74622153/175908967-4199b7dd-a200-4eb7-9b00-2172cb333e9d.png)

Enter the value for 
 * Variable name - JAVA_HOME
 * Variable value - C:\Java\jdk1.8.0_331 (Path to Java File)
 * Click OK

Click on the System variable Add C:\Program Files\Java\jdk1.8.0_331\bin to PATH variable.

![image](https://user-images.githubusercontent.com/74622153/175909207-0a4b2bc0-700c-48c0-af47-71d96c301ce7.png)

Now Open command prompt and type “java –version”, it will show bellow appear & verify Java installation.

![image](https://user-images.githubusercontent.com/74622153/175884496-ce42fe71-daf0-47fa-8269-53f705a99c11.png)



### Second Install Python

1. To install the Python package manager, navigate to https://www.python.org/ in your web browser.

2. Mouse over the Download menu option and download python

3. Once the download finishes, run the file to install Python.
4. On the set-up dailog box check the option Add Python to PATH.
5. ![image](https://user-images.githubusercontent.com/74622153/175909410-89bc46fc-5e28-4cec-b53e-ef1044e8aa1c.png)
6. Click on Install Now. 



### Third Install Apache Spark (3.1.2version)

 * Naviagte to portal "https://spark.apache.org/downloads.html"
 * ![image](https://user-images.githubusercontent.com/74622153/175885202-916bcea6-ec3a-432c-a27d-c793be775c76.png)
 * Click on Spark release archives.
 * Now click on Spark-3.1.2/
 * ![image](https://user-images.githubusercontent.com/74622153/175885467-9937eb44-67c1-4d75-ab0f-1cd094bf9d06.png)
 * Download the Spark file and Install it.

Add winutils.exe File

* Download the winutils.exe file for the underlying Hadoop version for the Spark (veriosn -3.1.2)
*  Navigate to this URL https://github.com/cdarlint/winutils/blob/master/hadoop-3.1.2/bin/winutils.exe.
*  Click on Download button.
*  Now Create a New folder "Hadoop/bin" Under C drive add this "winutils.exe" file to bin folder in Hadoop.

Set environmental variables:
  * In User variable Add SPARK_HOME to PATH with value C:\spark\spark-2.4.6(path to Spark).
  * ![image](https://user-images.githubusercontent.com/74622153/175908465-05989967-d7cc-4312-ab71-698b992c1e55.png)
  
  * In System variable Add %SPARK_HOME%\bin to PATH variable.  
    ![image](https://user-images.githubusercontent.com/74622153/175908536-222db8c8-39b2-4759-883d-ea472857ea36.png)

  * For Hadoop In User variable Add HADOOP_HOME to PATH with value C:\hadoop(path to Hadoop).
  * In System variable Add %HADOOP_HOME%\bin to PATH variable.
  
launch Spark

* Open Command Prompt 
* Type "spark-shell"
* The system should display several lines indicating the status of the application. You may get a Java pop-up. Select Allow access to continue.
Finally, the Spark logo appears, and the prompt displays the Scala shell.
* ![image](https://user-images.githubusercontent.com/74622153/175906058-c2f3e543-774d-46a9-a1a1-bacaa9df143e.png)

#### To write PySpark program
    
   Install pyspark which is compatible with Spark verwsion-3.1.2
    
    * pip install pyspark==3.1.2
    
### Done setting up the local standalone instance of Apache Spark (3.1.2version) on your laptop/desktop system


