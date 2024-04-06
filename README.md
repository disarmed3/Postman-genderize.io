API testing with Postman  
2 requests:
1. GET http call to genderize.io with parameter "maria", that asserts:  
   Step 1: response of the call is code=200 or 'OK'  
   Step 2: response json values are:  
           a. name is string type  
           b. gender is string type  
           c. probability, count are number type  
   Step 3: attribute values are:  
           a. name = maria  
           b. gender = female  
2. GET http call to genderize.io with parameter "peter" and "maria", that asserts:  
   Step 1: response of the call is code=200 or 'OK'  
   Step 2: response is data type = array  
   Step 3: response of the 2 json attribute values are:  
           a. for the first array json, name = peter and gender = male  
           b. for the second array json, name = maria and gender = female   
