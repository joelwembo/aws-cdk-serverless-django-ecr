# Sample for a Django Serverless CDK Application using AWS managed services

The purpose of this sample is to demo a serverless CDK stack for a Python [django](https://www.djangoproject.com/) Application that uses Amazon ECS with AWS Fargate, AWS Lambda, Amazon Aurora MySQL-Compatible Edition, Elastic Load Balancing (ELB) and Amazon CloudFront. 

The sample also uses RDS IAM Authentication for the django Backend to avoid hard-coded credentials in the settings file. The user setup is covered by a Lambda custom resource triggered on creation or changes of the database.

Another part of this sample is to use Cloudfront to distribute the traffic to the ELB (Dynamic Django content) and Amazon S3 (django static files) as well as configuring the Django Application to update the static content and database on new deployments.


## License

This library is licensed under the MIT-0 License. See the LICENSE file.
