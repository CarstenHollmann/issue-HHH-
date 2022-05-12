# Reproducer for Hibernate issue HHH-15265

If you have defined table/column comments in you mapping file, the configured schema (config file) would not be added to the SQL to create the comments in the database since Hibernate version 5.6.2.

See https://hibernate.atlassian.net/browse/HHH-15265


## Test before the issue

Change the ``<version.org.hibernate>`` value in the pom.xml to ``5.6.1.Final`` to get the valid version.

