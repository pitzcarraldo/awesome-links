# awesome-links

### How to name Java Classes
- https://stackoverflow.com/questions/1866794/naming-classes-how-to-avoid-calling-everything-a-whatevermanager
- http://www.bright-green.com/blog/2003_02_25/naming_java_classes_without_a.html

### Impl Classes is Anti Pattern
- https://octoperf.com/blog/2016/10/27/impl-classes-are-evil/
- https://rrees.me/2009/01/31/programming-to-interfaces-anti-pattern/
- http://stackoverflow.com/questions/5095955/service-s-new-serviceimpl-why-you-are-doing-that
- http://stackoverflow.com/questions/2814805/java-interfaces-implementation-naming-convention
- http://stackoverflow.com/questions/541912/interface-naming-in-java
- http://stackoverflow.com/questions/17275344/java-interface-naming-conventions
- https://blog.jooq.org/tag/naming-conventions/

### Reset IntelliJ License
```sh
rm -rf ~/Library/Preferences/IntelliJIdea*/eval/*.key
rm -rf ~/Library/Preferences/IntelliJIdea*/options/options.xml
```

### Inversion of Control & Dependency Injection
- http://martinfowler.com/bliki/InversionOfControl.html
  - 번역 : http://www.egovframe.org/wiki/doku.php?id=egovframework:rte:fdl:ioc_container:inversion_of_control
- http://martinfowler.com/articles/injection.html
  - 번역 : http://javacan.tistory.com/entry/120

### Responsive Image
- http://abhishek-tiwari.com/post/responsive-image-as-service-rias
- http://imageresizing.net/blog/2013/effortless-responsive-images
- https://github.com/carsonmcdonald/ServerSideResponsiveImageExample
- http://iipimage.sourceforge.net/2012/08/responsive-images-using-iipimage/
- https://github.com/thumbor/thumbor
- http://imageresizing.net/
- http://adaptive-images.com/
- http://www.picarisplatform.com/picaris-image-server-platform
- http://www.pixtulate.com/


### Comparing ClickHouse, Druid, Pinot
||ClickHouse|Druid|Pinot|
|--- |--- |--- |--- |
|Ecosystem|Matured|Matured|Incubating|
|References|Many|Many|Some big companies (LinkedIn, Uber)|
|Hadoop Friendly|No|Yes|Yes|
|Support Join|NativeBroadcast join only (right side data should fit in memory)|NativeBroadcast join only (right side data should fit in memory)|Using Prestojoining data from Pinot to other data sources not in Pinot|
|Performance|Fast|Fast|Faster than others|
|Setup / Management|Simple(Single Type Node)|Complex than ClickHouse(Depends on PostgresQL, Zookeeper)|Complex than ClickHouse(Depends on Helix, Zookeeper)|
|Storage|Local Storage/S3|HDFS/S3|HDFS/S3|
|Scalability|no auto sharding|background process rebalance the data||
|Presto Connector|Community|Official|Official|
|System level monitoring|Community Prometheus Exporter|ExporterImply service offers monitoring platform (for fee)|3rd party prometheus monitoring|

#### References
*   Comparing these 3 db
    *   [https://medium.com/@leventov/comparison-of-the-open-source-olap-systems-for-big-data-clickhouse-druid-and-pinot-8e042a5ed1c7](https://medium.com/@leventov/comparison-of-the-open-source-olap-systems-for-big-data-clickhouse-druid-and-pinot-8e042a5ed1c7)
    *   [https://docs.google.com/document/d/1GiB8zoiJ4Qs10A1LdIr6lJGWTfk-0ElU8aJbejomstY/edit](https://docs.google.com/document/d/1GiB8zoiJ4Qs10A1LdIr6lJGWTfk-0ElU8aJbejomstY/edit)
*   Druid supports JOIN: [https://imply.io/post/apache-druid-joins](https://imply.io/post/apache-druid-joins)
*   Pinot Use Case  
    *   [https://engineering.linkedin.com/blog/topic/pinot](https://engineering.linkedin.com/blog/topic/pinot)
    *   [https://eng.uber.com/engineering-sql-support-on-apache-pinot/](https://eng.uber.com/engineering-sql-support-on-apache-pinot/)
*   Discussions
    *   [https://news.ycombinator.com/item?id=22868286](https://news.ycombinator.com/item?id=22868286)
    *   [https://news.ycombinator.com/item?id=19825566](https://news.ycombinator.com/item?id=19825566)
*   TimeScale DB(TimeSeries DB based on PostgresQL):  [https://www.timescale.com/](https://www.timescale.com/)
