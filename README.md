#### pcp-zabbix-templates

There you can find templates to use with zabbix + pcp zabbix plugin.

##### Notes:
* Those templates are tested only on Linux, with 3.0 zabbix-agent and server
* They are exported from zabbix 3.0 instance and might not work with older versions  
* I use grafana for graphs, so graphs in zabbix can be wrong (or just lacking)  
* I started using zabbix not so long ago, so some items might be just plain wrong
* And this is still work-in-progress, so use at your own risk.

#### Components/Templates:
##### Discovery script
Required for discovery rules in Linux template.  
Can discover disks and network interfaces.  
##### Linux
Work-in-progress.  
Core system monitoring. Just like stock "Template OS Linux" with a bit more info.  
Features: 
* In-depth network monitoring (TCP connections, retransmits, UDP datagrams and so on)
* Memory monitoring: usage, faults, major faults  

With discovery script installed:
* Per-interface monitoring (errors, packets, bytes)
* Per-disk monitoring (IOPS, Bytes read/written, etc)

##### MySQL
Requires MySQL PMDAS in PCP.  
Lots of metrics, mainly InnoDB-centric, like innodb buffer pool hit ratio % and stuff.
