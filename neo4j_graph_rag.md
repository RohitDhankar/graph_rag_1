
systemctl {start|stop|restart} neo4j
systemctl start neo4j

```bash

$ 
dhankar@dhankar-1:.../neo4j$ sudo apt install openjdk-21-jdk
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  cuda-command-line-tools-11-0 cuda-compiler-11-0 cuda-cudart-11-0 cuda-cudart-dev-11-0 cuda-cuobjdump-11-0 cuda-cupti-11-0
  cuda-cupti-dev-11-0 cuda-documentation-11-0 cuda-driver-dev-11-0 cuda-gdb-11-0 cuda-libraries-11-0 cuda-libraries-dev-11-0
  cuda-memcheck-11-0 cuda-nsight-11-0 cuda-nsight-compute-11-0 cuda-nsight-systems-11-0 cuda-nvcc-11-0 cuda-nvdisasm-11-0 cuda-nvml-dev-11-0
  cuda-nvprof-11-0 cuda-nvprune-11-0 cuda-nvrtc-11-0 cuda-nvrtc-dev-11-0 cuda-nvtx-11-0 cuda-nvvp-11-0 cuda-samples-11-0 cuda-sanitizer-11-0
  cuda-toolkit-11-0 cuda-tools-11-0 cuda-visual-tools-11-0 dctrl-tools dkms freeglut3 freeglut3-dev libcublas-11-0 libcublas-dev-11-0
  libcufft-11-0 libcufft-dev-11-0 libcurand-11-0 libcurand-dev-11-0 libcusolver-11-0 libcusolver-dev-11-0 libcusparse-11-0
  libcusparse-dev-11-0 libgl1-mesa-dev libnpp-11-0 libnpp-dev-11-0 libnvjpeg-11-0 libnvjpeg-dev-11-0 libpython2-stdlib libpython2.7-minimal
  libpython2.7-stdlib linux-generic linux-headers-generic nsight-compute-2020.1.1 nsight-compute-2023.1.1 nsight-systems-2020.3.2
  nvidia-modprobe python-tk python2 python2-minimal python2.7 python2.7-minimal
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  openjdk-21-jdk-headless
Suggested packages:
  openjdk-21-demo openjdk-21-source visualvm
The following NEW packages will be installed:
  openjdk-21-jdk openjdk-21-jdk-headless
0 upgraded, 2 newly installed, 0 to remove and 56 not upgraded.
Need to get 86.0 MB of archives.
After this operation, 99.8 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://archive.linux.duke.edu/ubuntu jammy-updates/universe amd64 openjdk-21-jdk-headless amd64 21.0.7+6~us1-0ubuntu1~22.04 [82.6 MB]
Get:2 http://archive.linux.duke.edu/ubuntu jammy-updates/universe amd64 openjdk-21-jdk amd64 21.0.7+6~us1-0ubuntu1~22.04 [3,386 kB]          
Fetched 86.0 MB in 27s (3,142 kB/s)                                                                                                          
Selecting previously unselected package openjdk-21-jdk-headless:amd64.
(Reading database ... 413464 files and directories currently installed.)
Preparing to unpack .../openjdk-21-jdk-headless_21.0.7+6~us1-0ubuntu1~22.04_amd64.deb ...
Unpacking openjdk-21-jdk-headless:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
Selecting previously unselected package openjdk-21-jdk:amd64.
Preparing to unpack .../openjdk-21-jdk_21.0.7+6~us1-0ubuntu1~22.04_amd64.deb ...
Unpacking openjdk-21-jdk:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
Setting up openjdk-21-jdk-headless:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jar to provide /usr/bin/jar (jar) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jarsigner to provide /usr/bin/jarsigner (jarsigner) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/javac to provide /usr/bin/javac (javac) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/javadoc to provide /usr/bin/javadoc (javadoc) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/javap to provide /usr/bin/javap (javap) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jcmd to provide /usr/bin/jcmd (jcmd) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jdb to provide /usr/bin/jdb (jdb) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jdeprscan to provide /usr/bin/jdeprscan (jdeprscan) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jdeps to provide /usr/bin/jdeps (jdeps) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jfr to provide /usr/bin/jfr (jfr) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jimage to provide /usr/bin/jimage (jimage) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jinfo to provide /usr/bin/jinfo (jinfo) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jlink to provide /usr/bin/jlink (jlink) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jmap to provide /usr/bin/jmap (jmap) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jmod to provide /usr/bin/jmod (jmod) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jps to provide /usr/bin/jps (jps) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jrunscript to provide /usr/bin/jrunscript (jrunscript) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jshell to provide /usr/bin/jshell (jshell) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jstack to provide /usr/bin/jstack (jstack) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jstat to provide /usr/bin/jstat (jstat) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jstatd to provide /usr/bin/jstatd (jstatd) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jwebserver to provide /usr/bin/jwebserver (jwebserver) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/serialver to provide /usr/bin/serialver (serialver) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jhsdb to provide /usr/bin/jhsdb (jhsdb) in auto mode
Setting up openjdk-21-jdk:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jconsole to provide /usr/bin/jconsole (jconsole) in auto mode
dhankar@dhankar-1:.../neo4j$ 
dhankar@dhankar-1:.../neo4j$ sudo systemctl start neo4j.service
dhankar@dhankar-1:.../neo4j$ 
dhankar@dhankar-1:.../neo4j$ sudo systemctl status neo4j.service
○ neo4j.service - Neo4j Graph Database
     Loaded: loaded (/lib/systemd/system/neo4j.service; enabled; vendor preset: enabled)
     Active: inactive (dead) since Sun 2025-05-25 21:22:32 IST; 3s ago
    Process: 97266 ExecStart=/usr/share/neo4j/bin/neo4j console (code=exited, status=0/SUCCESS)
   Main PID: 97266 (code=exited, status=0/SUCCESS)
        CPU: 112ms

May 25 21:22:32 dhankar-1 systemd[1]: Started Neo4j Graph Database.
May 25 21:22:32 dhankar-1 neo4j[97266]: Unsupported Java 11.0.27 detected. Please use Java(TM) 21 to run Neo4j Server.
May 25 21:22:32 dhankar-1 systemd[1]: neo4j.service: Deactivated successfully.
dhankar@dhankar-1:.../neo4j$ 
dhankar@dhankar-1:.../neo4j$ 


```

