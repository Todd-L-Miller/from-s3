# from-s3

This is an HTCondor DAG that runs a DAG per file in an S3 bucket.  Specify
the bucket in the **arguments** line of `fetch.submit`.  The script `from-s3.sh`
will be run with the file from S3's name on the command line.
