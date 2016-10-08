FROM ubuntu

RUN apt-get update
RUN apt-get install -y python-netsnmp python-pip apt-utils software-properties-common
RUN apt-add-repository multiverse
RUN apt-get update
RUN apt-get install -y snmp-mibs-downloader
RUN pip install snmp_exporter
CMD snmp_exporter /etc/snmp_exporter.yml
