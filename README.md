# from-s3

This is an HTCondor DAG that runs a DAG per file in an S3 bucket.  Specify
the bucket in the **arguments** line of `fetch.submit` and its region in
the **tranfer_input_files** line of `from-s3.submit`; you will also need to
specify the access/secret key files.

The scripting depends on the `aws` command-line tool being installed and
configured to use the same keys as the submit file.

The script `from-s3.sh` will be run with the file from S3's name on the
command line, and the file available at that name in the sandbox.
