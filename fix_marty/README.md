# Fix Marty's files errors (server side)

## 1. Client

### A. pack/root/npcllist.txt

*Find*
 - ```20221	bear```

*Replace*
 - ```20221	bear_mount```

### B. pack/ym_npc/ymir work/npc

*Delete*
 - ```bear```



## 2. DataBase

```sql
UPDATE player.mob_proto SET folder='spider_spawn' WHERE vnum=2095;
UPDATE player.mob_proto SET folder='yamachun_boss' WHERE vnum=6091;
UPDATE player.mob_proto SET folder='yamachun_boss' WHERE vnum=4401;
UPDATE player.mob_proto SET folder='yamachun_boss' WHERE vnum=4411;
UPDATE player.mob_proto SET folder='yamachun_boss' WHERE vnum=6417;
UPDATE player.mob_proto SET folder='' WHERE vnum=20221;
UPDATE player.mob_proto SET folder='pig_young1' WHERE vnum=34017;
UPDATE player.mob_proto SET folder='dog_young1' WHERE vnum=34018;
UPDATE player.mob_proto SET folder='tiger_young1' WHERE vnum=34019;
UPDATE player.mob_proto SET folder='lion_young1' WHERE vnum=34020;
```

