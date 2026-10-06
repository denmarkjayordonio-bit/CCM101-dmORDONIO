# MinIO Deployment

For this laboratory, I deployed MinIO using Docker inside the KillerCoda Ubuntu environment. The MinIO image provided in the original instructions did not work in my setup, so I used the `elestio/minio` image instead.

First, I downloaded the MinIO image using:

```bash
docker pull elestio/minio

After the image was downloaded, I created the MinIO container using:

docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
elestio/minio server /data --console-address ":9001"

The container was named minio-server. Port 9000 was used for the MinIO API, while port 9001 was assigned to the MinIO Web Console.

I checked the container using:

docker ps

The result showed that the minio-server container was running properly and that the required ports were successfully mapped.

Result

The MinIO server was successfully deployed using Docker. I was also able to continue with the MinIO Web Console and use it for the storage activities.
