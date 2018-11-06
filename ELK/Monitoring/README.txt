Steps to configure Monitoring: 

Untar Metricbeat:
tar -xvf metricbeat.tar.gz
Edit metricbeat.yml:
Configure ES  + index to dump metricbeat data into

Configure Kibana dashboard UI for dumper ES
./metricbeat

Metricbeat has started!
./metricbeat -e -d "*"

chmod go-w .../metricbeat-6.2.4-linux-x86_64/metricbeat.yml
chmod go-w .../metricbeat-6.2.4-linux-x86_64/modules.d/system.yml
chmod go-w .../metricbeat-6.2.4-linux-x86_64/modules.d/nginx.yml


Running metricbeat in background:
nohup ./metricbeat -e -d "*" &> nohup_metricbeat.out &