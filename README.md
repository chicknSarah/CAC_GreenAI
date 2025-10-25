# CAC_GreenAI
CI forecasting, Alexa Skill. learning AppScript, Thunkable, submission for CAC!

This project uses Thunkable to create the UI of the app, and most of the coding is done on CoLab with python. Updating the CI forecast, using the Appliance recognizer, and data analysis were all done on CoLab. To communicate the inputs and outputs between Thunkable and CoLab, I used google sheets and Apps Script where needed to trigger certain functions.

So, the majority of the main project of GreenAI is in CoLab and Thunkable linked below:
https://x.thunkable.com/projectPage/672a4a2a6b13027e12120aa3
test out the app via the link. Click "See Inside" to view code.

The CoLab code used to update each region's past 24 hr of data, the next 24 hr forecast, the forecast lowest 4 CI hours, and the forecast average CI (the estimated CO2 saved is calculated on Thunkable):
https://colab.research.google.com/drive/1Hynh295SLFe9JAHiEoZXb6UXSMGFaB0a?usp=sharing

The other part of project GreenAI is an Alexa skill. It is built from the same data the app is built on. I made a prototype of the backend: Apps Script will communicate the data from the sheets to AWS S3 buckets with the help of an [S3 library](https://script.google.com/macros/library/d/1Qx-smYQLJ2B6ae7Pncbf_8QdFaNm0f-br4pbDg0DXsJ9mZJPdFcIEkw_/4?authuser=0).
Test and view: https://docs.google.com/spreadsheets/d/1SXpZWRT_GbjIOEhFvIHfY2OHF9m5AGHQBSIzs_iNnC0/edit?usp=sharing
make a copy of the sheets, then you can access the Apps Script code. Replace: "accessKeyId" and "secretAccessKey" with the keys found in your AWS profile representing your S3 buckets.
