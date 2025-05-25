### TODO -- https://stackoverflow.com/questions/68992799/warning-apt-key-is-deprecated-manage-keyring-files-in-trusted-gpg-d-instead


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

#### Install - Neo4j Ubuntu Local Install 

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
