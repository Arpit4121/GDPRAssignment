This file will brief you about the solutions and the things needed to test those on your local machine.

Project  Arpit_dotnet:
This project is a .Net Core Web API project which basically consists of 2 APIs i.e. CreateUser (which will be used for creating a user) and GetAllUsers (which will be used for fetching a list of all users).
Before running the web api project locally, add your MongoDB connection string in the placeholder inside MongoDbContext.cs file.
Once you run this project, you should be able to see the swagger doc.

Project Angular App_Arpit:
This is the angular app project which will basically deal with the UI.
Once you build and run this locally, you should be able to see a basic UI where you will have the option to Add a user and a table which will show the number of users present in the DB.
Before running the project, make sure you replace the actually API url in the user.service.ts file in the field 'apriUrl' so that your angular app calls the Web APIs.

GDPR methods used:
 Has Consent field in the User Model - If the user will not check this field before creating a user, it will not save the user info in the DB. However, if the user checks this check box before creating a user, the 
 user info will be stored in the DB meaning the user gave consent to store his/her info in the DB as per the GDPR guidelines.
Encryption - Before saving the Email and Address of the user, those fields are being encrypted and then saved in the DB as per the GDPR guidelines.

Project Console Application:
This solution contains the function 'IsGoodBinaryString' which states whether a binary string follows the 2 practices of a good binary string or not.
For testing this, just run this locally and you will see the output in the console.
