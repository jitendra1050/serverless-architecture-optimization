# serverless-architecture-optimization
serverless-architecture-optimization- brainstorm

For creating a server less architecture and Cost Optimization Challenge: Managing Billing Records in Azure Serverless Architecture we can use

**2 Options for 3 months old data**
  1. Blob storage: cheaper but might not work for complex query
  2. Azure SQL for serverless: expensive then Blob, but good with complex query

We can create a azure function which will move our 3 months old data from Cosmos to our old system by weekly, monthly, daily basis(depends on incoming data flow)

Issue with blob:
 * wont be able to do complex query to retrive data
 * will take more time then cosmosDB assuming seconds

Issue with Azure SQL
* Cold start issue, take more then initially, can use caching strategy or light query run to keep this service alive.
* Slighly expensive then BLOB.

ChatGPT conversation: https://chatgpt.com/share/6891a3e9-e0bc-800f-b693-5f1e47c58aa5
  
 
     
