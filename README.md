Bu proje Docker ile containerlara ayrılarak ayağa kaldırılmıştır. Mongodb ile ilişkisel alanların ihtiyaç duyulmadığı noktalarda verimliliği 
arttırmak için dockerize edilerek kullanılmıştıır. Aynı zamanda identity server microservisi ile diğer mikro servisler beslenerek database
işlemleri sağlanmaktadır. Redis kullanarak ise sepet mantığını cashleme ve performansı arttırma çalışmaları yapılmıştır. Yine olmazsa olmaz JWT
(Json Web Token) ile API'lar koruma altına alınmıştır.Client tarafı henüz geliştirilmemiş olup şuan backend mimarisine devam etmekteyim. Bu sayede aslında sürdürülebilir bir E-Ticaret platformunu ayağa kaldırmış
olacağım. Böylelikle yalnızca frontend tarafında clientlar düzenlenerek aslında bir çok firma için bu mimari güncel teknolojileri kullanarak
ayağa kaldırılacaktır. İlerleyen süreçte ise RabitMQ ile kuyruklama mantığını yine yapı içerisine dahil edeceğim. Proje çalışmalarım devam etmektedir.
Güncelleme sağlandıkça buraya da güncel verileri yazmış olacağım.

Hali hazırda testleri başarılı geçmiş API'lar:
Catalog Microservice : 11 API,
Identity Server Microservice :2 API,
Photo Stock Microservice : 2 API



Keywords: Docker,MongoDb,Identity Server, Redis,JWS (Json Web Token), MSSql

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

This project has been divided into containers using Docker for deployment. MongoDB has been dockerized and used to increase efficiency where relational fields are not required. Additionally, the identity server microservice is used to feed other microservices and handle database operations. Redis is used for caching and improving performance using a shopping cart mechanism. JWT (JSON Web Token) is employed to secure the APIs. The client-side has not been developed yet, and I am currently focusing on the backend architecture. By doing so, I aim to create a sustainable e-commerce platform by leveraging modern technologies. This architecture can be adopted by many companies by simply adjusting the client-side implementation. In the future, I plan to incorporate queueing logic using RabbitMQ. The project is still in progress, and I will provide further updates here.

Currently, the following APIs have passed successful testing:
Catalog Microservice: 11 APIs
Identity Server Microservice: 2 APIs
Photo Stock Microservice: 2 APIs
