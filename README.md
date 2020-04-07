Updates from Offical Docker Image
==================

This image adds SSL to the official Filerun docker image. 

You must modify the docker compose to pass through port 443 in the  ports listing (after 80:80)
      - "443:443"

You must install cert.pem and key.pem in the directory that you map to /user-files/

![FileRun Logo](https://filerun.com/images/long-logo.png)

What is FileRun?
==================

[FileRun](https://filerun.com) is a self-hosted Google Drive/Photos/Music alternative. It is a full featured web based file manager with an easy to use user interface.

Installation
==================
See https://docs.filerun.com/docker for the guide.

Default login
==================

The FileRun superuser default credentials are as follows:

``username``: ``superuser``
``password``: ``superuser``

The volume ``/filerun/user-files`` has been mounted. Make sure your FileRun users home folder paths start with the path "/user-files/".

License
==================
See the following document for the [licensing terms](https://goo.gl/wk2FSs).

Issues
==================
If you have any problems with or questions about this image, please [contact us](https://filerun.com/contact).

Documentation
==================
For FileRun documentation, please visit https://docs.filerun.com/
