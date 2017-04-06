[root@cluster2node1 unlimitedjce]$ kadmin.local -q "addprinc pcontop"

[root@cluster2node1 unlimitedjce]$ su pcontop

[pcontop@cluster2node1 unlimitedjce]$ kinit # test password.

[pcontop@cluster2node1 unlimitedjce]$ klist
Ticket cache: KEYRING:persistent:1000:1000
Default principal: pcontop@COMPWIRE.LOCAL