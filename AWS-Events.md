# AWS: Events

## AWS S3

1. What is Amazon S3?
 is an object storage service offering industry-leading scalability, data availability, security, and performance.

2. Name some use cases for Amazon S3.

- Build a data lake
- Back up and restore critical data
- Archive data at the lowest cost
- Run cloud-native applications

3. Name some benefits of using Amazon S3.

- Scale storage resources to meet fluctuating needs with 99.999999999% (11 9s) of data durability.
- Store data across Amazon S3 storage classes to reduce costs without upfront investment or hardware refresh cycles.
- Protect your data with unmatched security, compliance, and audit capabilities.
- Easily manage data at any scale with robust access controls, flexible replication tools, and
organization-wide visibility.

## AWS Lambda Basics

1. What is AWS Lambda?
AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner.
2. Name some use cases for AWS Lambdas.
Data processing,Scalable APIs.The Lambda functions can perform any kind of computing task, from serving web pages and processing streams of data to calling APIs and integrating with other AWS services.

3. Describe “serverless” to a non-technical friend.
The concept of “serverless” computing refers to not needing to maintain your own servers to run these functions.

## CDN

1. What is a CDN?

A Content Delivery Network (CDN) is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos.

2. How does a CDN work with relation to the website visitor?

CDNs work through servers nearest to the website visitor respond to the request. The content delivery network copies the pages of a website to a network of servers that are spread out at geographically different locations, caching the contents of the page. When a user requests a webpage that is part of a content delivery network, the CDN will redirect the request from the originating site’s server to a server in the CDN that is closest to the user and deliver the cached content. CDNs will also communicate with the originating server to deliver any content that has not been previously cached.

3. What are the benefits of employing a CDN?
it helps protect your website against certain forms of cyber attacks, such as Denial of Service attacks. It protects against these threats because CDNs allow for the handling of more traffic and withstanding hardware failure better than many origin servers. 