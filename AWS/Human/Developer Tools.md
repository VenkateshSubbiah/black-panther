## AWS X-Ray

Traces the requests of the application and the AWS services the app uses.
The client SDK sends segments of data as JSON to the X-Ray daemon listening to the UDP port. It is then sent in batches to the X-Ray.
https://docs.aws.amazon.com/xray/latest/devguide/aws-xray.html