## Talend ETL example
The example consists of 4 ETL jobs. Two CSV input files with customers and states will be aggregated into a postgres DB and finally written out into a CSV result file.

# Postgres DB
* Run a postgres docker image which listens on port 5433 
* Create a DB airflow and a user airflow with password airflow

# Talend Installation
* Install [JRE8](http://www.webupd8.org/2012/09/install-oracle-java-8-in-ubuntu-via-ppa.html)
* Download and unzip [Talend Open Studio for Linux](https://de.talend.com/products/data-integration-manuals-release-notes/)
* Install GTK2: sudo apt-get install libgtk2.0
* Start TOS with linux x86 shell script
* Create a new project

# Install the ETL jobs
* Clone the talend_customer_example
* Copy the content into your new project and refresh in TOS
* Install missing dependiencies within TOS
* CSV Input files are contained within [talend_kub_airflow](https://github.com/marodeur100/talend_kub_airflow)
* Clone talend_airflow and change the context within TOS to link to the input_files within talend_kub_airflow
* You should be able to run the example now
