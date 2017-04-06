0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170406152121_f4028c48-e760-40d6-b39f-616f3d7b7265): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406152121_f4028c48-e760-40d6-b39f-616f3d7b7265); Time taken: 1.327 seconds
INFO  : Executing command(queryId=hive_20170406152121_f4028c48-e760-40d6-b39f-616f3d7b7265): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406152121_f4028c48-e760-40d6-b39f-616f3d7b7265); Time taken: 0.807 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (3.767 seconds)
0: jdbc:hive2://localhost:10000/default>

[root@cluster2node1 security]# kinit george
Password for george@COMPWIRE.LOCAL:
[root@cluster2node1 security]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/fdqn@REALM.COM
scan complete in 3ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/fdqn@REALM.COM
17/04/06 15:40:31 [main]: ERROR transport.TSaslTransport: SASL negotiation failure
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - LOOKING_UP_SERVER)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.thrift.transport.TSaslClientTransport.handleSaslStartMessage(TSaslClientTransport.java:94)
        at org.apache.thrift.transport.TSaslTransport.open(TSaslTransport.java:271)
        at org.apache.thrift.transport.TSaslClientTransport.open(TSaslClientTransport.java:37)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:52)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:49)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1920)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport.open(TUGIAssumingTransport.java:49)
        at org.apache.hive.jdbc.HiveConnection.openTransport(HiveConnection.java:202)
        at org.apache.hive.jdbc.HiveConnection.<init>(HiveConnection.java:167)
        at org.apache.hive.jdbc.HiveDriver.connect(HiveDriver.java:105)
        at java.sql.DriverManager.getConnection(DriverManager.java:571)
        at java.sql.DriverManager.getConnection(DriverManager.java:187)
        at org.apache.hive.beeline.DatabaseConnection.connect(DatabaseConnection.java:146)
        at org.apache.hive.beeline.DatabaseConnection.getConnection(DatabaseConnection.java:211)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1501)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1396)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hive.beeline.ReflectiveCommandHandler.execute(ReflectiveCommandHandler.java:52)
        at org.apache.hive.beeline.BeeLine.execCommandWithPrefix(BeeLine.java:1128)
        at org.apache.hive.beeline.BeeLine.dispatch(BeeLine.java:1167)
        at org.apache.hive.beeline.BeeLine.execute(BeeLine.java:1003)
        at org.apache.hive.beeline.BeeLine.begin(BeeLine.java:915)
        at org.apache.hive.beeline.BeeLine.mainWithInputRedirection(BeeLine.java:511)
        at org.apache.hive.beeline.BeeLine.main(BeeLine.java:494)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)
Caused by: GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - LOOKING_UP_SERVER)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 35 more
Caused by: KrbException: Server not found in Kerberos database (7) - LOOKING_UP_SERVER
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 38 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 44 more
Unknown HS2 problem when communicating with Thrift server.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://localhost:10000/default;principal=hive/fdqn@REALM.COM: GSS initiate failed (state=08S01,code=0)
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/cluster2node1.compwire.local@COMPWIRE.LOCAL;
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/cluster2node1.compwire.local@COMPWIRE.LOCAL;
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170406154242_9eb3a653-35cf-465d-824e-b85ecf85b011): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406154242_9eb3a653-35cf-465d-824e-b85ecf85b011); Time taken: 0.134 seconds
INFO  : Executing command(queryId=hive_20170406154242_9eb3a653-35cf-465d-824e-b85ecf85b011): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406154242_9eb3a653-35cf-465d-824e-b85ecf85b011); Time taken: 0.252 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.551 seconds)
0: jdbc:hive2://localhost:10000/default> exit
. . . . . . . . . . . . . . . . . . . .> ;
Error: Error while compiling statement: FAILED: ParseException line 1:0 cannot recognize input near 'exit' '<EOF>' '<EOF>' (state=42000,code=40000)
0: jdbc:hive2://localhost:10000/default> [root@cluster2node1 security]# kinit ferdinand
Password for ferdinand@COMPWIRE.LOCAL:
kinit: Password incorrect while getting initial credentials
[root@cluster2node1 security]# kinit ferdinand
Password for ferdinand@COMPWIRE.LOCAL:
[root@cluster2node1 security]#  !connect jdbc:hive2://localhost:10000/default;principal=hive/cluster2node1.compwire.local@COMPWIRE.LOCAL;
-bash: !connect: event not found
[root@cluster2node1 security]# beeline
Beeline version 1.1.0-cdh5.10.1 by Apache Hive
beeline>  !connect jdbc:hive2://localhost:10000/default;principal=hive/cluster2node1.compwire.local@COMPWIRE.LOCAL;
scan complete in 3ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/cluster2node1.compwire.local@COMPWIRE.LOCAL;
Connected to: Apache Hive (version 1.1.0-cdh5.10.1)
Driver: Hive JDBC (version 1.1.0-cdh5.10.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170406154343_2c7ea72f-fc9d-4156-8a61-fbdb815aa6f9): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170406154343_2c7ea72f-fc9d-4156-8a61-fbdb815aa6f9); Time taken: 0.841 seconds
INFO  : Executing command(queryId=hive_20170406154343_2c7ea72f-fc9d-4156-8a61-fbdb815aa6f9): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170406154343_2c7ea72f-fc9d-4156-8a61-fbdb815aa6f9); Time taken: 0.573 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (1.641 seconds)
0: jdbc:hive2://localhost:10000/default>
