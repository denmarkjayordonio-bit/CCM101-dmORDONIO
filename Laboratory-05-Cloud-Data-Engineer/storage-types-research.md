# Cloud Storage Types

Cloud storage can be used in different ways depending on the type of data and how it needs to be accessed. The three common types are Block Storage, File Storage, and Object Storage.

| Storage Type | Description | Common Use | Example |
|---|---|---|---|
| Block Storage | Stores data in blocks and works similar to a disk connected to a server. | Operating systems, databases, and applications | AWS EBS |
| File Storage | Organizes data into files and folders that can be shared. | Shared files and folders | AWS EFS |
| Object Storage | Stores files as objects together with metadata. | Photos, videos, backups, and documents | Amazon S3 |

## Best Storage for the Client

For the client's photo-sharing application, I would choose **Object Storage**. Photos are considered unstructured data, and object storage is designed to handle this type of information.

It is also a good choice because the application may eventually contain a large number of uploaded photos. Using buckets makes it easier to organize and manage these files as the amount of stored data grows.