#
```bash
$ sudo systemctl enable neo4j.service
Synchronizing state of neo4j.service with SysV service script with /lib/systemd/systemd-sysv-install.
Executing: /lib/systemd/systemd-sysv-install enable neo4j
Created symlink /etc/systemd/system/multi-user.target.wants/neo4j.service → /lib/systemd/system/neo4j.service.
```

#

```bash
$ sudo systemctl start neo4j.service
dhankar@dhankar-1:.../neo4j$ 
dhankar@dhankar-1:.../neo4j$ sudo systemctl status neo4j.service
○ neo4j.service - Neo4j Graph Database
     Loaded: loaded (/lib/systemd/system/neo4j.service; enabled; vendor preset: enabled)
     Active: inactive (dead) since Sun 2025-05-25 21:15:55 IST; 13s ago
    Process: 96535 ExecStart=/usr/share/neo4j/bin/neo4j console (code=exited, status=0/SUCCESS)
   Main PID: 96535 (code=exited, status=0/SUCCESS)
        CPU: 129ms

May 25 21:15:55 dhankar-1 systemd[1]: Started Neo4j Graph Database.
May 25 21:15:55 dhankar-1 neo4j[96535]: Unsupported Java 11.0.27 detected. Please use Java(TM) 21 to run Neo4j Server.
May 25 21:15:55 dhankar-1 systemd[1]: neo4j.service: Deactivated successfully.
dhankar@dhankar-1:.../neo4j$ 

```
#

```bash
 systemctl cat neo4j
# /lib/systemd/system/neo4j.service
[Unit]
Description=Neo4j Graph Database
After=network-online.target
Wants=network-online.target

[Service]
ExecStart=/usr/share/neo4j/bin/neo4j console
Restart=on-abnormal
User=neo4j
Group=neo4j
Environment="NEO4J_CONF=/etc/neo4j" "NEO4J_HOME=/var/lib/neo4j"
LimitNOFILE=60000
TimeoutSec=120

[Install]
WantedBy=multi-user.target

```

#


cd /etc/neo4j/

```bash
$ cd /etc/neo4j/
dhankar@dhankar-1:.../neo4j$ ls -lahtr
total 56K
-rw-r--r--   1 neo4j adm  2.3K Apr 17 15:55 user-logs.xml
-rw-r--r--   1 neo4j adm  4.8K Apr 17 15:55 server-logs.xml
-rw-r--r--   1 neo4j adm  4.3K Apr 17 15:55 neo4j-admin.conf
-rw-r--r--   1 neo4j adm   17K Apr 25 02:00 neo4j.conf
drwxr-xr-x   2 neo4j adm  4.0K May 25 19:43 .
drwxr-xr-x 171 root  root  12K May 25 19:43 ..
dhankar@dhankar-1:.../neo4j$ 

```



-- pip install neo4j
-- pip install langchain-community
-- pip install langchain

-- https://pypi.org/project/neo4j/

- The Neo4j Operations Manual
- https://neo4j.com/docs/operations-manual/current/


-------------------------

##### content as is of the files at path - /etc/neo4j
-rw-r--r--   1 neo4j adm  4.3K Apr 17 15:55 neo4j-admin.conf
-rw-r--r--   1 neo4j adm   17K Apr 25 02:00 neo4j.conf

-------------------------


```bash
# You can also choose a specific advertised hostname or IP address, and
# configure an advertised port for each connector, by setting their
# individual advertised_address.

# By default, encryption is turned off.
# To turn on encryption, an ssl policy for the connector needs to be configured
# Read more in SSL policy section in this file for how to define a SSL policy.

# Bolt connector
server.bolt.enabled=true
#server.bolt.tls_level=DISABLED
#server.bolt.listen_address=:7687
#server.bolt.advertised_address=:7687

# HTTP Connector. There can be zero or one HTTP connectors.
server.http.enabled=true
#server.http.listen_address=:7474
#server.http.advertised_address=:7474

# HTTPS Connector. There can be zero or one HTTPS connectors.
server.https.enabled=false
#server.https.listen_address=:7473
#server.https.advertised_address=:7473

# Number of Neo4j worker threads.
#server.threads.worker_count=

#*****************************************************************

```





##### Neo4J - Graph RAG 

- https://neo4j.com/blog/developer/microsoft-graphrag-neo4j/

##### Initial Code Credits --  
- Initial Source Code - https://github.com/tomasonjo/blogs/blob/master/msft_graphrag/ms_graphrag_import.ipynb

#
```bash
(base) dhankar@dhankar-1:~/.../artifacts$ pwd
graph_rag/neo4j/data_dir/artifacts
(base) dhankar@dhankar-1:~/.../artifacts$ tree
.
├── create_base_documents.parquet
├── create_base_entity_graph.parquet
├── create_base_extracted_entities.parquet
├── create_base_text_units.parquet
├── create_final_communities.parquet
├── create_final_community_reports.parquet
├── create_final_documents.parquet
├── create_final_entities.parquet
├── create_final_nodes.parquet
├── create_final_relationships.parquet
├── create_final_text_units.parquet
├── create_summarized_entities.parquet
├── join_text_units_to_entity_ids.parquet
├── join_text_units_to_relationship_ids.parquet
└── stats.json

0 directories, 15 files

#
base) dhankar@dhankar-1:~/.../artifacts$ ls -lahtr
total 4.7M
-rw-r--r-- 1 dhankar dhankar 152K Jul  3  2024 create_base_text_units.parquet
-rw-r--r-- 1 dhankar dhankar 129K Jul  3  2024 create_base_extracted_entities.parquet
-rw-r--r-- 1 dhankar dhankar 149K Jul  3  2024 create_summarized_entities.parquet
-rw-r--r-- 1 dhankar dhankar 540K Jul  3  2024 create_base_entity_graph.parquet
-rw-r--r-- 1 dhankar dhankar 2.8M Jul  3  2024 create_final_entities.parquet
-rw-r--r-- 1 dhankar dhankar  29K Jul  3  2024 join_text_units_to_entity_ids.parquet
-rw-r--r-- 1 dhankar dhankar 117K Jul  3  2024 create_final_nodes.parquet
-rw-r--r-- 1 dhankar dhankar  26K Jul  3  2024 create_final_communities.parquet
-rw-r--r-- 1 dhankar dhankar  22K Jul  3  2024 join_text_units_to_relationship_ids.parquet
-rw-r--r-- 1 dhankar dhankar  81K Jul  3  2024 create_final_relationships.parquet
-rw-r--r-- 1 dhankar dhankar 5.6K Jul  3  2024 stats.json
-rw-r--r-- 1 dhankar dhankar 172K Jul  3  2024 create_final_text_units.parquet
-rw-r--r-- 1 dhankar dhankar 125K Jul  3  2024 create_final_documents.parquet
-rw-r--r-- 1 dhankar dhankar 241K Jul  3  2024 create_final_community_reports.parquet
-rw-r--r-- 1 dhankar dhankar 125K Jul  3  2024 create_base_documents.parquet
drwxr-xr-x 2 dhankar dhankar 4.0K Jul  3  2024 .
drwxrwxr-x 3 dhankar dhankar 4.0K May 25 14:58 ..

```
#

