# MinIO Deployment

## Docker Command

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"


##The command above was used to deploy the MinIO object storage server using Docker. It maps port 9000 for the MinIO API and port 9001 for the MinIO Web Console.

Web Console Port

The MinIO Web Console was accessed using port 9001.

Port 9000 is used for the MinIO API, while port 9001 is used for the MinIO Web Console.

Bucket Name

The bucket created for the photo-sharing application is:

client-photos

The bucket is used to store the sample file uploaded during the activity.

Environment Variables

The -e flags in the Docker command set environment variables for the MinIO server.

MINIO_ROOT_USER=cloudadmin sets the root username.
MINIO_ROOT_PASSWORD=CloudNova2026! sets the root password.

These environment variables provide the login credentials used to access the MinIO Web Console.
