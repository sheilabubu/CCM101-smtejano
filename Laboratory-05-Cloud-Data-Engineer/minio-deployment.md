# MinIO Deployment Documentation

## Docker Command Used

The MinIO object storage server was deployed using Docker with the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
```

## Web Console Port

The MinIO Web Console was accessed using port:

```text
9001
```

Port 9000 was used for the MinIO API, while port 9001 was used for the Web Console.

## Bucket Created

The bucket created in the MinIO Web Console was:

```text
client-photos
```

A sample file was uploaded to the bucket to verify that the object storage server was working correctly.

## Environment Variables

The `-e` flags in the Docker command were used to set environment variables for the MinIO server.

* `MINIO_ROOT_USER=cloudadmin` sets the username for the MinIO administrator account.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the password for the MinIO administrator account.

These environment variables provide the login credentials used to access the MinIO Web Console.