#### Windows installation
- https://neo4j.com/docs/operations-manual/current/installation/windows/

Not done 

#



#

- https://neo4j.com/docs/operations-manual/current/installation/linux/debian/

Most Neo4j configuration goes into neo4j.conf.

For operating systems using systemd, some package-specific options are set in neo4j.service and can be edited using systemctl edit neo4j.service.

For operating systems that are not using systemd, some package-specific options are set in /etc/default/neo4j.


#### Install - Neo4j Ubuntu Local Install 


```bash

$ sudo apt-get install neo4j -y
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following packages were automatically installed and are no longer required:
  cuda-command-line-tools-11-0 cuda-compiler-11-0 cuda-cudart-11-0 cuda-cudart-dev-11-0 cuda-cuobjdump-11-0 cuda-cupti-11-0
  cuda-cupti-dev-11-0 cuda-documentation-11-0 cuda-driver-dev-11-0 cuda-gdb-11-0 cuda-libraries-11-0 cuda-libraries-dev-11-0
  cuda-memcheck-11-0 cuda-nsight-11-0 cuda-nsight-compute-11-0 cuda-nsight-systems-11-0 cuda-nvcc-11-0 cuda-nvdisasm-11-0 cuda-nvml-dev-11-0
  cuda-nvprof-11-0 cuda-nvprune-11-0 cuda-nvrtc-11-0 cuda-nvrtc-dev-11-0 cuda-nvtx-11-0 cuda-nvvp-11-0 cuda-samples-11-0 cuda-sanitizer-11-0
  cuda-toolkit-11-0 cuda-tools-11-0 cuda-visual-tools-11-0 dctrl-tools dkms freeglut3 freeglut3-dev libcublas-11-0 libcublas-dev-11-0
  libcufft-11-0 libcufft-dev-11-0 libcurand-11-0 libcurand-dev-11-0 libcusolver-11-0 libcusolver-dev-11-0 libcusparse-11-0
  libcusparse-dev-11-0 libgl1-mesa-dev libnpp-11-0 libnpp-dev-11-0 libnvjpeg-11-0 libnvjpeg-dev-11-0 libpython2-stdlib libpython2.7-minimal
  libpython2.7-stdlib linux-generic linux-headers-generic nsight-compute-2020.1.1 nsight-compute-2023.1.1 nsight-systems-2020.3.2
  nvidia-modprobe python-tk python2 python2-minimal python2.7 python2.7-minimal
Use 'sudo apt autoremove' to remove them.
The following additional packages will be installed:
  cypher-shell daemon openjdk-21-jre openjdk-21-jre-headless
Suggested packages:
  fonts-ipafont-gothic fonts-ipafont-mincho fonts-wqy-microhei | fonts-wqy-zenhei
The following NEW packages will be installed:
  cypher-shell daemon neo4j openjdk-21-jre openjdk-21-jre-headless
0 upgraded, 5 newly installed, 0 to remove and 56 not upgraded.
Need to get 240 MB of archives.
After this operation, 420 MB of additional disk space will be used.
Get:1 https://debian.neo4j.com stable/latest amd64 cypher-shell all 1:2025.04.0 [39.7 MB]
Get:2 http://archive.linux.duke.edu/ubuntu jammy/universe amd64 daemon amd64 0.8-1 [60.9 kB]
Get:3 http://archive.linux.duke.edu/ubuntu jammy-updates/universe amd64 openjdk-21-jre-headless amd64 21.0.7+6~us1-0ubuntu1~22.04 [46.8 MB]
Get:4 https://debian.neo4j.com stable/latest amd64 neo4j all 1:2025.04.0 [154 MB]        
Get:5 http://archive.linux.duke.edu/ubuntu jammy-updates/universe amd64 openjdk-21-jre amd64 21.0.7+6~us1-0ubuntu1~22.04 [234 kB]            
Fetched 240 MB in 25s (9,698 kB/s)                                                                                                           
Preconfiguring packages ...
Selecting previously unselected package daemon.
(Reading database ... 412754 files and directories currently installed.)
Preparing to unpack .../daemon_0.8-1_amd64.deb ...
Unpacking daemon (0.8-1) ...
Selecting previously unselected package openjdk-21-jre-headless:amd64.
Preparing to unpack .../openjdk-21-jre-headless_21.0.7+6~us1-0ubuntu1~22.04_amd64.deb ...
Unpacking openjdk-21-jre-headless:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
Selecting previously unselected package openjdk-21-jre:amd64.
Preparing to unpack .../openjdk-21-jre_21.0.7+6~us1-0ubuntu1~22.04_amd64.deb ...
Unpacking openjdk-21-jre:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
Selecting previously unselected package cypher-shell.
Preparing to unpack .../cypher-shell_1%3a2025.04.0_all.deb ...
Unpacking cypher-shell (1:2025.04.0) ...
Selecting previously unselected package neo4j.
Preparing to unpack .../neo4j_1%3a2025.04.0_all.deb ...
Unpacking neo4j (1:2025.04.0) ...
Setting up openjdk-21-jre-headless:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/jpackage to provide /usr/bin/jpackage (jpackage) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/keytool to provide /usr/bin/keytool (keytool) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/bin/rmiregistry to provide /usr/bin/rmiregistry (rmiregistry) in auto mode
update-alternatives: using /usr/lib/jvm/java-21-openjdk-amd64/lib/jexec to provide /usr/bin/jexec (jexec) in auto mode
Setting up openjdk-21-jre:amd64 (21.0.7+6~us1-0ubuntu1~22.04) ...
Setting up daemon (0.8-1) ...
Setting up cypher-shell (1:2025.04.0) ...
Setting up neo4j (1:2025.04.0) ...
Adding system user `neo4j' (UID 138) ...
Adding new user `neo4j' (UID 138) with group `neo4j' ...
Not creating home directory `/var/lib/neo4j'.
Processing triggers for desktop-file-utils (0.26-1ubuntu3) ...
Processing triggers for hicolor-icon-theme (0.17-2) ...
Processing triggers for gnome-menus (3.36.0-1ubuntu3) ...
Processing triggers for man-db (2.10.2-1) ...
Processing triggers for mailcap (3.70+nmu1ubuntu1) ...
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 



```

