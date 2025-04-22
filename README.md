For API testing, I use Postman, which is an API testing tool.

Environment Setup for API testing:

a. At first, I use the below command from VS code editor to run the "inde.js" file by entering the mockedAPI folder 
  
  cd .\mockedAPI\
  
  node index.js

Then I got the 

[Application listening on PORT 9999]

b. Secondly, I moved the storage folder, which contains the  "account.json" file, under the mockedAPI folder

c. Thirdly, I open POSTMAN -> create collection [QA Quiz Challenge-API Test Script] -> create API requests [GET, POST, PUT, DELETE] with body & scripts 

d. To create the body in case of "POST" request in POSTMAN, I followed the  script line below from "index.js" of the mockedAPI folder: 

   const {username, name, password, favouriteFruit, favouriteMovie, favouriteNumber} = req.body;
  
e. To create the body in case of "Put" request in POSTMAN, I used the  script line below from "index.js" of the mockedAPI folder: 

   const {name, password, favouriteFruit, favouriteMovie, favouriteNumber} = req.body;

f. To create scripts in POSTMAN, I go to scripts -> post-response -> </> snippets 

f. Finally, save all the API requests in the collection [QA Quiz Challenge-API Test Script] & run
