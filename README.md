# README #

Remember to move or add tag for release of any follow up commits to repository if commit is to be included in production.

### OpenEMR Repository for wkhtmltopdf Binaries ###

* This is a composer repository to hold binaries for the PdfCreator class.
* This repository current version .1 - wkhtmltopdf version 0.12.4 - current release 0.12.4.1

### Command Line Implementation ###

* Change into openemr's root directory. Installed composer is required.
* Run:> composer require "openemr/wkhtmltopdf-openemr"
* Application will attempt to set execute permission to binaries if User owner allows otherwise, set from command line. 0544 should work in most instances.
* Following is one way: > sudo find vendor/openemr/wkhtmltopdf-openemr/bin -type f -exec chmod 544 {} \; 

### Compsoer.json Edit ###

* Add required: "openemr/wkhtmltopdf-openemr" : "0.12.4.1"
* Add this repository: "type" : "vcs", "url" : "https://github.com/openemr/wkhtmltopdf-openemr"
