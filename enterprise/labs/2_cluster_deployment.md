{
  "timestamp" : "2017-04-06T21:02:23.349Z",
  "clusters" : [ {
    "name" : "pcontop",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "333447168"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_enable_impersonation",
            "value" : "false"
          }, {
            "name" : "hiveserver2_java_heapsize",
            "value" : "333447168"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "4117757952"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "693"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "cluster2node1.compwire.local"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0078d2571590911d638f00427dcad19e",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-08295c96458079a2d79e3095b2c31ef4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6894d25855d111dcd2f87d859da877e3",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2a18cb56-a1d7-45d8-9e54-bec696e84af7"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-9333b0c4702738f4f76da932ab7a858f",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-a6b5a6f149451e142af9a3016a394065",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "780dd554-30b4-469d-b4f5-be70b9a01d62"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-0078d2571590911d638f00427dcad19e",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "echdfqxqjt5l92eq0mi2xoej8"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-0078d2571590911d638f00427dcad19e",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1luzxp1efiruo4vpcp7zyvb1k"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "333447168"
          } ]
        } ],
        "items" : [ {
          "name" : "enableSecurity",
          "value" : "true"
        } ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-0078d2571590911d638f00427dcad19e",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "es1cvd6p7o0dmeztd5uqw2jzi"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-08295c96458079a2d79e3095b2c31ef4",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8xduhjccohgmi6jvvlu3gxsej"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-9333b0c4702738f4f76da932ab7a858f",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b8m7pbk318x2qahyvrdoo925u"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "auth_backend",
          "value" : "desktop.auth.backend.AllowAllBackend"
        }, {
          "name" : "database_host",
          "value" : "cluster2node1.compwire.local"
        }, {
          "name" : "database_password",
          "value" : "hue"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-0078d2571590911d638f00427dcad19e"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "sentry_service",
          "value" : "sentry"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-0078d2571590911d638f00427dcad19e",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "83arr7bntd1t7go5qwgy9b0xd"
          }, {
            "name" : "secret_key",
            "value" : "wBR9fPM1E06ThJhIT26SPTs8tgCl3L"
          } ]
        }
      }, {
        "name" : "hue-KT_RENEWER-0078d2571590911d638f00427dcad19e",
        "type" : "KT_RENEWER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1q5848vhebfo47qmg2j93larp"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "cluster2node1.compwire.local"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "333447168"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-0078d2571590911d638f00427dcad19e",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8ca45vw261jcaqym6g20m2dci"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "4"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "333447168"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "rm_cpu_shares",
            "value" : "1800"
          }, {
            "name" : "rm_io_weight",
            "value" : "900"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "1"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "4872"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "333447168"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5951"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "1"
          } ]
        } ],
        "items" : [ {
          "name" : "hadoop_secure_web_ui",
          "value" : "true"
        }, {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "FGt2LJqYoDG30idSTWoodvKmxljllI"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-0078d2571590911d638f00427dcad19e",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "57xsndc24nyobr6sop4bkjjgm"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-08295c96458079a2d79e3095b2c31ef4",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8fldt9wn7747ltzjdxw4vxfh4"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-6894d25855d111dcd2f87d859da877e3",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2a18cb56-a1d7-45d8-9e54-bec696e84af7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7pd0sdu1d3hr0e44mrmafu7vz"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-9333b0c4702738f4f76da932ab7a858f",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7lz8k1egcsbf3tny59uq82qp5"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-0078d2571590911d638f00427dcad19e",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "53"
          }, {
            "name" : "role_jceks_password",
            "value" : "64k3w18zfa434xqjbk4kf14z1"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "333447168"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3806568448"
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/dfs/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "333447168"
          }, {
            "name" : "role_config_suppression_namenode_java_heapsize_minimum_validator",
            "value" : "true"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "333447168"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_encrypt_data_transfer_algorithm",
          "value" : "AES/CTR/NoPadding"
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "rSTkpbh3Vmwnju3mWTmqbenFh3tgc1"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "fxh6CgB7lu5YnlhSL5Qpa57CCFLlq8"
        }, {
          "name" : "hadoop_secure_web_ui",
          "value" : "true"
        }, {
          "name" : "hadoop_security_authentication",
          "value" : "kerberos"
        }, {
          "name" : "hadoop_security_authorization",
          "value" : "true"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "JONeBtRsq7DssIx7MQvDr7r0FuKTNf"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-0078d2571590911d638f00427dcad19e",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-08295c96458079a2d79e3095b2c31ef4",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "58cmu2vbdm0gxr4pbi5g7zz30"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-6894d25855d111dcd2f87d859da877e3",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2a18cb56-a1d7-45d8-9e54-bec696e84af7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "enwsip6ylgcfohm1mfymzpufm"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-9333b0c4702738f4f76da932ab7a858f",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "cx5po8bv764yn07ftupgq55kl"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-a6b5a6f149451e142af9a3016a394065",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "780dd554-30b4-469d-b4f5-be70b9a01d62"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "65vism269lntz4myv6mgw7oud"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-0078d2571590911d638f00427dcad19e",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e4bndavldfqpnc4thr3crvuj0"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-9333b0c4702738f4f76da932ab7a858f",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "96xhfhjdeavlcs3walba5nw5e"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-08295c96458079a2d79e3095b2c31ef4",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4ek36mlwbf4149nehze6f7x95"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-9333b0c4702738f4f76da932ab7a858f",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b700v44va3iys0kq6wtr37nno"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-a6b5a6f149451e142af9a3016a394065",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "780dd554-30b4-469d-b4f5-be70b9a01d62"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6a4ivepog8jqfam1k4qxo0wpd"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-0078d2571590911d638f00427dcad19e",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "pcontopservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "pcontopservice1"
          }, {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "528qoyh7ik0xje2qdvrwykfiu"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-9333b0c4702738f4f76da932ab7a858f",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "pcontopservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "pcontopservice1"
          }, {
            "name" : "namenode_id",
            "value" : "68"
          }, {
            "name" : "role_jceks_password",
            "value" : "6b9qrvruf0i995fs141tm8dlo"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    }, {
      "name" : "sentry",
      "type" : "SENTRY",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SENTRY_SERVER",
          "items" : [ {
            "name" : "sentry_server_java_heapsize",
            "value" : "268435456"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "sentry_server_database_host",
          "value" : "cluster2node1.compwire.local"
        }, {
          "name" : "sentry_server_database_password",
          "value" : "sentry"
        }, {
          "name" : "sentry_service_admin_group",
          "value" : "hive,impala,hue,solr,kafka,pcontop"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "sentry-GATEWAY-08295c96458079a2d79e3095b2c31ef4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-6894d25855d111dcd2f87d859da877e3",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2a18cb56-a1d7-45d8-9e54-bec696e84af7"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-9333b0c4702738f4f76da932ab7a858f",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-GATEWAY-a6b5a6f149451e142af9a3016a394065",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "780dd554-30b4-469d-b4f5-be70b9a01d62"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "sentry-SENTRY_SERVER-0078d2571590911d638f00427dcad19e",
        "type" : "SENTRY_SERVER",
        "hostRef" : {
          "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2omoyl5y8ea5c6hor5sfx1xop"
          } ]
        }
      } ],
      "displayName" : "Sentry"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568",
    "ipAddress" : "192.168.100.171",
    "hostname" : "cluster2node1.compwire.local",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2bab254e-5d20-4ca2-ba9c-949db84c18fb",
    "ipAddress" : "192.168.100.176",
    "hostname" : "cluster2node2.compwire.local",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "381b76be-0cbc-4d04-951f-d8edb35fcfe0",
    "ipAddress" : "192.168.100.173",
    "hostname" : "cluster2node3.compwire.local",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "780dd554-30b4-469d-b4f5-be70b9a01d62",
    "ipAddress" : "192.168.100.174",
    "hostname" : "cluster2node4.compwire.local",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "2a18cb56-a1d7-45d8-9e54-bec696e84af7",
    "ipAddress" : "192.168.100.175",
    "hostname" : "cluster2node5.compwire.local",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "Minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "a5162e68d476a071f56370eebc8e4d37ad9a212e706095162b41db23f1832838",
    "pwSalt" : -2163523717172393961,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-0078d2571590911d638f00427dcad19e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "7ecfcb43dd158cc200d0b7f3d4fea6c2535b8d89f2fcde4f486614b0e6ebfc67",
    "pwSalt" : 6125211835794013604,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-0078d2571590911d638f00427dcad19e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "b7651315615acd7f3be93960d852545520a783800b79b56770298f983510ba6a",
    "pwSalt" : -1788944796194570508,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-0078d2571590911d638f00427dcad19e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "0c1b5d176fed66d8f1181ebe16df93e1b1b51e6ba23b17149efae3629e6bd509",
    "pwSalt" : 7015582798952727149,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-0078d2571590911d638f00427dcad19e",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "eb94f8778fea3d00dd6096621e885e1f4d1b7e2f1a317921e2f659510f5804ce",
    "pwSalt" : 5924363449816543517,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "4658d817d23a363b78e9d81c4d844f5fbe53aa903169a7249f1e5c6946533647",
    "pwSalt" : 3363406210100512577,
    "pwLogin" : true
  }, {
    "name" : "pcontop",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "1fd376c7de27ccdbbf47a4e0e0efcea67c2f5d602de4c8a04fe5b7e515500f8d",
    "pwSalt" : -2248462356599395546,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.10.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170319-2001",
    "gitHash" : "f226435f6fa5f545543c00245900ae43bea7a29c",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "cluster2node1.compwire.local"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ {
        "name" : "ssl_client_truststore_location",
        "value" : "/usr/java/jdk1.7.0_67-cloudera/jre/lib/security/jssecacerts"
      }, {
        "name" : "ssl_client_truststore_password",
        "value" : "passw0rd"
      } ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-0078d2571590911d638f00427dcad19e",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "8tn4xhj8fv6h6ng94b2veu41z"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-0078d2571590911d638f00427dcad19e",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ai39xjbgz961evrin29t90zp7"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-0078d2571590911d638f00427dcad19e",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "14dwmq8rdrm37jpjzfiy4wg44"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-0078d2571590911d638f00427dcad19e",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "4vg67y6r8u7mrm502v571t4kd"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-0078d2571590911d638f00427dcad19e",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "d815c0b0-ffb1-49e2-96df-67bb8f94e568"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "f578uhvrnrx1amwm8mf5lyo4j"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "AD_USE_SIMPLE_AUTH",
      "value" : "false"
    }, {
      "name" : "AGENT_TLS",
      "value" : "true"
    }, {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/22/2012 14:20"
    }, {
      "name" : "KDC_ADMIN_PASSWORD",
      "value" : "BQIAAABIAAIADkNPTVBXSVJFLkxPQ0FMAAxjbG91ZGVyYS1zY20ABWFkbWluAAAAAVjmQEQBABcAEIhG9+ruj7EXrQa92DC3WGwAAAAB"
    }, {
      "name" : "KDC_ADMIN_USER",
      "value" : "cloudera-scm/admin@COMPWIRE.LOCAL"
    }, {
      "name" : "KDC_HOST",
      "value" : "cluster2node1.compwire.local"
    }, {
      "name" : "KEYSTORE_PASSWORD",
      "value" : "passw0rd"
    }, {
      "name" : "KEYSTORE_PATH",
      "value" : "/opt/cloudera/security/pki/agent.jks"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "NOT_ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,http://192.168.100.171/cdh5.10.1/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    }, {
      "name" : "SECURITY_REALM",
      "value" : "COMPWIRE.LOCAL"
    }, {
      "name" : "TRUSTSTORE_PASSWORD",
      "value" : "passw0rd"
    }, {
      "name" : "TRUSTSTORE_PATH",
      "value" : "/usr/java/jdk1.7.0_67-cloudera/jre/lib/security/jssecacerts"
    }, {
      "name" : "WEB_TLS",
      "value" : "true"
    } ]
  }
}