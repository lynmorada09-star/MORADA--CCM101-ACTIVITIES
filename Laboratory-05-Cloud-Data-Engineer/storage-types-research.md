
# Research: Cloud Storage Types

## Comparison Table

| Storage Type | Description (How it stores data) | Primary Use Case | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splits data into fixed-sized volumes (blocks) with unique addresses. Functions like a raw, unformatted hard drive attached to a virtual server. | Virtual machine boot disks, high-performance transactional databases. | AWS EBS (Elastic Block Store) |
| **File Storage** | Organizes data in a hierarchical tree structure of folders and files, accessible over network protocols like NFS or SMB. | Shared file repositories, legacy enterprise software, central media asset storage. | AWS EFS (Elastic File System) |
| **Object Storage** | Manages data as self-contained objects containing raw binary data, metadata, and a unique identifier within a flat address space. | Unstructured media (photos, videos), system backups, cloud-native application storage. | AWS S3 (Simple Storage Service) |

## Recommendation for Client Application

Object Storage is the best fit for storing user-uploaded images in a photo-sharing application because it scales endlessly without requiring host partition management or disk resizing. Since files are addressed via flat HTTP REST endpoints rather than complex filesystem trees, media can be uploaded and served directly over the web efficiently and cost-effectively.