#

```bash
(base) dhankar@dhankar-1:~/.../graph_rag_1$ sudo apt-get install wget curl nano software-properties-common dirmngr apt-transport-https gnupg gnupg2 ca-certificates lsb-release ubuntu-keyring unzip -y
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
lsb-release is already the newest version (11.1.0ubuntu4).
ubuntu-keyring is already the newest version (2021.03.26).
ubuntu-keyring set to manually installed.
ca-certificates is already the newest version (20240203~22.04.1).
curl is already the newest version (7.81.0-1ubuntu1.20).
dirmngr is already the newest version (2.2.27-3ubuntu2.3).
gnupg is already the newest version (2.2.27-3ubuntu2.3).
nano is already the newest version (6.2-1ubuntu0.1).
software-properties-common is already the newest version (0.99.22.9).
unzip is already the newest version (6.0-26ubuntu3.2).
wget is already the newest version (1.21.2-2ubuntu1.1).
apt-transport-https is already the newest version (2.4.13).
The following packages were automatically installed and are no longer required:
  cuda-command-line-tools-11-0 cuda-compiler-11-0 cuda-cudart-11-0 cuda-cudart-dev-11-0 cuda-cuobjdump-11-0 cuda-cupti-11-0
  cuda-cupti-dev-11-0 cuda-documentation-11-0 cuda-driver-dev-11-0 cuda-gdb-11-0 cuda-libraries-11-0 cuda-libraries-dev-11-0
  cuda-memcheck-11-0 cuda-nsight-11-0 cuda-nsight-compute-11-0 cuda-nsight-systems-11-0 cuda-nvcc-11-0 cuda-nvdisasm-11-0 cuda-nvml-dev-11-0
  cuda-nvprof-11-0 cuda-nvprune-11-0 cuda-nvrtc-11-0 cuda-nvrtc-dev-11-0 cuda-nvtx-11-0 cuda-nvvp-11-0 cuda-samples-11-0 cuda-sanitizer-11-0
  cuda-toolkit-11-0 cuda-tools-11-0 cuda-visual-tools-11-0 dctrl-tools dkms freeglut3 freeglut3-dev libcublas-11-0 libcublas-dev-11-0
  libcufft-11-0 libcufft-dev-11-0 libcurand-11-0 libcurand-dev-11-0 libcusolver-11-0 libcusolver-dev-11-0 libcusparse-11-0
  libcusparse-dev-11-0 libgl1-mesa-dev libnpp-11-0 libnpp-dev-11-0 libnvjpeg-11-0 libnvjpeg-dev-11-0 libpython2-stdlib libpython2.7-minimal
  libpython2.7-stdlib linux-generic linux-headers-generic nsight-compute-2020.1.1 nsight-compute-2023.1.1 nsight-systems-2020.3.2
  nvidia-modprobe python-tk python2 python2-minimal python2.7 python2.7-minimal
Use 'sudo apt autoremove' to remove them.
The following NEW packages will be installed:
  gnupg2
0 upgraded, 1 newly installed, 0 to remove and 56 not upgraded.
Need to get 5,544 B of archives.
After this operation, 52.2 kB of additional disk space will be used.
Get:1 http://archive.linux.duke.edu/ubuntu jammy-updates/universe amd64 gnupg2 all 2.2.27-3ubuntu2.3 [5,544 B]
Fetched 5,544 B in 1s (6,774 B/s)                       
Selecting previously unselected package gnupg2.
(Reading database ... 412748 files and directories currently installed.)
Preparing to unpack .../gnupg2_2.2.27-3ubuntu2.3_all.deb ...
Unpacking gnupg2 (2.2.27-3ubuntu2.3) ...
Setting up gnupg2 (2.2.27-3ubuntu2.3) ...
Processing triggers for man-db (2.10.2-1) ...
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 


```
#

Add the Neo4j repository with:

```bash

echo "deb [signed-by=/usr/share/keyrings/neo4j.gpg] https://debian.neo4j.com stable latest" | sudo tee -a /etc/apt/sources.list.d/neo4j.list

#

sudo apt-get update
#

```
#### ERROR 


