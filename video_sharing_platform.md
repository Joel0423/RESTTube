Real World Application - Video sharing platform
Video sharing platforms like YouTube can be developed with a microservice architecture.

Microservices-
1. User Management
A Microservice to handle user login and registration
Scalability: There can be a huge number of people trying to login or register. The traffic can spike at certain times so scalability is important
Flexibility: You can manage user profile features without touching unrelated services.
Independent Deployment: Security patches or new login features can be deployed quickly to the user management service alone reducing risk

2. Video Storage and Delivery
A microservice that handles uploading videos to be stored in a database and then retrieving it when a user wants to play it.
Scalability: Video uploads and streaming are resource-intensive and require large amounts of storage and bandwidth. So scalability is important. Also by keeping it as a microservice we can scale it effectively without needing to scaling other microservices that are less resource intensive. 
Independent Deployment: Even if a microservice like user comments are not available the videos can still be played

3. User Comments
A microservice to handle user comments on videos.
Scalability: Comment activity can be varied and can spike on any number of videos on the platform, whereas some videos would have minimal comment activity. So scalability is important here.
Flexibility: You can add features like threaded replies or spam filtering to comments without interfering with the video or user management services.