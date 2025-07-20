path: /etc/exports

content:
/data *(rw,sync,no_subtree_check)
/data/ELK *(rw,sync,no_root_squash,no_all_squash)
/mnt/data/elasticsearch 192.168.101.0/24(rw,sync,no_subtree_check,no_root_squash)
/mongo-data 192.168.101.0/24(rw,sync,no_subtree_check,no_root_squash)
