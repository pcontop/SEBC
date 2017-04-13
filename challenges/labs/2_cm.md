[root@cluster2node2 ~]# ls /etc/yum.repos.d
CentOS-Base.repo  CentOS-Debuginfo.repo  CentOS-Media.repo    CentOS-Vault.repo
CentOS-CR.repo    CentOS-fasttrack.repo  CentOS-Sources.repo  cloudera-manager.repo
[root@cluster2node2 ~]#

/usr/share/cmf/schema/scm_prepare_database.sh \
mysql -h cluster2node1.compwire.local -u root -p \
--scm-host cluster2node2.compwire.local scm scm scm