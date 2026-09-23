# Types of Cloud Storage

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be accessed by a system as disk storage. | Virtual machines, databases, and applications that need disk-like storage. | AWS EBS |
| File Storage | Stores data as files and folders that can be shared and accessed through a file system. | Shared files, documents, and applications that need shared storage. | AWS EFS |
| Object Storage | Stores data as objects together with metadata inside a storage system. | Images, videos, backups, and other large amounts of unstructured data. | AWS S3 |

## Why Object Storage is Suitable for the Client

Object Storage is a suitable choice for the client's photo-sharing application because it is designed for storing large amounts of unstructured data such as images. It also allows uploaded files to be stored separately from the web server, which is useful when the application needs to handle millions of photos.
