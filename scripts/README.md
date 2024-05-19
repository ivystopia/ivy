# Backups for myself

> This is free and unencumbered software released into the public domain.
>
> Anyone is free to copy, modify, publish, use, compile, sell, or
> distribute this software, either in source code form or as a compiled
> binary, for any purpose, commercial or non-commercial, and by any
> means.
>
> In jurisdictions that recognize copyright laws, the author or authors
> of this software dedicate any and all copyright interest in the
> software to the public domain. We make this dedication for the benefit
> of the public at large and to the detriment of our heirs and
> successors. We intend this dedication to be an overt act of
> relinquishment in perpetuity of all present and future rights to this
> software under copyright law.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
> EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
> NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM,
> DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
> OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR
> THE USE OR OTHER DEALINGS IN THE SOFTWARE.
>
> For more information, please refer to <https://unlicense.org>


## sync_to_s3

[sync_to_s3](./sync_to_s3)

* A Bash script in my PATH.
* It automatically uploads all files from the current directory to a matching-named S3 bucket.
* It functions similarly to `cd foobar && aws s3 sync . s3://foobar`, but it also preserves the remote Content-Type of each object during the upload.

## invalidate_all_cloudfront

[invalidate_all_cloudfront](./invalidate_all_cloudfront)

* A Bash script in my PATH.
* It invalidates all the paths `/*` on every CloudFront distribution you have access to.

## delete_bucket

[delete_bucket](./delete_bucket)

* A Python script in my PATH.
* Deletes an S3 bucket even if it has versioning enabled.
* All objects in the bucket are deleted permanently.
* Requires `boto3`.