```bash
$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ echo "deb [signed-by=/usr/share/keyrings/neo4j.gpg] https://debian.neo4j.com stable latest" | sudo tee -a /etc/apt/sources.list.d/neo4j.list
deb [signed-by=/usr/share/keyrings/neo4j.gpg] https://debian.neo4j.com stable latest
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ sudo apt-get update
Get:1 file:/var/cuda-repo-ubuntu1804-11-8-local  InRelease [1,575 B]
Get:1 file:/var/cuda-repo-ubuntu1804-11-8-local  InRelease [1,575 B]
Hit:2 http://dl.google.com/linux/chrome/deb stable InRelease
Hit:3 https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64  InRelease                                           
Hit:4 https://packages.microsoft.com/repos/azure-cli jammy InRelease                                                                  
Hit:5 https://packages.microsoft.com/repos/code stable InRelease          
Get:6 https://debian.neo4j.com stable InRelease [44.2 kB]
Err:6 https://debian.neo4j.com stable InRelease         
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 59D700E4D37F5F19
Hit:7 http://archive.linux.duke.edu/ubuntu jammy InRelease
Hit:8 http://archive.linux.duke.edu/ubuntu jammy-updates InRelease
Hit:9 http://archive.linux.duke.edu/ubuntu jammy-backports InRelease
Hit:10 http://archive.linux.duke.edu/ubuntu jammy-security InRelease
Reading package lists... Done
W: GPG error: https://debian.neo4j.com stable InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 59D700E4D37F5F19
E: The repository 'https://debian.neo4j.com stable InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 

```
#
```bash

$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ wget -O - https://debian.neo4j.com/neotechnology.gpg.key | sudo apt-key add -
--2025-05-25 18:34:44--  https://debian.neo4j.com/neotechnology.gpg.key
Resolving debian.neo4j.com (debian.neo4j.com)... Warning: apt-key is deprecated. Manage keyring files in trusted.gpg.d instead (see apt-key(8)).
108.138.192.72, 108.138.192.68, 108.138.192.98, ...
Connecting to debian.neo4j.com (debian.neo4j.com)|108.138.192.72|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3905 (3.8K) [application/pgp-keys]
Saving to: ‘STDOUT’

-                                   100%[=================================================================>]   3.81K  --.-KB/s    in 0s      

2025-05-25 18:34:44 (1.18 GB/s) - written to stdout [3905/3905]

OK
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ sudo apt-get update
Get:1 file:/var/cuda-repo-ubuntu1804-11-8-local  InRelease [1,575 B]
Get:1 file:/var/cuda-repo-ubuntu1804-11-8-local  InRelease [1,575 B]
Hit:2 https://packages.microsoft.com/repos/azure-cli jammy InRelease                                                                         
Hit:3 https://packages.microsoft.com/repos/code stable InRelease                                                                             
Hit:4 http://dl.google.com/linux/chrome/deb stable InRelease                                                                                 
Get:5 https://debian.neo4j.com stable InRelease [44.2 kB]                                                                             
Hit:6 http://archive.linux.duke.edu/ubuntu jammy InRelease                                          
Err:5 https://debian.neo4j.com stable InRelease
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 59D700E4D37F5F19
Hit:7 http://archive.linux.duke.edu/ubuntu jammy-updates InRelease
Hit:8 http://archive.linux.duke.edu/ubuntu jammy-backports InRelease
Hit:9 http://archive.linux.duke.edu/ubuntu jammy-security InRelease
Hit:10 https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64  InRelease
Reading package lists... Done
W: GPG error: https://debian.neo4j.com stable InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 59D700E4D37F5F19
E: The repository 'https://debian.neo4j.com stable InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ 


```
#
Seems to work for the Kali Repo -- 
$ wget -O - https://debian.neo4j.com/neotechnology.gpg.key | sudo apt-key add -


wget -O - https://debian.neo4j.com/neotechnology.gpg.key | gpg --dearmor | sudo tee /usr/share/keyrings/neo4j-archive-keyring.gpg

wget -O- <https://example.com/key/repo-key.gpg> | gpg --dearmor | sudo tee /usr/share/keyrings/<myrepository>-archive-keyring.gpg

$ 
(base) dhankar@dhankar-1:~/.../graph_rag_1$ wget -O - https://debian.neo4j.com/neotechnology.gpg.key | gpg --dearmor | sudo tee /usr/share/keyrings/neo4j-archive-keyring.gpg
--2025-05-25 18:51:52--  https://debian.neo4j.com/neotechnology.gpg.key
Resolving debian.neo4j.com (debian.neo4j.com)... 108.138.192.72, 108.138.192.27, 108.138.192.68, ...
Connecting to debian.neo4j.com (debian.neo4j.com)|108.138.192.72|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 3905 (3.8K) [application/pgp-keys]
Saving to: ‘STDOUT’

-                                   100%[=================================================================>]   3.81K  --.-KB/s    in 0s      

2025-05-25 18:51:53 (24.5 MB/s) - written to stdout [3905/3905]

X<��q�b}��·j9�Lݡw:��_ph/�AԵ��t���s�G!��&5?K�tOt�S#������u/�y:�C�*�0@�n���#�"���+��5�y0t����D?%<c�3�E"{c��(�P����m#���`Z��r7�y���Z�����|��z=rn(���(D8�4&��i~U��91����+�pS ����_
B����)�=��2B�ǚC����X���F��V�HC��Ν�]^WĊ�{"���'1�,S��mWk_
                                                       �ȘL��g�������%=7Z�=�ܘ��wZ������kc�R7��f�-�]=��=;��(|��H�\5=J��Q7�d_�/,IƓ+<S��%�X1�d�^�_��IX)l(��n,kHK��r3��{jv%/���BOL�@�
                                  ���מ�Y�y�M`1��YL�B�1��d%�ҟ����xj��)�z��'e�-n���
��ڟ��!/�a�����!e7_�}�une'�E��GbG�'Neo4j Admins <admins@neotechnology.com>�?
                                                                           	

!�v}I$�n�Y���_f��~	%$�
	Y���_d��l�{��,)|�7��	���]<���ōX)�g����t맍�0��m�=g�(:XG�ɑ�� j��H5����"�S��ƌ'r�zU}��4�HH)���?�������Z�ø��:Ƶ
�,��--&i�:��U��	Y��H/����(����|ڻ8�C1�Gg����vr�PF.�vBƪ����6�<�v�t�5�*I��*8��%s� +�$���l���R�4����+>�,Z�6�G�\�Bh��R;��fZ�o|~��@���,$̓��A��;C����]n�q�<,dr�rj�Gy���Y������2	��^�+��fcm��l�m�A��0�#��eM���q@�BW���/.�6�XQ�,]�a�{��l*LL'"ٷ��,ô(���sߘ��3�k{eMPx��:qo*z�k�9��������۹X�.>�:Cn��õ��R��v�z����"x*�\ε�Q���m����W���ɋᚯ3��-\��3���Ց�<i����(X<�	��
                                                                  	

�
	Y���_�
              �*]�Ss��a.��?#���.��e��M�F�~�[|�?Dn���ܔ�����K�������R an�x���4��,�-A���ɗ��1��-��2$�[�W5�cC�@��Ȕ�fn�
                                                                                                                 ���dSV��0vs�#zSs�kL���:�P���)@Q�nS���'���3���0uJ������m��ق�G'���6[ʍ�!W��E�&���2񈸾{Ry�%���A2��R�T4~0j���FS=����X��=�ْ���R{*�q׻v�Rl��h�y��@�}��YS�}�G�]��E�n0�I�[a�mW#Y����+�r�SŌ���/��F=9es�%��&���\vk�Fl����Z
                                �6�q�u,����y��x��ʰ������~�͝v�ɤ�
�#�m&����%�%W�H��19i�                                         (a�c�ꗦ6��g�ki�ANu�7¿�Y
�'!��G=Q�Z-�
/(�2�(���ٙ�ܤ��(Q(��m߰�
X<���(������E�)�#��"hT�~�gWf�
                             B'&�H�u�^N+��A�l���<hw���>��0s��<�" 3�3㣩So��z�����F�a�;�-�<��MH�J�;�����<%?.�c!��鱂��U�d���q��cw,u����2}
                                                                                                                                      ,����/H����c3���:��Ws���2���
                    '�H�ż���~o�2s�ܵo�T�����,X���~s�/�m~��j<u9���k��ڱ

�rC�X�G�R����(���K��$�P��9>8]��Y�7�;�aa�3�+���S8�V��wiQ�Ew�� xB�@-�d�k��U�����;����#&��-Caz��t/����PN�kmUݷ�A���Ɍ%J4�B�[��c�;�2sl�cPLP���
                                                                                                                                        ���z����3��r芄[O�9}��sM��d��-"e�#@mS����tD�_d��~� �Ov�f%���A����c�h�k3fZF�
                                                                    |@f&`�z����X<�
                                                                                  	��
	Y���_��ܗ$`9��lNDԭ��0�D�����D\C��p��KR�$�BA�HtBq9����c�(�Z���D�H���n�T��`]��,�SU��_$�$��L���|���mt2�n
                                                                                                            ��;}���$
