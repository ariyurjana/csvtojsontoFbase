# csvtojsontoFbase
convert csv to json and store to Firebase
I have a dataset in the form of CSV and want to store it in Firebase database. Read the Firebase data and populate into the dropdown of a spinner
I take the CSV file and convert it using an online service to a JSON file.
Over to Android,create a project with blank activity
Add GSON dependency to the project
create a POJO class containing one integer and another string for storing code and description. Autogenerate the constructor, setter and getters.
In activity_main.xml drag a spinner into the layout
Create another resource file called ddvw_row.xml. In this drag a Linear Layout with horizontal orientation.
Drag two textview's into this linear layout.
Create an Assets folder and drag and drop the json file created in step 4.
Create a FBaseHelper.java class
Use the json file in the assets folder and read its contents into a string variable.
Using fromJson method passing the string from step 13 populate the POJO class
Add this POJO class to the ArrayList
I am having trouble with step 14, fromJson is only populating null into the member variables of the POJO class
