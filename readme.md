## Flask S3 Uploader

This is a basic example showing how to use Flask, Flask-WTF and Boto
to automatically upload user files to S3, bypassing storage on the server.

## Quick Start

Update config.py with your Amazon details.

## Other Notes

The most efficient way of handling the downloads is likely to be
just upload the file to the local webserver to enable a quick
as possible response to the user, then adding the 'upload to S3'
task to a message/task queue that runs in the background as the
server can manage.