7X�Ў_�d�+K'��c�����HPy�`��-�U]�����W��,�%�E�`�^��B�Ջ[Q]�8��H���]
�����[�Q�`�0�y�1��%q��4�:�6AŠI^	~M��:�B��E}mIƦ�;�L`��d�z��n��B���$���['o?�h�� ����]&�nJ
�ҋ��N�����]/D��l�Y�S��_�L�4�^�����/S���Z��R-��a�(base) dhankar@dhankar-1:~/.../graph_rag_1$ 



=======================


Linux Uprising Blog



This article explains how to securely add OpenPGP keys and third-party APT repositories on Debian, Ubuntu, and Linux distributions based on these, like Linux Mint, Pop!_OS, Elementary OS and so on, to replace the deprecated apt-key.

When you try to add an APT repository key using apt-key on Debian, Ubuntu and Linux distributions based on these, you'll see the following message: 

"Warning: apt-key is deprecated. Manage keyring files in trusted.gpg.d instead (see apt-key(8))". Some newer Ubuntu versions also show a warning when using a deprecated key: "W: (...) Key is stored in legacy trusted.gpg keyring (/etc/apt/trusted.gpg), see the DEPRECATION section in apt-key(8) for details".

The apt-key man page mentions that the "use of apt-key is deprecated, except for the use of apt-key del in maintainer scripts to remove existing keys from the main keyring". What's more, "apt-key will last be available in Debian 11 and Ubuntu 22.04."

The reason for this change is that when adding an OpenPGP key that's used to sign an APT repository to /etc/apt/trusted.gpg or /etc/apt/trusted.gpg.d, the key is unconditionally trusted by APT on all other repositories configured on the system that don't have a signed-by (see below) option, even the official Debian / Ubuntu repositories. As a result, any unofficial APT repository which has its signing key added to /etc/apt/trusted.gpg or /etc/apt/trusted.gpg.d can replace any package on the system. So this change was made for security reasons (your security).

It's also worth noting that while the apt-key deprecation message says to "manage keyring files in trusted.gpg.d instead", the Debian wiki states otherwise. That's because adding OpenPGP keys to /etc/apt/trusted.gpg and /etc/apt/trusted.gpg.d is equally unsecure, as mentioned above.

You can continue to use apt-key for now as it still works. However, it would be a good idea to start transitioning to utilizing the signed-by option as explained below, especially if you maintain a third-party repository.


So what's the proper, secure way of adding third-party (unofficial) repositories and their OpenPGP signing keys on Debian, Ubuntu, and Linux distributions based on these, like Linux Mint, Pop!_OS, Elementary OS and so on, to replace the deprecated apt-key?

1. Download the APT repository key

According to the Debian wiki, the key should be downloaded over HTTPS to a location only writable by root, for example /usr/share/keyrings. 

The key name should contain a short name describing the repository, followed by archive-keyring. E.g. if the repository is called myrepository, the key file should be named myrepository-archive-keyring.gpg.

The OpenPGP key file can be ascii-armored or not. To verify if a key file is ascii-armored, download the key file and run this command (note that the key extension can be .gpg, .asc, .key, and probably others):

file <repo-key>.gpg
If the output of this command is similar to the following, then the key is ascii-armored:

repo-key.gpg: PGP public key block Public-Key (old)

That being said, this is how to properly, and securely download and add a repository signing key to your system:

For ascii-armored OpenPGP keys
Ezoic
To download using wget and add such an OpenPGP key to your system, use:

wget -O- <https://example.com/key/repo-key.gpg> | gpg --dearmor | sudo tee /usr/share/keyrings/<myrepository>-archive-keyring.gpg

Ezoic

What everything in this command does / means:

wget downloads the key from https://example.com/key/repo-key.gpg and outputs the key to stdout (-O-). Replace the URL here with the URL of the key you want to download and add to your system

gpg --dearmor: the gpg command is the OpenPGP encryption and signing tool; its --dearmor option unpacks the input from an OpenPGP ASCII armor

sudo tee /usr/share/keyrings/<myrepository>-archive-keyring.gpg: as super user (sudo), read the standard input, which in this case is the output provided by gpg --dearmor, and write this to the /usr/share/keyrings/<myrepository>-archive-keyring.gpg file. 

Replace the <myrepository> name with a descriptive name for the repository key you're adding
For example, to add the Signal application APT repository, you'd use:

wget -O- https://updates.signal.org/desktop/apt/keys.asc | gpg --dearmor | sudo tee /usr/share/keyrings/signal-archive-keyring.gpg


Or to use the command given as an example on the Debian wiki (you need to run it as root, e.g. after running sudo -i; it uses curl instead of wget to download the key):

curl <https://example.com/key/repo-key.gpg> | gpg --dearmor > /usr/share/keyrings/<myrepository>-archive-keyring.gpg
Example of using this command to add the Signal APT repository:

curl https://updates.signal.org/desktop/apt/keys.asc | gpg --dearmor > /usr/share/keyrings/signal-archive-keyring.gpg

For non-ascii-armored OpenPGP keys
Download the OpenPGP key using wget and add it to your system using:

wget -O- <https://example.com/key/repo-key.gpg> | sudo tee /usr/share/keyrings/<myrepository-archive-keyring.gpg>
Or to use the command given as an example on the Debian wiki (you need to run it as root, e.g. after running sudo -i):

wget -O /usr/share/keyrings/<myrepository-archive-keyring.gpg> <https://example.com/key/repo-key.gpg>
I did not add an example here because I couldn't find a third-party repository that uses a non ascii-armored OpenPGP key.


To import OpenPGP keys directly from a keyserver to a file in /usr/share/keyrings:
sudo gpg --no-default-keyring --keyring /usr/share/keyrings/<myrepository>-archive-keyring.gpg --keyserver <hkp://keyserver.ubuntu.com:80> --recv-keys <fingerprint>
Instead of hkp://keyserver.ubuntu.com:80, you can use some other key server if you wish.

Example in which we'll import the OpenPGP key of the Linux Uprising Shutter PPA to /usr/share/keyrings/linux-uprising-shutter-archive-keyring.gpg (the fingerprint can be obtained by clicking the green "Technical details about this PPA" link from the PPA page - it's under "Adding this PPA to your system"):

