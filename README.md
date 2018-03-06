# Distributed-Transactions
Sample configurations for distributed transactions in EI


1. Configure ActiveMQ and Mysql with EI using the lib jars available in libs folder.
2. Setup Mysql 5.7.21 and execute resources/database.sql to create the database and table.
3. Replace transactions.properties file found in EI/wso2/lib with resources/transactions.properties.
4. Replace EI/conf/datasources/master-datasources.xml with resources/master-datasources.xml.
5. Start Mysql and ActiveMQ.
6. Deploy orderRequestAPI (resources/orderRequestAPI.xml) in EI using management console.
7. Invoke API using sample payload found in resources folder, with below command.

curl -v -X POST  -d  sampleRequest.xml -H "Content-type: text/xml" http://host:8280/quote/store
