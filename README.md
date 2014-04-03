Slumber DB - Key Value Store for JSON / REST
=========

The JSON database for REST and Websocket storage.


This is an effort to write key / value stores for JSR-107 RI
and one for HazelCast MapStore.

The goals are simple. Write a MySQL, LevelDB, LMDB, and RocksDB key / value store
for Java serialization and JSON for HazelCast MapStore and JSR-107 RI Cache Stores.

The MySQL version will use Boon JSON serialization and kryo.


Boon is the fastest JSON serialization.
Kryo is the fastest Java serialization.

The plan is to use leveldbjni for the leveldb implementation, and later Vertx for a storage replica set.



**LevelDB** is a lightweight database by **Google** modeled after BigTable tablet store.
LevelDB gets used by Chrome.

**RocksDB** is a server-side version of LevelDB by **Facebook** that reportedly is more scalable.

**MySQL** is well MySQL.

**LMDB** is an fast, compact key/value store which gets used by the OpenLDAP Project.


**Kryo** is the fastest and efficient object graph serialization for the JVM.



See Kryo at: https://github.com/EsotericSoftware/kryo

See Boon at: https://github.com/RichardHightower/boon

See LevelDBJNI at: https://github.com/fusesource/leveldbjni

See LevelDB at: https://code.google.com/p/leveldb/

See RocksDB at: http://rocksdb.org/

See RocksDBJNI at: https://github.com/fusesource/rocksdbjni

See LMDB: http://symas.com/mdb/

See LMDBJNI: https://github.com/chirino/lmdbjni

Special thanks to Hiram Chirino for writing leveldbjni, lmdbjni and rocksdbjni.
Without Hiram, Apache Apollo bad-ass, none of this would be possible.

https://github.com/chirino


Special thanks to Tim Fox for writing Vertx. Tim is the author of Vertx which leads the charts for fast JVM based web servers.
Vertx is so much more than a web server.

https://github.com/purplefox

http://www.infoq.com/news/2011/12/apollo-benchmarks


Rick Hightower works on JSR-107 and JSR-347 as well as Boon
which has an in-memory query engine, and a fast JSON parser/serializer.