sudo gpg --no-default-keyring --keyring /usr/share/keyrings/linux-uprising-shutter-archive-keyring.gpg --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 1CC3D16E460A94EE17FE581CEA8CACC073C3DB2A

You might also like: How To Keep A Package From Updating In Ubuntu, Debian Or Linux Mint [APT]


2. Add the repository sources.list entry

Third-party repository sources.list entries should be added in the 
/etc/apt/sources.list.d 
directory, and not directly in the 
/etc/apt/sources.list 
file.

Previously, a sources.list file from the 
/etc/apt/sources.list.d 
directory would look like this:

deb https://repository.example.com/debian/ stable main
However, to be able to use the key added under step 1, 
the sources.list entry must now look like this (/etc/apt/sources.list.d/<myrepository.list>):

deb [signed-by=/usr/share/keyrings/<myrepository>-archive-keyring.gpg]
 <https://repository.example.com/debian/ stable main>

It's important to note here that if you also want to add the 
arch=amd64 option together with signed-by, 
you need to separate the two options by a space, like this:

deb [arch=amd64 signed-by=/usr/share/keyrings/<myrepository>-archive-keyring.gpg] <https://repository.example.com/debian/ stable main>

As an example, to add the Signal repository to your Debian / Ubuntu system, 
create a file (as root; for example to open Nano command line text editor with this file: 

sudo nano /etc/apt/sources.list.d/signal.list) 

called signal.list 
in 
/etc/apt/sources.list.d 
with the following contents (assuming you've already downloaded the key as explained above, as 

/usr/share/keyrings/signal-archive-keyring.gpg

):

deb [arch=amd64 signed-by=/usr/share/keyrings/signal-archive-keyring.gpg] https://updates.signal.org/desktop/apt xenial main

Remember to run sudo apt update after adding a new signing key and repository, to update the software sources.

You may also add the repository in the Deb822 file format, but to try and not complicate things even more, I won't explain that here. You can read about that on the Debian wiki.

You may also like: How To Find The Package That Provides A File (Installed Or Not) On Ubuntu, Debian Or Linux Mint


How to remove an already existing OpenPGP key added to the APT trusted keyring (/etc/apt/trusted.gpg or /etc/apt/trusted.gpg.d)

When adding OpenGPG keys as explained above, you'll want to remove the same key from /etc/apt/trusted.gpg or /etc/apt/trusted.gpg.d, in case you've added it there previously. Without doing this, there's no added security benefit.

Removing existing OpenPGP keys from the /etc/apt/trusted.gpg.d directory should be pretty easy. That's because the key filename should be pretty descriptive. For example, the Tor repository gpg key filename from this directory on my system is deb.torproject.org-keyring.gpg

So to get rid of already existing keys added to /etc/apt/trusted.gpg.d, all you have to do is remove the key files. You need to do this as root. So either open the file manager of your choice as root, using admin:// (for example, to open a location as root in Nautilus, press Ctrl + L so you can type in its address bar, and type admin:///etc/apt/trusted.gpg.d), or remove them from the command line, using:

sudo rm /etc/apt/trusted.gpg.d/<myrepository-keyring.gpg>
The instructions below also work for removing keys from the /etc/apt/trusted.gpg.d directory.

As for removing APT gpg keys stored in /etc/apt/trusted.gpg, things are a bit more complicated. Use the following command to list all APT OpenPGP keys imported in both /etc/apt/trusted.gpg and /etc/apt/trusted.gpg.d:

apt-key list
The keys stored in /etc/apt/trusted.gpg should be listed at the top, followed by the keys from the /etc/apt/trusted.gpg.d directory. You'll need to inspect the key uid in order to figure out the key that you want to remove. Usually, the uid should show the company or user that signed the key, followed by their email address.

Keys from /etc/apt/trusted.gpg are listed by apt-key list like this (example):

pub   rsa4096 2016-04-22 [SC]

      B9F8 D658 297A F3EF C18D  5CDF A2F6 83C5 2980 AECF

uid           [ unknown] Oracle Corporation (VirtualBox archive signing key) <info@virtualbox.org>

sub   rsa4096 2016-04-22 [E]


The key ID is the last 8 characters of the GPG key's fingerprint (so in this example, that's 2980AECF).

To delete a key (from either /etc/apt/trusted.gpg or /etc/apt/trusted.gpg.d), you can now use:

sudo apt-key del <KEY-ID>
For example, to delete the key from the example above, you'd use:

