# Building a Serverless Image Rekognition Software
Services i have used:
AWS S3:

       Amazon Simple Storage Service (Amazon S3) is storage for the Internet. It is designed to make web-scale computing easier. Amazon S3 has a simple web services interface that you can use to store and retrieve any amount of data, at any time, from anywhere on the web.

IAM ROLE:

               AWS Identity and Access Management (IAM) is a web service that helps you securely control access to AWS resources. You use IAM to control who is authenticated (signed in) and authorized (has permissions) to use resources. 
               
 Amazon Rekognition: 
 
                    Amazon Rekognition makes it easy to add image and video analysis to your applications. You just provide an image or video to the Amazon Rekognition API, and the service can identify objects, people, text, scenes, and activities. It can detect any inappropriate content as well. Amazon Rekognition also provides highly accurate facial analysis, face comparison, and face search capabilities.
                    
AWS LAMBDA:

                    AWS Lambda function reads data from the stream and sends the data in real-time to an Amazon DynamoDB table to be stored. The delivery stream archives the events in an Amazon S3 bucket and sends the data to a Kinesis Data Analytics application for processing. Once the data is processed, it is sent to Kinesis Data Streams.
                    
![image](https://user-images.githubusercontent.com/90968579/231437194-d735d52a-913a-4afa-8d34-b79952789c65.png)

STEPS:

1.Create an S3 bucket. 

2.Create a Lambda Function.

3.Attach permissions policies in IAM Role:

         Grant READONLY Access to 
- AmazonS3ReadOnlyAccess , 
- AmazonRekognitionReadOnlyAccess.

4.Create IAM role.
5.Enter into the source code in lambda function.

6.First give the bucket details to the code.

7.Later give object details what we have inserted in the s3 bucket.

8.Give the required commands.

9.Click on Deploy.

10. Click on test and we get our execution results.


Output:

![image](https://user-images.githubusercontent.com/90968579/231437524-1437da00-f82d-433b-8bf3-698733faf6df.png)

![image](https://user-images.githubusercontent.com/90968579/231437583-dbca4274-e340-4754-aee8-c7e6f0ac0d5c.png)



