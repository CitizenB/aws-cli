=========
CHANGELOG
=========

1.2.2
=====

* Fix an issue causing ``s3 sync`` with the ``--delete`` incorrectly deleting files (issue 440)
* Fix an issue with ``--output text`` combined with paginated results (boto/botocore#165)
* Fix a bug in text output when an empty list is encountered (issue 446)


1.2.1
=====

* Update the AWS Direct Connect command to support the latest features
* Fix text output with single scalar value (issue 428)
* Fix shell quoting for ``PAGER``/``MANPAGER`` environment variable (issue 429)
* --endpoint-url is explicitly used for URL of remote service (boto/botocore#163)
* Fix an validation error when using ``--ip-permissions`` and ``--group-id`` together (issue 435)


1.2.0
=====

* Update Amazon Elastic Transcoder command with audio transcoding features
* Improve text output (``--output text``) to have a consistent output structure
* Add ``--query`` argument that allows you to specify output data using a JMESPath expression
* Upgrade requests library to 2.0.0
* Update Amazon Redshift region configuration to include ``ap-southeast-1``  and ``ap-southeast-2``
* Update Amazon S3 region configuration to include ``fips-us-gov-west-1``
* Add a bundled installer for the CLI which bundles all necessary dependencies (does not require pip)
* Fix an issue with ZSH tab completion (issue 411)
* Fix an issue with S3 requests timing out (issue 401)
* Fix an issue with ``s3api delete-objects`` not providing the ``Content-MD5`` header (issue 400)


1.1.2
=====

* Update the Amazon EC2 command to support Reserved Instance instance type modifications
* Update the AWS OpsWorks command to support new resource management features
* Fix an issue when transferring files on different drives on Windows
* Fix an issue that caused interactive help to emit control characters on certain Linux distributions


1.1.1
=====

* Update the Amazon CloudFront command to support the latest API version 2013-08-26
* Update the Auto Scaling client to support public IP address association of instances
* Update Amazon SWF to support signature version 4
* Update Amazon RDS with a new subcommand, ``add-source-identifier-to-subscription``


1.1.0
=====

* Update the ``s3`` commands to support the setting for how objects are stored in Amazon S3
* Update the Amazon EC2 command to support the latest API version (2013-08-15)
* Fix an issue causing excessive CPU utilization in some scenarios where many files were being uploaded
* Fix a memory growth issue with ``s3`` copying and syncing of files
* Fix an issue caused by a conflict with a dependency and Python 3.x that caused installation to fail
