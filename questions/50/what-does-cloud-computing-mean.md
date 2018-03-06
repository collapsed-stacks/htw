## What does "Cloud Computing" mean?

- posted by: [MalsR](https://stackexchange.com/users/-1/31-malsr) on 2011-04-18
- tagged: `networking`, `cloud-computing`
- score: 1

What does "cloud computing" mean and how are cloud computing services provided?


## Answer 78

- posted by: [eMansipater](https://stackexchange.com/users/-1/56-emansipater) on 2011-04-18
- score: 2

<p>"Cloud computing" refers mainly to the experience of a computer user where a service is provided to them across the internet without the specific details of the service (such as what physical computer hardware it runs on, which geographic location that hardware has, or how many devices and other services that service relies on) being either readily apparent to the user, or indeed mattering at all for its usage.  The metaphor of a "cloud" refers to this vagueness and uncertainty of detail.  Specifically, "the cloud" is a metaphor for the internet, with its pool of resources available equally to all connected users.</p>

<p>As an example, consider the use of a web-based email provider like <a href="https://mail.google.com/" rel="nofollow">Gmail</a>.  The service is accessed simply by typing in an internet address, or via en email client like any other email service; however "behind the scenes" the user may <em>actually</em> be accessing internet servers in different geographical locations, with multiple copies of their data stored in multiple places.  The web page being "served" to them may be balanced across multiple physical and virtual providers or even moved seamlessly between them while running.  The failure of any given computer in any given Google data centre would not impact their experience of the Gmail service in the slightest--and all this happens invisibly, without any of its complexity evident to the user who is simply reading an email forward about cats.  It's like the water in your sink--you just turn on the tap and it comes.</p>

<p>Several techniques are used to provide "cloud computing" services, such as</p>

<ul>
<li>The use of <a href="http://en.wikipedia.org/wiki/Hardware_virtualization" rel="nofollow">virtual machines</a> to run multiple independent "computers" on a single set of hardware.</li>
<li>Custom software layers to abstract requirements such as <a href="http://en.wikipedia.org/wiki/Storage_virtualization" rel="nofollow">storage space</a> or processing power away from the hardware that provides them.</li>
<li>The use of <a href="http://en.wikipedia.org/wiki/Load_balancing_%28computing%29" rel="nofollow">load balancing</a> methods to distribute or move workloads between multiple computers or locations while providing a seamless experience to the user.</li>
<li>The offering of highly scalable and adaptable environments to web and software developers under a <a href="http://en.wikipedia.org/wiki/Utility_computing" rel="nofollow">utility computing</a> model where the program or web service can use as much or as little computing resources as needed with a single bill for the combined total at the end.</li>
</ul>

<p>The key characteristic of "cloud computing" is that computer processing and data are <a href="http://en.wikipedia.org/wiki/Cloud_computing#Characteristics" rel="nofollow">not in a specified, known, or static place</a>.</p>



## Answer 55

- posted by: [Jacob](https://stackexchange.com/users/-1/28-jacob) on 2011-04-18
- score: 1

There are several concepts of "the cloud" I'll try to cover the basics
The concept of a cloud means a server is virtualized under another one. This means instead of buying the resources of an entire server, you can scale up and down with little or no down time. Clouds usually are billed as a per time usage vs once a month flat fee.( IE 1 IP is 2 cents an hour vs 12 a month) Clouds also have other features that dedicated servers don't. Instances can usually switch hosts very quickly incase of hardware failure. Also, storage is generally on a SAN(Storage area network) which provides redundant storage, and helps to move the server between hosts.  


## Answer 59

- posted by: [geoffc](https://stackexchange.com/users/-1/34-geoffc) on 2011-04-18
- score: 1

There are two basic approaches. 

 1. Host your app on someone elses hardware in their data center that they run using a traditional operating system like Windows, Linux, or Unix.  All you do is run your application there.   Thus the hardware is abstracted (like Amazon EC3) and not your problem.
 2. Write an application that resides entirely on custom platforms.  Google as an example wrote their own storage layer.  Their own authentication layer, and so on, with very little being core basic operating system stuff.  You can write to all these different layers for your applications.

The Windows cloud commercials baffle me.  I think they are hilarious, but I cannot see the Cloud aspect of them. 





---

All content is licensed under the [CC BY-SA 3.0 license](https://creativecommons.org/licenses/by-sa/3.0/).
