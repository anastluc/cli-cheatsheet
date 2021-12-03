# Google cloud cli

## Serve static files workflow

### Create a bucket
```
gsutil mb gs://<your-bucket-name>
```

### Grant read access (chmod)
```
gsutil defacl set public-read gs://<your-bucket-name>
```

### Upload a local folder to the bucket
```
gsutil -m rsync -r ./static gs://<your-bucket-name>/static
```
