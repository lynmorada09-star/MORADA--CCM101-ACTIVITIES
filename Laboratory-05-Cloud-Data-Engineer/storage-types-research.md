# Research: Cloud Storage Types

## Comparison Table

| Storage Type | Description (How it stores data) | Primary Use Case | Cloud Provider Example |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splitting data into fixed-sized volumes called blocks, each with its own address. Acts like an raw unformatted hard drive attached to a virtual machine. | Operating systems, databases, high-performance transactional applications. | AWS EBS (Elastic Block Store) |
| **File Storage** | Storing data in a hierarchical file system tree with folders, subfolders, and files using protocols like NFS or SMB. | Shared file systems, legacy enterprise application storage, content management systems. | AWS EFS (Elastic File System) |
| **Object Storage** | Storing data as discrete objects containing raw data, customizable metadata, and a unique identifier within a flat address space. | Unstructured data (images, videos, backups), big data analytics, modern cloud-native apps. | AWS S3 (Simple Storage Service) |

## Recommendation for Client Application

Object Storage is the ideal choice for storing user-uploaded images in a photo-sharing application because it provides virtually infinite scalability and a flat namespace designed for massive amounts of unstructured data. Unlike traditional block or file storage, object storage decouples file access from the web server host, allowing images to be served directly via HTTP REST APIs while accommodating high traffic volume at a fraction of the cost.
```[cite: 1]

---

### Step 3: Deploy MinIO Container (Checkpoint 3)

1. Launch your **KillerCoda Ubuntu/Docker Playground**[cite: 1].
2. Execute the official Docker run command to pull and launch MinIO[cite: 1]:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"
```[cite: 1]

3. Verify that the container is actively running[cite: 1]:

```bash
docker ps
```[cite: 1]

4. **Take Screenshot 1:** Capture your terminal showing both the successful container creation hash and the `docker ps` table output[cite: 1]. Save this screenshot as `minio-deployed.png` inside `Laboratory-05-Cloud-Data-Engineer/screenshots/`[cite: 1].

---

### Step 4: Web Console Access & Bucket Creation (Checkpoint 4)

1. In KillerCoda, click on **Traffic / Ports** (or **Custom Ports**) in the top menu[cite: 1].
2. Type **`9001`** and open the port[cite: 1].
3. Log into the MinIO Console using[cite: 1]:
   * **Username:** `cloudadmin`[cite: 1]
   * **Password:** `CloudNova2026!`[cite: 1]
4. Select **Buckets** on the left menu, click **Create Bucket**, and name it: **`client-photos`**[cite: 1].
5. Click into your new `client-photos` bucket and click **Upload** to upload any image or test file from your computer[cite: 1].
6. **Take Screenshot 2:** Capture the browser showing the `client-photos` bucket contents containing your uploaded file[cite: 1]. Save this as `minio-bucket-upload.png` inside `Laboratory-05-Cloud-Data-Engineer/screenshots/`[cite: 1].

---

### Step 5: Technical Documentation & README (Checkpoint 5)

Write the following into `minio-deployment.md`[cite: 1]:

```markdown
# MinIO Deployment Documentation

## Technical Overview

- **Deployment Command:**
  ```bash
  docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  minio/minio server /data --console-address ":9001"
