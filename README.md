# public-html-config

Contains any files + top-level htaccess/config files needed to set up the `public_html` folder

We are currently using Bluehost to host our files. Whenever we create a subdomain, what Bluehost 
will do is create a folder inside `public_html` containing all files for that subdomain.

Unfortunately, that means that the folder for the subdomain is mixed with all files served from the 
top-level domain, which is untidy. 

The solution we're using is to create a separate `main` subfolder that will contain all files for 
the main website. 

This repo contains the `.htaccess` file needed to actually make that all work out.

## Deployment

Simply copy the contents of the `dist` folder into `public_html`. 
