<h1>End-to-End Web Application on AWS</h1>


<h2>Description</h2>
In this lab I will show you how to build an End-to-End web application from scratch, using five AWS services. <br />


<h2>AWS Applications Used</h2> 

- <b>AWS Amplify</b> 
- <b>AWS Lambda</b>
- <b>Amazon API Gateway</b> 
- <b>Amazon DynamoDB</b>
- <b>AWS Identity and Access Management (IAM)</b> 


<h2>Environments Used </h2>

- <b>AWS</b> 

<h2>Lab walk-through:</h2> 

<p align="center">
Lab 1.1 AWS Amplify <br/> 

<p align="center">
Step 1: Navigate to the "AWS Amplify" application and select "Get Started" on "Host your web app".  <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/1a878be3-cbb6-4b8e-8541-bca26a2b2146" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 2: Next you will select "Deploy without Git provider" and click "Continue".  <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/721600e8-4c38-42c0-8c45-891b3294fbe9" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Step 3: Select your App name. In this lab we will go with "PowerOfMath" for our name. Use "dev" for your Environment name and select "drag and drop" and upload your Zip file. Then select "Save and deploy".  <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/a424d500-3a68-4e20-a9c7-0c59efefc9b0" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Step 4: Now you should have a successful deployment.  <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/6bac143b-d2b7-4e59-849f-2e598089ff61" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Lab 1.2 Lambda <br/> 

<p align="center">
Step 1: Next you will navigate to "Lambda" and click "Create function".  <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/f6f09720-f939-4339-87f2-333f67499517" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Step 2: Select "Author from scratch", for your function name choose "PowerOfMathFunction", Select the latest version of python for your Runtime, Select "x86_64" for your Architecture and then click "Create function". <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/736f48b1-2bdd-4ff8-a3ef-34bb7eaf8910" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 3: You will need to write your code for the Lambda function. Use the code I wrote in the image shown. Next click "Deploy" to deploy your code. <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/77627029-d01e-4f93-8e4e-e768027b2877" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 4: Click on "Test" and select "Create new event". Use PowerOfMathTestEvent for your Event name. Select "Private", and use the code I wrote in the image. Then select "Save".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/44a0640a-5440-47d1-80a4-9ba05fe521a3" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Lab 1.3 API Gateway <br/> 

<p align="center">
Step 1: Navigate to API Gateway and click "Create API". Next you will want to select "Rest API" and click "Build".    <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/fde615e2-f1e5-44c7-a41a-2a66047f6bd4" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 2: Select "Rest" for your protocol, and choose create "New API". For your API name choose "PowerOfMathAPI" and then click "Create API".    <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/b58cee67-df9b-402f-a361-3876c7cd689a" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 3: Next you will select "Resources", click on "Actions", and choose "Create Method".    <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/06135088-e809-42cf-8181-036653b05df8" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 4: Select "Post" and for integration type select "Lambda Function". For lambda funtion you will want to type out "PowerOfMathFunction" and then click save.   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/2cdf08c5-6fc8-4023-a3bd-4a3182b5a34a" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Step 5: Make sure you have "POST" selected and on the Actions menue select "Enable CORS".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/b335fea1-2667-487b-9f21-7536d95ddbb4" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 6: Once on the "Enable CORS" tab select "Enable CORS and replace existing CORS headers".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/2c1d3556-8bc4-45d4-960f-068eb0920a2b" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 7: Next select "Actions", then "Deploy API", then choose "new stage" and use "dev" for your stage name. Then click "deploy".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/d8243b4b-e49a-42ef-a66a-ca0f5eedd276" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Lab 1.4 DynamoDB <br/>

<p align="center">
Step 1: Next you will navigate to the "DynamoDB" dashboard and select "Create table".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/84c57e62-0cdc-472d-aa3a-57cb6354b19e" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Step 2: Under table name, use "PowerOfMathDatabase". For your partition key use "ID" and leave the rest of the settings default. Then select "Create Table".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/0d3fcfd8-0f60-409b-a43c-a2a7982045f9" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 3: Next you will navigate back to your Lambda function that was created earlier and click on Configuration, then select Permissions and click on your "Role Name" link.   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/ae75f09c-3487-41ad-9c31-bc0afcf8e0b9" alt="Disk Sanitization Steps"/>
<br />  

<p align="center">
Step 4: Once on your permissions policies tab, click Add permissions and select "Create inline policy".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/1b8765a0-0ccb-4ca1-8038-1a66419b17fb" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 5: In the policy editor select "JSON" and copy the code I wrote in the policy editor. Then click "next".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/d379d60b-6a02-4c8a-9fd3-d742dcc121cf" alt="Disk Sanitization Steps"/>
<br /> 

<p align="center">
Step 6: In policy name under policy details you will want to choose "PowerOfMathDynamoPolicy" for your policy name. Then click "Create policy".   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/2afbd63d-e2d1-4005-aa76-24050386f4f4" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Lab 1.5 Update Lambda Function <br/>

<p align="center">
Step 1: Next you will want to navigate back to your Lambda Function and select "code". Then you will need to copy the new code I wrote for your Lambda Function.   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/fef959b6-05c5-45cd-bb5e-306a6283ff2b" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
Step 2: Once you have your updated code you will need to navigate to AWS Amplify and select your app that you created. Then you will choose the updated file and upload it to your application. Now you should have your updated and complete Web Application.   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/dee5cdf3-173d-4f31-95dc-122bcb2910d4" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
AWS Web Application   <br/>
<img src="https://github.com/brycehallcloud/End-to-End-Web-Application-on-AWS/assets/144934324/9a252b4a-50bf-4148-84c5-71abb4b232f4" alt="Disk Sanitization Steps"/>
<br />










