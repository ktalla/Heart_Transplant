## GOAL
Write a HeartTransplant class that has the ability to select the patient, from a pool of patients, with the highest potential to survive the longest after the heart transplant surgery. Used the HeartTransplantDriver to test the methods within the HeartTransplant class.



## FILES

**HeartTransplantDriver.java** <br>
  This is the program you should compile and run. It builds a HeartTransplant object and calls instance methods on it. No need to make changes to it, but you are welcome to change it if you want. It is for testing purposes only. <br>
**SurvivabilityByAge.java**<br>
  Stores information about the survivability of patients, by age, after n years post heart transplant surgery.<br>
**SurvivabilityByCause.java**<br>
  Stores information about the survivability of patients, by heart condition cause, after n years post heart transplant surgery.<br>
**Patient.java**<br>
  Stores patient information. Contain constants representing patient codes (health condition code, gender code, urgency code, ethnicity code…)<br>
**Data.txt**<br>
  Contains patient information, as well as survivability by age and cause rates. This file should be piped when executing HeartTransplantDriver  <br>
  How to run the driver: <br>
  **Compile:** javac HeartTransplantDriver.java <br>
  **Execute:** java HeartTransplantDriver < data.txt <br>
**HeartTransplant.java**<br>
  This is the file you will write your code on. Provided as an empty file, complete it based on documentation. <br>
  
  # Data File Format <br>

The data file is divided in three sections. The first section is the person section, the second the rates of survivability by age section, and the third is the rates of survivability by heart condition cause section. <br><br>

**First section: person **<br><br>

The first line of this section has an integer that refers to the number of persons in the file. The file has one person per line in the following format:<br>
PersonID Ethinicity Gender Age Cause Urgency StateOfHealth <br><br>
 
The example below has 3 persons, the first person’s ID  4101, Ethnicity 10, Gender 13, Age 75, Cause 3, Urgency 8, and StateOfHealth 7. You can see the meaning of each code in the Person.java file. <br>

**Second section: survivability by age** <br><br>

The first line of this section has an integer that refers to the number of survivability by age rates in the file. The file has one rate per line in the following format:<br>
Age YearsPostTransplant Rate<br><br>
 
The example below has 8 rates, the first rate specifies that people with age LESS than 1 year old, 5 years post transplant have a survivability rate of 83.6%.
**Third section: survivability by heart condition cause**<br><br>

The first line of this section has an integer that refers to the number of survivability by cause rates in the file. The file has one rate per line in the following format:<br>
Cause YearsPostTransplant Rate<br><br>
 
The example below has 5 rates, the first rate specifies that people with heart condition cause 4 (heart muscle disease), 1 year post transplant have a survivability rate of 89.4%.You can see the meaning of each code in the Person.java file. <br><br>

**Example**
3
4101  10  13  75  3  8  7
4102  11  14  78  4  9  5
4103  12  14  40  3  8  5
8
 1  5 83.6
 6  5 87.4
 11 5 86.8
 18 5 90
 35 5 86.9
 50 5 88.8
 65 5 87.8
120 5 84.3
5
4 1 89.4
1 1 82.1
3 1 87.1
0 1 88.2
2 1 88.2


