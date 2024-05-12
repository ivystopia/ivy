# Backups for myself

> [Unlicense](https://github.com/ivystopia/ivy/blob/main/scripts/LICENSE)

## sync_to_s3

`sync_to_s3`

* A Bash script in my PATH.
* It automatically uploads all files from the current directory to a matching-named S3 bucket.
* It functions similarly to `cd foobar && aws s3 sync . s3://foobar`, but it also preserves the remote Content-Type of each object during the upload.

## invalidate_all_cloudfront

`invalidate_all_cloudfront`

* A Bash script in my PATH.
* It invalidates all the paths `/*` on every CloudFront distribution you have access to.

## delete_bucket

`delete_bucket`

* A Python script in my PATH.
* Deletes an S3 bucket even if it has versioning enabled.
* All objects in the bucket are deleted permanently.
* Requires `boto3`.

## docker-compose-monerod.yml

`docker-compose-monerod.yml`

* Docker compose file for running Monero Daemon
* Uses [simple-monerod](https://github.com/sethforprivacy/simple-monerod-docker) image
