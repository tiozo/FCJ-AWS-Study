### Introduction Edge Locations

Edge Location is the Data Center used to deliver content fast to your users.
It is the site that is nearest your user.

### Fast Delivery

AWS Edge Locations uses a service called CloudFront.
CloudFront is used to store cached copies of your contents.
Resulting in fast delivery of your content.

> [!tips]
> Hosting a static website on S3 with CloudFront to reduce the cost of accessing the web, since a static website rarely change & is usually accessed -> Caching is a good way to reduce HTTP/HTTPS Get/Post to the S3 bucket.

### What is Cache ? 

Caching helps the software to deliver content faster and cheaper.
Cache is fast storage that copies and stores parts of data.
The data is stored in hardware that can deliver content fast, for example, RAM. 
The main job of cache is deliver content fast (look up to notes).
The data is saved in fast hardware layer so that it does not have to use the "slow" storage hardware.

> [!notes]
> Caching exists precisely _because_ cache I/O (RAM/network) is dramatically cheaper and faster than database I/O (disk/query processing), and caching isn't magically works as "save on ram = fast". 
> 
> Caching isn't infinitely scale, you must solve the problem of Cache Invalidation and Cache Eviction. (remove some cache or remove all)
> 
> Caching is designed to **prevent** applications from hitting the database repeatedly. However, it introduces a new problem: **cache inconsistency**. This is similar to the data integrity issues (like race conditions) that can happen in the database, but as you said, it 'changes the place' of the problem. Now, instead of just a database problem, you also have a cache synchronization problem, which can be less severe but is still a critical issue."
> 
> Cache has a property can be stated: "if it lost, it only have a problem called "cold-start" and the data of the application will remains the same."

> [!Additional Info]
> The content is delivered faster because the data is no longer requested from the primary location. 
> It is delivered from the Edge Location. The location nearest to the user.

