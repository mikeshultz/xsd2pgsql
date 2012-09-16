xsd2pgsql
=========

Create a DB structure from an XML Schema.

Usage
=====
Ouput of ``--help``::

    usage: xsd2pgsql.py [-h] [-f] [-a] [-d [NAME]] [-u [USERNAME]] [-p [PASSWORD]]
                        [-n [HOSTNAME]] [-P [PORT]]
                        FILE [FILE ...]

    Create a database based on an XSD schema. If no database name is specified,
    SQL is output to stdout.

    positional arguments:
      FILE                  XSD file to base the Postgres Schema on

    optional arguments:
      -h, --help            show this help message and exit
      -f, --fail            Fail on finding a bad XS type
      -a, --as-is           Don't normalize element names
      -d [NAME], --database [NAME]
                            DB Name
      -u [USERNAME], --user [USERNAME]
                            DB Username
      -p [PASSWORD], --password [PASSWORD]
                            DB Password
      -n [HOSTNAME], --host [HOSTNAME]
                            DB Host
      -P [PORT], --port [PORT]
                            DB Port (Default: 5432)
