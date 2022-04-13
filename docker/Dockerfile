FROM apache/superset:1.4.2

# Switching to root to install the required packages
USER root

# installing the redshift driver to connect to the datawarehouse
RUN pip install sqlalchemy-redshift

# Switching back to using the `superset` user
USER superset