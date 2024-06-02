Espoo, Finland / me@moham.info / [LinkedIn](https://www.linkedin.com/in/mhpandi/)

#### I am a software engineer who takes full ownership of building solutions and diving deep into technical complexities. I am eager to leverage my experience to make a significant impact on team success.

<br />

|                           | Technologies                                                           |
|---------------------------|------------------------------------------------------------------------|
| **Programming languages** | Java, Kotlin, JavaScript, Python                                       |
| **Web**                   | Spring MVC, JAX-RS, Javalin, Express, Flask                            |
| **Cloud**                 | AWS (ECS, Lambda, CloudFormation, DynamoDB, EMR, SageMaker, Glue, etc) |
| **Big Data**              | Hadoop, Spark                                                          |
| **DevOps**                | Docker, Kubernetes, Terraform                                          |
| **Data**                  | JDBC, JPA, Spring Data                                                 |
| **Search**                | Apache Lucene, Solr, Elasticsearch                                     |
| **UI**                    | GWT, JSF, Java Swing                                                   |


## Experience

### [Mapbox](https://www.mapbox.com)

- **[Static Images API](https://docs.mapbox.com/api/maps/static-images)**: It serves more than 6K requests per second including customers like **Strava** and **Yahoo Japan** weather. To have a successful rendered image as response we leveraged node.js native addons to use [Mapbox GL](https://docs.mapbox.com/help/glossary/mapbox-gl/) native renderer as part of our HTTP service. Moreover, we needed to integrate with upstream services such as [vector tiles](https://docs.mapbox.com/api/maps/vector-tiles/), and [raster tiles](https://docs.mapbox.com/api/maps/raster-tiles/).


- **AWS S3 Optimization**: Originally, we stored tiles on S3, partitioned by date. Although this method was efficient, it posed challenges when we needed to delete tiles associated with inactive customers. To address this, we decided to reorganize our data, partitioning it by account ID instead of date. I utilized an [AWS Glue ETL](https://docs.aws.amazon.com/prescriptive-guidance/latest/serverless-etl-aws-glue/aws-glue-etl.html) job to establish a pipeline that facilitated this reformatting, streamlining the process for better management and cost efficiency.


- **ECS Tasks Provisioning**: Design a solution to provision additional temporary [ECS tasks](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definitions.html) in response. In services deployed on Fargate Spot, there is always a chance of capacity interruptions. AWS initiates a Spot interruption when it needs to reclaim the Spot capacity. After this interrupt, the application is granted a 120-second window to perform a graceful shutdown. If the service scheduler is unable to place a new task due to the unavailability of Fargate Spot capacity, then the “Spot interruption” will lead to a task placement failure that potentially can affect the service availability.


- **Semantic tiles API**: Provide location API for [Square Enix](https://www.square-enix.com/) which is used in the [Dragon Quest](https://dragonquest.square-enix-games.com/xi/en-us/) game. Here we served our vector tiles for some specific tileset sources to extract some features that are used in the game.


- **[Geocoding API](https://docs.mapbox.com/api/search/geocoding/) Enhancement**: Enhanced API by sharding the search index based on request category.


- **[Tiling Service](https://docs.mapbox.com/mapbox-tiling-service/guides/)**: Made the service highly available by designing replication and failover strategies. Storing tiles in multiple regions and having a failover mechanism makes it possible to read and write tilesets during a regional S3 outage.


- **Atlas Security Updates**: Revived [Atlas](https://www.mapbox.com/atlas) with major security updates for customers like [USAF](https://www.airforce.com/). Atlas supports Docker Compose, a tool for defining and running multi-container Docker applications. Atlas for Docker Compose lets customers run Atlas on a single host.


- **Site Reliability Engineering**: Actively participated in the on-call rotation, assuming Site Reliability Engineering (SRE) responsibilities for over ten production services. This role required me to ensure the high availability, performance, and resilience of our services, which are critical in a high-stakes production environment.

### [F-Secure](https://www.f-secure.com/en)

- **Cloudify Device Registry Service**: Developed the backend for SENSE-enabled routers, integrating security features into the router by monitoring network traffic. Components included:
  - Pairing service for SENSE mobile app registration
  - Data management of routers and connected devices
  - Operators configuration management
  - User profiles and feature management

### [Bankify](https://bankify.io/)

- **Invoice Barcode Scanner**: Developed primary revenue-generating service and consulted on integrating data mining techniques into the automated savings API.


- **Recommendation Engine**: Designed an engine on top of extracted data from receipt images.

### [Parsian Insurance](https://parsianinsurance.ir/fa-IR/parsianinsurance/1/page/%D8%AE%D8%A7%D9%86%D9%87)

- **Backend Service Development**: Developed backend service for life insurance offering and proposed an end-to-end solution for replacing the legacy Personal Accident Insurance system. Tasks included:
  - Designing an end-to-end architecture
  - Leading an agile team through development process
  - Taking a domain-driven approach for maximum collaboration with business experts
  - Developing back-end module

### [Mehad](https://mehad.ir/)

- **Software Interface for Car ECUs**: Implemented software connecting car ECUs to PCs, enhancing efficiency of diagnostic tool operators. Contributions to the flagship product, iDiag, included:
  - Developing a software interface for ECU-PC connections
  - Integrating a module for connecting to a wireless station for real-time testing
  - Refactoring production software for customized distribution packages

### Persian Search Engine

- **Graduate Research Project**: Joined "ranker" team to implement a search engine, focusing on full-text search and big data challenges. Key responsibilities included:
  - Modelling documents in vector space
  - Designing the inverted index
  - Scheduling MapReduce jobs to update index weights
  - Implementing ranking algorithm for user queries

### [Douran Group](https://www.linkedin.com/company/douran-group/?originalSubdomain=ir)

- **Junior Software Engineer**: Collaborated on the human resources module of the Douran ERP system and developed database migration tools. Contributions included:
  - Developing the ERP human resource module
  - Creating automated database migration tools for upgrading base information and schemas
  - Developing a web interface for migration tools to streamline processes

## Education

- **Master's degree in Artificial Intelligence and Robotics** (Iran University of Science and Technology)
  - Thesis: [A Novel Similarity Measure for Sequence Data](https://www.researchgate.net/publication/236848462_A_Novel_Similarity_Measure_for_Sequence_Data)
  - Publication: [NDVI Optimization Using Genetic Algorithm](https://www.semanticscholar.org/paper/NDVI-Optimization-Using-Genetic-Algorithm-Kabiri-Pandi/b6c87aea6b1ffd7c3ca9468df43e0d706ac057b6)

- **Bachelor's degree in Software Engineering** (Sharif University of Technology)
