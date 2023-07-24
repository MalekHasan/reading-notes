# AWS: Events
## AWS SQS vs SNS

1. What is the difference betweeen SQS and SNS?

SNS is a distributed publish-subscribe service.
SQS is distributed queuing service.

2. What are some use cases for both SNS and SQS?
Choose SNS if:

You would like to be able to publish and consume batches of messages.
You would like to allow same message to be processed in multiple ways.
Multiple subscribers are needed.
Choose SQS if:

You need a simple queue with no particular additional requirements.
Decoupling two applications and allowing parallel asynchronous processing.
Only one subscriber is needed.

## AWS SNS and SQS

1. Describe how to use SQS and SNS in a “fanout” pattern.

The "fanout" pattern using Amazon SQS and SNS involves setting up an SNS topic as a central point for message distribution. Multiple SQS queues subscribe to this topic. When a message is published to the SNS topic, it automatically fans out to all subscribed SQS queues. Each SQS queue represents a separate consumer that processes the messages independently and asynchronously. This pattern enables decoupling between publishers and subscribers, allowing easy scaling and fault tolerance. SQS ensures message durability, and subscribers can process messages at their own pace. With this pattern, you can implement event-driven architectures efficiently, achieving high scalability and flexibility in distributed systems.

2. Explain how “push notifications” work, using SNS.
Push notifications are messages sent from a server or backend system to a mobile device or application without the mobile device explicitly requesting the information. They are commonly used to deliver real-time updates, alerts, or messages to users on their devices, even when the app is not actively running. Amazon SNS (Simple Notification Service) is a fully managed service that facilitates sending push notifications to mobile devices and other endpoints.

Here's how push notifications work using Amazon SNS:

- Registration: The mobile app needs to register with the appropriate push notification service for the specific platform it's running on (e.g., Apple Push Notification Service - APNs for iOS devices, Firebase Cloud Messaging - FCM for Android devices). During this registration process, the app receives a unique device token from the push notification service.

- Integration with Amazon SNS: Once the mobile app has obtained the device token, it sends this token to the backend server. The backend server then integrates with Amazon SNS and creates a platform endpoint, associating the device token with a specific user or app.

- Topic Creation: In Amazon SNS, a topic is created to group similar endpoints together. For example, you might have a topic for sending notifications related to breaking news, another topic for updates on user activities, etc.

- Subscriptions: Mobile app endpoints (identified by their device tokens) subscribe to the relevant topics they are interested in. This subscription is done through the backend server using the Amazon SNS API.

- Message Publishing: When there's new information or an event to notify users about, the backend server publishes a message to the appropriate topic in Amazon SNS.

- Fanout to Subscribers: Amazon SNS takes care of the fanout process, sending the message to all the subscribed endpoints (i.e., the mobile devices associated with the device tokens subscribed to the topic).

- Notification on Devices: Upon receiving the push notification from Amazon SNS, the push notification service for the respective platform (e.g., APNs for iOS or FCM for Android) delivers the message to the target mobile device.

- Display on Mobile Device: The mobile device's operating system handles the push notification and displays it to the user as a banner, alert, or in the notification center, depending on the device's settings and user preferences.

## SQS and SNS Basics

1. How might a large scale, distributed application make use of a Queue system like SQS?

In a large-scale, distributed application, Amazon SQS is utilized for load leveling, asynchronous processing, and scalability. It decouples components, preventing bottlenecks, and improves performance. Asynchronous processing offloads time-consuming tasks to SQS, ensuring responsiveness. Scaling consumers handles increased message processing, while SQS provides fault tolerance by persisting messages. In microservices architectures, SQS facilitates communication between services. Cross-region communication is enabled, connecting regions in multi-region setups. SQS allows for delayed and scheduled tasks, supporting task execution at specified times. It enhances reliability, ensures high availability, and enables seamless coordination across the distributed infrastructure.