sudo apt-key del 2980AECF
You might like: How To List All Packages In A Repository On Ubuntu, Debian Or Linux Mint [APT]

References:

https://wiki.debian.org/DebianRepository/UseThirdParty
https://askubuntu.com/a/1307181/1149075
https://zebnemeth.wordpress.com/2021/01/15/install-signal-desktop-using-gpg/
https://github.com/docker/docker.github.io/issues/11625
Thanks to u/ZebNemeth for the suggestion!

Share This:Mastodon Twitter Diaspora Reddit Telegram WhatsApp
How To Install GNOME 40 On Ubuntu 21.04 Hirsute Hippo For Testing Purposes [PPA]
Install macOS Big Sur Or Catalina In A Virtual Machine Using Docker-OSX
Remap Keyboard And Mouse Buttons On Linux With The New Key Mapper GUI (Supports X11 And Wayland)
Please post civil and on-topic comments. Commenting guidelines.

Ezoic
Recent Posts
normcap
NormCap: Screen Capture Tool For Text Using OCR
pipx logo
How To Fix pipx: Fatal Error From pip Prevented Installation / No Module Named pip
Upscayl ai image upscaler
Upscayl AI Image Upscaler 2.5 Adds Option To Import Custom Models, New Settings Tab
gpu screen recorder for linux
GPU Screen Recorder For Linux Adds Support For AMD And Intel GPUs
hanabi gnome live wallpaper
Hanabi Is A Live Wallpaper For GNOME Desktop
reminders rememberance Linux GTK4 Microsoft To Do sync
Reminders Is A GTK4 To-Do List App That Syncs With Microsoft To Do
Join us on Telegram

Follow us on Twitter



Editor's Picks
How To Enable Hardware Accelerated Video Decode In Google Chrome, Brave, Vivaldi And Opera Browsers On Debian, Ubuntu Or Linux Mint
Install macOS Big Sur Or Catalina In A Virtual Machine Using Docker-OSX
Create A Bootable USB Drive By Simply Copying The ISO To The USB With Ventoy (Linux And Windows)
How To Boot To Console (Text) Mode Using Debian / Ubuntu, Fedora, Arch Linux / Manjaro And More
FFmpeg: Extract Audio From Video In Original Format Or Converting It To MP3 Or Ogg Vorbis
How To Install DaVinci Resolve 18 In Ubuntu, Linux Mint Or Debian (Generate DEB Package)
How To Change The GRUB Boot Order Or Default Boot Entry In Ubuntu, Linux Mint, Debian, Or Fedora With Grub Customizer
New Oracle Java 11 Installer For Ubuntu Or Linux Mint (Using Local Oracle Java .tar.gz)
How To Fix `Could not get lock /var/lib/dpkg/lock - open (11 Resource temporarily unavailable)` Errors
How To Mount OneDrive In Linux Using Rclone (Supports Business And Personal Accounts)
Linux Uprising
About
Privacy Policy
Terms of Service
Cookie Information
Cookie Settings
License
Creative Commons Attribution 4.0 International License

The registered trademark Linux® is used pursuant to a sublicense from the Linux Foundation, the exclusive licensee of Linus Torvalds, owner of the mark on a world-wide basis.
Blog Archive

Blog Archive
Blog focused on Linux and FOSS.

```bash

(base) dhankar@dhankar-1:~/.../graph_rag_1$ wget -O - https://debian.neo4j.com/neotechnology.gpg.key | sudo apt-key add -
--2025-05-25 19:04:50--  https://debian.neo4j.com/neotechnology.gpg.key
Resolving debian.neo4j.com (debian.neo4j.com)... 108.138.192.72, 108.138.192.27, 108.138.192.68, ...
Connecting to debian.neo4j.com (debian.neo4j.com)|108.138.192.72|:443... Warning: apt-key is deprecated. Manage keyring files in trusted.gpg.d instead (see apt-key(8)).
connected.
HTTP request sent, awaiting response... 200 OK
Length: 3905 (3.8K) [application/pgp-keys]
Saving to: ‘STDOUT’

-                                   100%[=================================================================>]   3.81K  --.-KB/s    in 0s      

2025-05-25 19:04:50 (10.2 MB/s) - written to stdout [3905/3905]

OK
(base) dhankar@dhankar-1:~/.../graph_rag_1$ sudo apt-get install neo4j -y
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
E: Unable to locate package neo4j
(base) dhankar@dhankar-1:~/.../graph_rag_1$ sudo apt-get update
Get:1 file:/var/cuda-repo-ubuntu1804-11-8-local  InRelease [1,575 B]
Get:1 file:/var/cuda-repo-ubuntu1804-11-8-local  InRelease [1,575 B]
Hit:2 https://packages.microsoft.com/repos/azure-cli jammy InRelease                   
Hit:3 https://packages.microsoft.com/repos/code stable InRelease                                                          
Hit:4 http://dl.google.com/linux/chrome/deb stable InRelease                                                              
Get:5 https://debian.neo4j.com stable InRelease [44.2 kB]                                       
Err:5 https://debian.neo4j.com stable InRelease                                                  
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 59D700E4D37F5F19
Hit:6 http://archive.linux.duke.edu/ubuntu jammy InRelease                    
Hit:7 http://archive.linux.duke.edu/ubuntu jammy-updates InRelease            
Hit:8 http://archive.linux.duke.edu/ubuntu jammy-backports InRelease
Hit:9 http://archive.linux.duke.edu/ubuntu jammy-security InRelease
Hit:10 https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64  InRelease
Reading package lists... Done
W: GPG error: https://debian.neo4j.com stable InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY 59D700E4D37F5F19
E: The repository 'https://debian.neo4j.com stable InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.

```


======================================

wget -O - https://debian.neo4j.com/neotechnology.gpg.key | sudo gpg --dearmor -o /etc/apt/keyrings/neotechnology.gpg echo 'deb [signed-by=/etc/apt/keyrings/neotechnology.gpg] https://debian.neo4j.com stable latest' | sudo tee -a /etc/apt/sources.list.d/neo4j.list sudo apt-get update

### TODO -- https://stackoverflow.com/questions/68992799/warning-apt-key-is-deprecated-manage-keyring-files-in-trusted-gpg-d-instead
