[Community Weekly Update] 2019-10-07 ~ 2019-10-18

This is the first weekly community update, which helps you quickly capture Pulsar's highlights and spot trends over last week, meanwhile strengthen the communication and connection within the Pulsar family.

## Pulsar Development

- [CI]  ASF Jenkins is still in a flaky state. There is still a huge backlog of pull requests to be merged due to Jenkins issue. Ali Ahmed drove the efforts looking into different CI options to address the problem [1].

- [PIP] [metadata] Matteo proposed introducing pluggable metadata interface in PIP-45 (https://github.com/apache/pulsar/wiki/PIP-45:-Pluggable-metadata-interface). It is a great movement to support other metadata storage besides zookeeper. The first pull request was merged [2].

- [DOC] [connector] Yu Liu (@Anonymitaet) continues contributing to the documentation for built-in connectors (https://github.com/apache/pulsar/issues/5015). Hope we can fill the documentation gap soon. Those changes are available in the latest version of documentation (http://pulsar.apache.org/docs/en/next/io-connectors/). 

[1] https://mail-archives.apache.org/mod_mbox/pulsar-dev/201910.mbox/%3CCANcJaZucPz%2BinJ%3DaVNVM0f-1qEJ_J%3DRcamkj8v6XeiqY4Thv_A%40mail.gmail.com%3E

[2] https://mail-archives.apache.org/mod_mbox/pulsar-dev/201910.mbox/%3CCA%2BJmKXYakGKi9d7j%2Bavo4WW%3DRu3BY-ZUpLDW3RLeAic-NVN1sA%40mail.gmail.com%3E
 
## Notable Bug Fix

- [Broker] Deduplication may drop messages if there is an error persisting to bookkeeper. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/issues/5218

- [Broker] Race condition while triggering message redelivery after an ack-timeout event. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5276

- [Broker] If a cursor is not durable, close dispatcher when all consumers are removed from subscription. (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5340

- [TIEREDSTORAGE] Don't require both region and endpoint to be specified (Fixed, Release: 2.4.2 / 2.5.0)

    https://github.com/apache/pulsar/pull/5355

## Ecosyste

- Pulsar + Flink
  
    The discussion of adding Pulsar connector to Flink main repo continues in Flink mailing list. The contributions include Sink Connector, Source Connector and Catalog integration. FLIP-72 is the umbrella for the whole contribution. 

    https://cwiki.apache.org/confluence/display/FLINK/FLIP-72%3A+Introduce+Pulsar+Connector

- Pulsar + Skywalking
  
    The integration of Pulsar and Skywalking was completed [3]. The Pulsar plugin is now available in Skywalking main repo and will be released in its 6.5.0 release. Kudos to Penghui and the Skywalking community. Penghui also wrote a tutorial about using Skywalking to trace Pulsar messages [4]. 

    [3] https://github.com/apache/skywalking/pull/3476

    [4] https://medium.com/streamnative/use-apache-skywalking-to-trace-apache-pulsar-messages-b543ac253053

- Pulsar .NET Client

    Many features landed in the Pulsar .NET Client in the past 2 weeks (https://github.com/fsharplang-ru/pulsar-client-dotnet) 

  - Oct 16th: 0.6.0 released with consumer seek support.
  
  - Oct 15th: 0.5.0 released with compacted topics support.
  
  - Oct 8th: 0.4.0 released with key/value properties support.
  
  .NET client package is available at: https://www.nuget.org/packages/Pulsar.Client

- Pulsar Express
  
    Pulsar Express released 0.5.0 on Oct 13 with many features like broker health check, namespace creation and deletion, topic creation, and son on.

## Event/News

- [HUG] Special Apache Pulsar Meetup chez OVH (Paris 17)
  
    The first Pulsar meetup in Paris was held at OVH office. It was organized by HUG France and dedicated to talks for Pulsar. Committers and contributors from OVH, Clever Cloud and StreamNative gathered together to give an introduction of Pulsar/BookKeeper and share the use cases of Pulsar.

    https://www.meetup.com/fr-FR/Hadoop-User-Group-France/events/264920447/ 

- Flink Forward Europe 2019 | Berlin
  
    The Flink community conference happened in Berlin last week. Sijie Guo gave a presentation about the latest integration with Flink 1.9+ around schema/catalog, exactly-once source and etc, and demonstrated the capability of using Pulsar as a unified event stream storage for unified data processing. 

    The presentation is available at https://www.slideshare.net/streamnative/query-pulsar-streams-using-apache-flink. 
    
    https://europe-2019.flink-forward.org/conference-program# 

- Nantes Java User Group
  
    Bruno Bonnin provided an overview of Apache Pulsar at Nantes Java User Group on Oct 15th.
    
    https://nantesjug.org/#/events/2019_10_15

- Crunch Data Conference | Budapest 
  
    Crunch Data Conference happened from Oct 16 to Oct 18. Ivan Kelly gave a presentation of “Infinite topic backlogs with Apache Pulsar”.  

    https://crunchconf.com/speaker/IvanKelly#talks

- ParisDataEng’ #15 ~ Data Engineering with Delta Lake, Pulsar and Spark-tools
  
    There will be a ParisDataEng meetup on Oct 22nd in Paris, including a Pulsar talk by Quentin Adam from CleverCloud. He will share their success story of using Pulsar to manage its high scalable logs infrastructure. 

    https://www.meetup.com/Paris-Data-Engineers/events/264819837/
    
## Blog/Article

- Life beyond Kafka with Apache Pulsar (by Avaro Santos Andres)
  
  https://dzone.com/articles/life-beyond-kafka-with-apache-pulsar

- An introduction to Stream Processing with Pulsar Functions (by Matteo Merli and Jerry Peng)
  
    https://dzone.com/articles/an-introduction-to-stream-processing-with-pulsar-f

- 5 More Reasons to Choose Apache Pulsar over Kafka (by Chris Bartholomew)
  
    https://kafkaesque.io/5-more-reasons-to-choose-apache-pulsar-over-kafka/
