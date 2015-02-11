Export WP posts by user
=======================

This script exports WordPress posts by user. Currently a bash script, will migrate to node.js later.

Requirements
------------

* curl
* wget

Users file
----------

List all of the users in a file called ```users``` with the following format:

```bash
# Formar: id, username
1, admin
34, JoeDirt
87, BobRoberts
...
...
```

Modify script with WP user / pass
---------------------------------

Edit the script to set the following user credentials:

```bash
wpuser='' #wordpress.com user name
wpblog='' #wordpress.com blog name (the part that appears in the domain)
wppwd='' #wordpress.com password
```

Run the script
--------------
```bash
./export
```

This will create a seperate file for each user specified in the ```users``` file. Each file will contain WordPress export xml that can be imported in any WP.org or WP.com site.

Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by:
  * [Andrew Harvey](http://andrewharvey4.wordpress.com/)
  * [Tom Vincent](http://tlvince.com/contact/)

Updated by [Sam Morrison](https://www.twitter.com/samcns)
