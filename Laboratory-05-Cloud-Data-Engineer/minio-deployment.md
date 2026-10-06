## I deployed **MinIO** using Docker in the **KillerCoda Ubuntu Playground**. The original MinIO image provided in the instructions was not working in my environment, so I used the `elestio/minio` image instead. This image worked properly with my Docker setup.

The command I used was:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
elestio/minio server /data --console-address ":9001"
```

## MinIO Ports and Bucket

I used port `9001` to open the **MinIO Web Console**, while port `9000` is used for the **MinIO API**.

After starting MinIO, I created a bucket named:

`client-photos`

This bucket was used to store the sample file that I uploaded.

The `-e` options in the command were used to set the administrator login credentials.

* `MINIO_ROOT_USER=cloudadmin` sets the administrator username.
* `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the administrator password.

## Checking the Docker Container

To verify that MinIO was running properly, I used:

```bash
docker ps
```

The result showed that the `minio-server` container was running successfully. It also confirmed that ports `9000` and `9001` were properly mapped.

