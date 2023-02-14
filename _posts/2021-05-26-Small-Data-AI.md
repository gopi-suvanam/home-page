## Small Data AI

There is a fascinating story about horse manure paraphrased in the TV series “Silicon Valley”:

> In the 1890s, the Industrial Revolution had people flocking to the city, and more people equals more horses, and more horses equals more manure. And it was predicted that by the middle of the next century, there would be nine feet of manure covering the streets. But what no one saw coming, was a new technology that would completely obliterate those concerns. The car. Over night, the manure problem vanished.

Our current problem with large amount of data spread out on the Internet and various organizations is also similar to the problem of horse manure in the 1890s. Organizations are collection data from all the sources possible and putting them in a central location. Now they want to figure out a way to “use” the data. They start spending incredible amounts of money data lakes, BigData platforms etc. They are not ready for the invention of the car, which will obviate the need for storing all the data manure: i.e. AI using Small Data.

### Hype About BigData
There is a whole lot of bragging about how data is growing and is changing the world. But ask any expert where it can be used and most of them give examples of using basic analytics and call that BigData use cases. In reality, BigData has not shown any significant contribution to many organizations that have spent millions of dollar on it. The only real use of BigData that I have come across is in the space of online marketing: selling the right advertisement or product to the consumer. May be things will change. But I don’t see any significant development happening until BigData is stopped being seen as a monolithic field. It would be even better if the word is not used all together. Instead data analytics and AI should be focused on the basis of verticals: financial analytics, marketing analytics, machine analytics etc. Companies should also focus on niche and not try to solve all problems using a single platform.

### User Control on Data
A big reason for move towards Small Data AI is related user privacy and control. Globally, regulations on data privacy are becoming stringent. Customers are also becoming more and more aware of their right with regards to their data. Having custody of customer data is becoming a liability more than an asset. If not immediately, eventually most of the customer data will not be available for service providers to monetize. Decentralized solutions (like blockchain based applications) will further reduce the availability of data. To put it shortly, software may not be able to learn from user shared images, companies may not be able to use user data for cross-selling etc. Data based algorithms will still be used, but the data used in those algorithms will be severely restricted.

### AI without BigData
AI is not necessarily equivalent to BigData. We as humans do not need to see 100,000 pictures of cats to figure out if an image has a cat. We use more sophisticated process (algorithm) to identify objects. Similarly with regards to other areas of cognition and decision making, like for example understanding a piece of text or driving a car on the road, we use much more sophisticated process than learning from millions of input data sets. Using large amount of data to train machines is a shortcut, in some ways - a lazy approach, to achieve intelligence or the pretense of intelligence. AI can exist without BigData. Of course more research has to go in to building such an AI.

### Cheap RAM is obviating the need for BigData Solutions
The hype about BigData tools is also because even running through several hundreds of GB in memory was becoming a problem, forget about terra and peta bytes of data. This particular problem is especially faced by data scientists who want to build models and experiment with data. This problem has led to spawning of several BigData tools with multiple layers. This led to complex stack with lot of overheads ala MLlib on Spark on HBase on Yarn on HDFS on Java on Virtual Machine on Bare Metal. All this for doing task which are quite “immature” compared to the high end analytics data scientists actually want to do. The whole complexity drops if the memory available on a single machine increases drastically, which is what is happening right now. Simple desktops can have upto 128GB easily. Higher end servers are easily available on AWS or any other cloud solutions. Not many organizations need more than a couple of 100s of GBs of data for analysis (especially after discarding unnecessary data). With high end memory, most data science problems can be solved beautifully using traditional tools like R or Python. Thus data scientists can focus on actual analysis rather than engineering a complex set of tools.

### Tools and Techniques for Small Data AI
So that brings us to the question of the tools and techniques that can be used to leverage AI using small data.

1. Database innovations: Columnar databases and other similar innovations solve the problem of running analytics on large amount of data. For example one need not implement Hadoop ecosystem to process large amount of data - columnar databases or No-SQL databases (depending on the use case) are not only sufficient but more importantly efficient.
2. Non-Deep Learning: Using more diverse set of machine learning tools other than just using neural networks for learning. Ensemble algorithms, state-space models etc. can be good complement to neural networks.
3. Statistical Learning: There is considerable research on statistical learning (parametric and non-parametric estimation of distributions/relationships). This research is the work of several centuries outside the domain of machine learning. Such models are used through out scientific community. These models can be applied in AI as well.
4. Probabilistic models: Other data based approaches one can also build probabilistic/fuzzy models, which can be finetuned heuristically or with limited set of data.
Incremental learning: Humans do not learn everything in one day. Same can be with machines. Machines can learn, store the learn information and every incremental data point can be used to update the learn information. Thus only the learnt information is stored and not the whole data.
5. Transfer learning: Another interest thing humans do is transfer the learning from one set of activity to another. For example, we learn how to recognize trees when we are kids and we use that learning while driving a car to avoid hitting trees. When we start learning how to drive a car we do not start from scratch. We come with previously learnt skills, which are transferred to the job of driving a car. current AI projects on the other hand try to build end-to-end learning, which is very very inefficient. We should use the concept of transfer learning more efficiently to learn from limited set of data available.
6. Fog/edge computing: There has been an increased dependence on centralized computing using using the cloud. When users start taking control of their data and want their data to be on their device, developers should develop more decentralized processing solutions. These are what I call as fog (decentralized and spread across several users) or edge (computation done on the user’s device) computing solutions. Some examples of fog computing include BitTorrent, Blockchain etc.
