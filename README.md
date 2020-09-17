# How big MNCs stores, manages and manipulates thousands of terabytes of data with high speed and efficiency

![image](https://user-images.githubusercontent.com/61896468/93468971-702b5300-f90d-11ea-91b1-91782e652803.png)

## Big Data has gained much attention from the academia and the IT industry. In the digital and computing world, information is generated and collected at a rate that rapidly exceeds the boundary range.

# Current figures

## Currently, over 2 billion people worldwide are connected to the Internet, and over 5 billion individuals own mobile phones. By 2020, 50 billion devices are expected to be connected to the Internet. At this point, predicted data production will be 44 times greater than that in 2009.

# YouTube

## Users upload 100 hours of new videos per minute

## Each month, more than 1 billion unique users access YouTube

## Over 6 billion hours of video are watched each month, which corresponds to almost an hour for every person on Earth.

## This figure is 50% higher than that generated in the previous year

![image](https://user-images.githubusercontent.com/61896468/93469219-d3b58080-f90d-11ea-9cbe-adf17fb0a8c6.png) 

# Facebook

## Every minute, 34,722 Likes are registered

## 100 terabytes (TB) of data are uploaded daily

## Currently, the site has 1.4 billion users

## The site has been translated into 70 languages

![image](https://user-images.githubusercontent.com/61896468/93469293-ecbe3180-f90d-11ea-85b1-228c3ed14c7a.png) 

# Twitter

## The site has over 645 million users

## The site generates 175 million tweets per day

# Foursquare

## This site is used by 45 million people worldwide

## This site gets over 5 billion check-ins per day

## Every minute, 571 new websites are launched

# Google+

## 1 billion accounts have been created on Google

## The site gets over 2 million search queries per minute

## Every day, 25 petabytes (PB) are processed

# Apple

## Approximately 47,000 applications are downloaded per minute

# Brands

## More than 34,000 Likes are registered per minute

# Tumblr

## Blog owners publish 27,000 new posts per minute

# Instagram

## Users share 40 million photos per day

![image](https://user-images.githubusercontent.com/61896468/93469349-019ac500-f90e-11ea-947d-78460819e7dc.png) 

# Flickr

## Users upload 3,125 new photos per minute

# LinkedIn

## 2.1 million groups have been created

# WordPress

## Bloggers publish near 350 new blogs per minute

# WHAT IS BIG DATA IN SIMPLE TERMS?

## Big data refers to the large, diverse sets of information that grow at ever-increasing rates. It encompasses the volume of information, the velocity or speed at which it is created and collected, and the variety or scope of the data points being covered.

# BIG DATA CHALLENGES

## These issues first started preoccupying Google, whose business model is based on storing huge amounts of data and having access to all of it at one time. Makes sense. Their system was adapted into the Hadoop Distributed File System (HDFS for experts).

## The basis of the system is to store the data on a cluster of servers. Instead of having to invest in a really large server, the system functions on the hard drives of lots of computers that you can compare to your PC. This system is infinitely scalable.

## The data is stored redundantly (meaning the same information is written on several different servers, usually 3), so that the system isn’t weakened by one server going down.

## The cluster of servers is constituted of a client server, a driver node, and worker nodes (they’re also often called master nodes and slave nodes, but that’s not super politically correct). A node is a server by the way, which is basically a computer. I am grossly simplifying but the driver node distributes jobs and tracks them across the worker nodes who execute the jobs.

# Challenges faced by Funderbeam

## Funderbeam has more than 160k startups in its database. This is amazing, but it’s also partly troublesome as navigating through the myriad startups becomes very difficult if there is no coherent classification of startups to help filter them by similar industries. Recognizing this, it’s one of our priorities to make the experience of finding information on startups as user-friendly as possible. Here is how we’re accomplishing this.

# How the challenges were resolved.

## We started out by pulling data from various sources where certain tags were applied to startups by the databases or the startups themselves. By doing this, we generated thousand of different tags for most of the 160k startups. Some tags were far too general, like “software”, while others were too specific and didn’t appear often independently. For example, similar tags like music video, music streaming, music chart, music entertainment, music, music label, music venues, and independent music (there are 100’s more like this), are related, so we cluster them together as music and audio. On the other hand, there were some broad tags that were too trivial, i.e. advertising, apps, shopping and so on. In addition, some of the tags were often not descriptive of a company’s actual business and some just had the singular vs. plural problem like designer vs. designers.

![image](https://user-images.githubusercontent.com/61896468/93469424-1d05d000-f90e-11ea-8135-6fbeb4faa51c.png) 

## To overcome these limitations, we used a process called ‘hierarchical clustering’ to group tags with similar characteristics into clusters. What helped us with computing the similarity between tags was using information about the keywords in Wikipedia. Specifically, we compared the content similarity of Wikipedia articles between the different tags. If our algorithm spotted frequently occurring keywords (terms that are specific and representative of a given industry) between two Wikipedia articles, the tags were considered similar.

## The resulting clusters depicted on the massive dendrogram above is a bit much so below we have zoomed in to how the aforementioned music & audio cluster got merged and what are its nearest ‘companions’.

## The outcome of the whole clustering process and data cleansing was an organized set of 45 different tag clusters. Considering we currently have thousands of different tags in our database, this is quite some narrowing and it has significantly eased the experience of searching for startups. For example, you can search from automotive to wellness & fitness industries. And you can filter your searches by valuation, last funding size, headquarters, founding date, and many more features, all on Funderbeam Data.

# The How? What? And why? Of clustered storage

## A computer cluster is a set of loosely or tightly connected computers that work together so that, in many respects, they can be viewed as a single system. Unlike grid computers, computer clusters have each node set to perform the same task, controlled and scheduled by software.

# Clustered storage promises better performance, scalability and reliability, but it's not designed to fit the needs of every storage environment.

## Clustered storage combines multiple arrays or controllers to increase their performance, capacity or reliability. In many cases, it’s a cost-effective way to meet today’s storage needs. But clustering isn’t right for everyone.

## Before choosing whether or how to adopt clustered storage, storage managers should understand their business and data access requirements. This includes asking themselves the following questions:

# What requires the best performance: random or sequential I/O?

## Which is more important: reliability or speed?

## What storage protocols and topologies must be supported?

## How quickly and to what point in time is recovery required after a disaster or hardware failure?

## Clustering has been hitting the news headlines in the last year. For example, EMC Corp. now supports cluster storage for archiving and backup; Hewlett-Packard (HP) Co. bought PolyServe and its clustered file server; IBM Corp. recently purchased XIV Ltd., a privately held storage technology company based in Tel Aviv, Israel; and Sun Microsystems Inc. acquired the Lustre file system.

```
While definitions vary, clustering generally refers to an architecture in which multiple resources (such as servers or storage arrays) work together to increase reliability, scalability, performance and capacity. Technically, clustering can be done at the level of the disk drive as with RAID, in which multiple disk drives increase the scalability and reliability of the array. But the more common definition of clustering has it being done at the file server or file-system level (see "Cluster vs. Grid vs. Global namespace," below).
```

# BIG DATA CHALLENGES

## Big data challenges include storing and analyzing large, rapidly growing, diverse data stores, then deciding precisely how to best handle that data.

## Here we have a list of industry specific big data challenges and how the challenges are overcome:

# 1. Banking and Securities

## Industry-specific Big Data Challenges

```
A study of 16 projects in 10 top investment and retail banks shows that the challenges in this industry include: securities fraud early warning, tick analytics, card fraud detection, archival of audit trails, enterprise credit risk reporting, trade visibility, customer data transformation, social analytics for trading, IT operations analytics, and IT policy compliance analytics, among others.
```

![image](https://user-images.githubusercontent.com/61896468/93469506-39097180-f90e-11ea-8a1b-3c1535048d93.png) 

# Applications of Big Data in the Banking and Securities Industry

## The Securities Exchange Commission (SEC) is using Big Data to monitor financial market activity. They are currently using network analytics and natural language processors to catch illegal trading activity in the financial markets.

```
Retail traders, Big banks, hedge funds, and other so-called ‘big boys’ in the financial markets use Big Data for trade analytics used in high-frequency trading, pre-trade decision-support analytics, sentiment measurement, Predictive Analytics, etc.

This industry also heavily relies on Big Data for risk analytics, including; anti-money laundering, demand enterprise risk management, "Know Your Customer," and fraud mitigation.

Big Data providers are specific to this industry includes 1010data, Panopticon Software, Streambase Systems, Nice Actimize, and Quartet FS.
```

# 2. Communications, Media and Entertainment

## Industry-specific Big Data Challenges

```
Since consumers expect rich media on-demand in different formats and a variety of devices, some Big Data challenges in the communications, media, and entertainment industry include:

Collecting, analyzing, and utilizing consumer insights

Leveraging mobile and social media content

Understanding patterns of real-time, media content usage

Applications of Big Data in the Communications, Media and Entertainment Industry

Organizations in this industry simultaneously analyze customer data along with behavioral data to create detailed customer profiles that can be used to:

Create content for different target audiences

Recommend content on demand

Measure content performance

A case in point is the Wimbeldon Championship (YouTube Video) that leverages Big Data to deliver detailed sentiment analysis on the tennis matches to TV, mobile, and web users in real-time.

Spotify, an on-demand music service, uses Hadoop Big Data analytics, to collect data from its millions of users worldwide and then uses the analyzed data to give informed music recommendations to individual users.
```

![image](https://user-images.githubusercontent.com/61896468/93469581-51798c00-f90e-11ea-8993-7cc62ffaced8.png) 

```
Amazon Prime, which is driven to provide a great customer experience by offering video, music, and Kindle books in a one-stop-shop, also heavily utilizes Big Data.

Big Data Providers in this industry include Infochimps, Splunk, Pervasive Software, and Visible Measures.
```

# 3. Healthcare Providers

## Industry-specific Big Data Challenges

```
The healthcare sector has access to huge amounts of data but has been plagued by failures in utilizing the data to curb the cost of rising healthcare and by inefficient systems that stifle faster and better healthcare benefits across the board.

This is mainly because electronic data is unavailable, inadequate, or unusable. Additionally, the healthcare databases that hold health-related information have made it difficult to link data that can show patterns useful in the medical field.
```

![image](https://user-images.githubusercontent.com/61896468/93469662-6bb36a00-f90e-11ea-9eac-e0ae5e9eeb65.png) 

```
Other challenges related to Big Data include the exclusion of patients from the decision-making process and the use of data from different readily available sensors.
```

# Applications of Big Data in the Healthcare Sector

```
Some hospitals, like Beth Israel, are using data collected from a cell phone app, from millions of patients, to allow doctors to use evidence-based medicine as opposed to administering several medical/lab tests to all patients who go to the hospital. A battery of tests can be efficient, but it can also be expensive and usually ineffective.
```

![image](https://user-images.githubusercontent.com/61896468/93469716-7ff76700-f90e-11ea-8ed8-d7716f2c6361.png) 

```
Free public health data and Google Maps have been used by the University of Florida to create visual data that allows for faster identification and efficient analysis of healthcare information, used in tracking the spread of chronic disease.

Obamacare has also utilized Big Data in a variety of ways.

Big Data Providers in this industry include Recombinant Data, Humedica, Explorys, and Cerner.
```

![image](https://user-images.githubusercontent.com/61896468/93469784-969dbe00-f90e-11ea-9fbc-af3eb5b62612.png) 

# 4. Education

```
EducationIndustry-specific Big Data Challenges

From a technical point of view, a significant challenge in the education industry is to incorporate Big Data from different sources and vendors and to utilize it on platforms that were not designed for the varying data.

From a practical point of view, staff and institutions have to learn new data management and analysis tools.

On the technical side, there are challenges to integrating data from different sources on different platforms and from different vendors that were not designed to work with one another.

Politically, issues of privacy and personal data protection associated with Big Data used for educational purposes is a challenge.
```

# Applications of Big Data in Education

```
Big data is used quite significantly in higher education. For example, The University of Tasmania. An Australian university with over 26000 students has deployed a Learning and Management System that tracks, among other things, when a student logs onto the system, how much time is spent on different pages in the system, as well as the overall progress of a student over time.
```

![image](https://user-images.githubusercontent.com/61896468/93469842-a917f780-f90e-11ea-9d7c-af6bfaee09f1.png)

 

## In a different use case of the use of Big Data in education, it is also used to measure teacher’s effectiveness to ensure a pleasant experience for both students and teachers. Teacher’s performance can be fine-tuned and measured against student numbers, subject matter, student demographics, student aspirations, behavioral classification, and several other variables.

```
On a governmental level, the Office of Educational Technology in the U. S. Department of Education is using Big Data to develop analytics to help correct course students who are going astray while using online Big data courses. Click patterns are also being used to detect boredom.
```

### Big Data Providers in this industry include Knewton and Carnegie Learning and MyFit/Naviance.

![image](https://user-images.githubusercontent.com/61896468/93469889-c0ef7b80-f90e-11ea-9e3d-696333228c55.png) 

# 5. Manufacturing and Natural Resources

## Industry-specific Big Data Challenges

```Increasing demand for natural resources, including oil, agricultural products, minerals, gas, metals, and so on, has led to an increase in the volume, complexity, and velocity of data that is a challenge to handle.

Similarly, large volumes of data from the manufacturing industry are untapped. The underutilization of this information prevents the improved quality of products, energy efficiency, reliability, and better profit margins.
```

## Applications of Big Data in Manufacturing and Natural Resources

```In the natural resources industry, Big Data allows for predictive modeling to support decision making that has been utilized for ingesting and integrating large amounts of data from geospatial data, graphical data, text, and temporal data. Areas of interest where this has been used include; seismic interpretation and reservoir characterization.

Big data has also been used in solving today’s manufacturing challenges and to gain a competitive advantage, among other benefits.

In the graphic below, a study by Deloitte shows the use of supply chain capabilities from Big Data currently in use and their expected use in the future.
```

![image](https://user-images.githubusercontent.com/61896468/93469971-dbc1f000-f90e-11ea-8ecb-fc3010a2cf47.png) 

# 6. Government

### Industry-specific Big Data Challenges

```
In governments, the most significant challenges are the integration and interoperability of Big Data across different government departments and affiliated organizations.
```

![image](https://user-images.githubusercontent.com/61896468/93470047-f2684700-f90e-11ea-9711-5c864ba4a336.png) 

## Applications of Big Data in Government

```
In public services, Big Data has an extensive range of applications, including energy exploration, financial market analysis, fraud detection, health-related research, and environmental protection.

Some more specific examples are as follows:

Big data is being used in the analysis of large amounts of social disability claims made to the Social Security Administration (SSA) that arrive in the form of unstructured data. The analytics are used to process medical information rapidly and efficiently for faster decision making and to detect suspicious or fraudulent claims.

The Food and Drug Administration (FDA) is using Big Data to detect and study patterns of food-related illnesses and diseases. This allows for a faster response, which has led to more rapid treatment and less death.

The Department of Homeland Security uses Big Data for several different use cases. Big data is analyzed from various government agencies and is used to protect the country.
```

![image](https://user-images.githubusercontent.com/61896468/93470107-04e28080-f90f-11ea-99ac-4c396378ec23.png) 

## Big Data Providers in this industry include Digital Reasoning, Socrata, and HP.

# 7. Insurance

## Industry-specific Big Data Challenges

```Lack of personalized services, lack of personalized pricing, and the lack of targeted services to new segments and specific market segments are some of the main challenges.

In a survey conducted by Marketforce challenges identified by professionals in the insurance industry include underutilization of data gathered by loss adjusters and a hunger for better insight.
```

## Applications of Big Data in the Insurance Industry

```
Big data has been used in the industry to provide customer insights for transparent and simpler products, by analyzing and predicting customer behavior through data derived from social media, GPS-enabled devices, and CCTV footage. The Big Data also allows for better customer retention from insurance companies.

When it comes to claims management, predictive analytics from Big Data has been used to offer faster service since massive amounts of data can be analyzed mainly in the underwriting stage. Fraud detection has also been enhanced.

Through massive data from digital channels and social media, real-time monitoring of claims throughout the claims cycle has been used to provide insights.

Big Data Providers in this industry include Sprint, Qualcomm, Octo Telematics, The Climate Corp.
```

# 8. Retail and Wholesale trade

## Industry-specific Big Data Challenges

```
From traditional brick and mortar retailers and wholesalers to current day e-commerce traders, the industry has gathered a lot of data over time. This data, derived from customer loyalty cards, POS scanners, RFID, etc. are not being used enough to improve customer experiences on the whole. Any changes and improvements made have been quite slow.
```

## Applications of Big Data in the Retail and Wholesale Industry

```
Big data from customer loyalty data, POS, store inventory, local demographics data continues to be gathered by retail and wholesale stores.

In New York’s Big Show retail trade conference in 2014, companies like Microsoft, Cisco, and IBM pitched the need for the retail industry to utilize Big Data for analytics and other uses, including:

Optimized staffing through data from shopping patterns, local events, and so on

Reduced fraud

Timely analysis of inventory

Social media use also has a lot of potential use and continues to be slowly but surely adopted, especially by brick and mortar stores. Social media is used for customer prospecting, customer retention, promotion of products, and more.

Big Data Providers in this industry include First Retail, First Insight, Fujitsu, Infor, Epicor, and Vistex.
```

# 9. Transportation

## Industry-specific Big Data Challenges

```
In recent times, huge amounts of data from location-based social networks and high-speed data from telecoms have affected travel behavior. Regrettably, research to understand travel behavior has not progressed as quickly.


In most places, transport demand models are still based on poorly understood new social media structures.
```

## `Applications of Big Data in the Transportation Industry`

```
Some applications of Big Data by governments, private organizations, and individuals include:

Governments use of Big Data: traffic control, route planning, intelligent transport systems, congestion management (by predicting traffic conditions)

Private-sector use of Big Data in transport: revenue management, technological enhancements, logistics and for competitive advantage (by consolidating shipments and optimizing freight movement)

Individual use of Big Data includes route planning to save on fuel and time, for travel arrangements in tourism, etc.
```

![image](https://user-images.githubusercontent.com/61896468/93470192-20e62200-f90f-11ea-95d9-822bcd1d4a5f.png)

# 10. Energy and Utilities

## Industry-specific Big Data Challenges

```
The image below shows some of the main challenges in the energy and utility industry.
```

## Applications of Big Data in the Energy and Utility Industry

```
Smart meter readers allow data to be collected almost every 15 minutes as opposed to once a day with the old meter readers. This granular data is being used to analyze the consumption of utilities better, which allows for improved customer feedback and better control of utilities use.

In utility companies, the use of Big Data also allows for better asset and workforce management, which is useful for recognizing errors and correcting them as soon as possible before complete failure is experienced.

Big Data Providers in this industry include Alstom Siemens ABB and Cloudera.
```

# What is Distributed Storage?

## A distributed storage system is infrastructure that can split data across multiple physical servers, and often across more than one data center. It typically takes the form of a cluster of storage units, with a mechanism for data synchronization and coordination between cluster nodes.

```
`Distributed storage ` is the basis for massively scalable cloud storage systems like Amazon S3 and Microsoft Azure Blob Storage, as well as on-premise distributed storage systems like Cloudian Hyperstore.
```

```
Distributed storage systems can store several types of data:

Files—a distributed file system allows devices to mount a virtual drive, with the actual files distributed across several machines.

Block storage—a block storage system stores data in volumes known as blocks. This is an alternative to a file-based structure that provides higher performance. A common distributed block storage system is a Storage Area Network (SAN).

Objects—a distributed object storage system wraps data into objects, identified by a unique ID or hash.
```

# What is Hadoop and why it matters?

## Hadoop is an open-source software framework for storing data and running applications on clusters of commodity hardware. It provides massive storage for any kind of data, enormous processing power and the ability to handle virtually limitless concurrent tasks or jobs.

![image](https://user-images.githubusercontent.com/61896468/93470253-3d825a00-f90f-11ea-83f7-51f3b8087afe.png) 

# Why is Hadoop important?

## Ability to store and process huge amounts of any kind of data, quickly. With data volumes and varieties constantly increasing, especially from social media and the Internet of Things (IoT), that's a key consideration.

```
`Computing power `:

Hadoop's distributed computing model processes big data fast. The more computing nodes you use, the more processing power you have.

`Fault tolerance`:
Data and application processing are protected against hardware failure. If a node goes down, jobs are automatically redirected to other nodes to make sure the distributed computing does not fail. Multiple copies of all data are stored automatically.

`Flexibility`:
Unlike traditional relational databases, you don’t have to preprocess data before storing it. You can store as much data as you want and decide how to use it later. That includes unstructured data like text, images and videos.

`Low cost`:
The open-source framework is free and uses commodity hardware to store large quantities of data.

`Scalability`:
You can easily grow your system to handle more data simply by adding nodes. Little administration is required.
```

![image](https://user-images.githubusercontent.com/61896468/93470330-5db21900-f90f-11ea-8fd1-c2702ceddf88.png)
