# **CountryApp**

### **Asp.Net Core 7 (.NET 7) | True Ultimate Guide**

<br>

Requirement: Create an Asp.Net Core Web Application that serves country details based on the request path.

<br>

### **Consider the following hard-coded list of countries:**

1, United States

2, Canada

3, United Kingdom

4, India

5, Japan

You can store these countries directly as a dictionary.

<br>

### **Example #1:**

If you receive a HTTP GET request at path "/countries", it has to return the list of available countries.

Request Url: /countries

Request Method: GET

Response Status Code: 200

Response body (output):

1, United States

2, Canada

3, United Kingdom

4, India

5, Japan

![2022-10-26_19-50-59-77393b36c5a638a9f8d3c4d4508af9c0](https://user-images.githubusercontent.com/60389872/203924538-22c7e159-4334-4781-a4bc-a2386bb1120d.png)

<br>

### **Example #2:**

If you receive a HTTP GET request at path "/countries/{countryID}", it has to return the corresponding country name.

Request Url: /countries/1

Request Method: GET

Response Status Code: 200

Response body (output):

United States

![2022-10-26_19-50-59-110a382ed3fb1fd249df0dc96f145ac1](https://user-images.githubusercontent.com/60389872/203924360-e619ddfd-a515-46d7-bbbb-a43e844a039e.png)

<br>

### **Example #3:**

If you receive a HTTP GET request at path "/countries/{countryID}", if the countryID doesn't exist (that is - outside the range of 1 to 5), it should return HTTP 404 response.

Request Url: /countries/6

Request Method: GET

Response Status Code: 404

Response body (output):

[No Country]

<br>

### **Example #3:**

If you receive a HTTP GET request at path "/countries/{countryID}", if the countryID is greater than 100, it should return HTTP 404 response.

Request Url: /countries/101

Request Method: GET

Response Status Code: 400

Response body (output):

The CountryID should be between 1 and 100

<br>

### **Route Constraints:**

The "countryID" parameter should be an int value.

The value of "countryID" parameter should be between 1 and 100.

<br>

### **Instructions:**

- Create routes with UseEndPoints() middleware.

- Use essential route parameters and route constraints.

- Use parameter validation when necessary.

- Use Map(), MapGet() or MapPost() methods to create endpoints, according to the requirement.

- Return the response with appropriate response status code based on above examples.

