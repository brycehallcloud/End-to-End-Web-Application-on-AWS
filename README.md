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





