# Mission Reflection

Object storage is far better suited for storing millions of user photos than a traditional block storage drive because of its flat address structure and HTTP-native architecture. Block storage binds hard drives directly to virtual server instances, forcing engineers to constantly manage disk space limits, filesystem overhead, and volume attachments. In contrast, object storage treats every uploaded image (like `aws-homepage.png`) as a distinct object with custom metadata, serving it directly via S3 API calls with near-limitless capacity.

Using Docker made deploying the MinIO server effortless. Instead of installing binary packages, setting up system services, and manually configuring environment variables on the Ubuntu host, a single `docker run` command pulled the `elestio/minio` image and spun up a functional object storage instance with port forwarding and custom credentials in less than 10 seconds.

In cloud computing, a "bucket" (such as our `client-photos` bucket) acts as a top-level logical container for organizing objects. It serves as an administrative boundary where engineers define security access policies, bucket privacy settings, encryption rules, and data retention lifecycles.

Enterprise companies ensure their object storage data remains safe during physical server crashes by implementing cross-region replication and erasure coding. Erasure coding divides data into chunks, calculates parity bits, and distributes them across multiple independent storage nodes, enabling complete data recovery even if multiple physical hard drives or entire nodes fail simultaneously.

Working directly in the KillerCoda terminal has noticeably strengthened my Linux command line skills. Commands like `docker ps` to verify container states and `docker logs minio-server` to inspect live container output are now becoming second nature.
