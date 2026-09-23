# Mission 5 Reflection

Object Storage is better suited for storing millions of photos because it is designed for large amounts of unstructured data such as images. Unlike traditional block storage, object storage organizes files as objects and can be used to store many files for applications such as photo-sharing platforms. This makes it a suitable storage option for the client's application.

Docker made it easier to deploy the MinIO storage server because I did not need to manually install and configure every part of the storage software. By using a Docker command, I was able to start MinIO and configure its ports and login credentials using environment variables. This made the deployment process faster and easier to manage.

A bucket in cloud storage is a container where objects or files are stored. In this activity, I created a bucket named `client-photos` and used it to store a sample file. The bucket helped organize the uploaded data inside the MinIO storage system.

Large enterprise companies can use different methods to help prevent object storage data from being lost when a physical server crashes. They can keep multiple copies of data, use backup systems, and store data across different servers or locations. These methods help protect important files from hardware failures.

My confidence in using the Linux command line is also improving. In this activity, I was able to use Docker commands in the terminal and check the running container. I also learned how Docker can be used together with MinIO to create a working object storage environment. Overall, this mission gave me more practical experience with cloud storage, Docker, and Linux.
