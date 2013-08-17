***

## Open Intelligence Gathering

### What Is Open Intelligence?

> Open Intelligence is all information floating over internet and publicly available with/without general public log-in to social/professional/educational portals.

> It's also the cause of an intelligent & planned attack instead of going on a blind date with the target.

> There is an entire area of expertise in itself around it, but it's finished products and prophecies are of a great utilization in Modern Security Era.

***

### Legal Documents Got Them

> Every kind of organization, and person is ought to have some legal entity in modern society.

> Being a legal entity means lots of information spread over loads of big & small legal departments.

> Every information you can gather can lead to weak password and other 'guessworks'.

***

### Search Engines Sort Them

> Google.com, the ultimate search power helps you get more target oriented results by using specific search parameters.

> ShodanHQ.com, some call it to be Google for hackers. It's a search engine exposing list of online available devices. You could search for desired Domain and it will try to list all publicly accessible network devices.

> Search facility on NVD.NIST.gov, OSVDB.org, CVE.MITRE.org, SANS.org, CERT.org, EXPLOIT-DB.com, PacketStormSecurity.org, and loads of other nice hacker's blogs, news sites and forums available out there.

***

### Web Activity Caught Them


#### You Blog/Comment

> What are blogs about, the technology you use and ways you work revealing the services on your box.

> The problems (mis-configurations/practices) get discussed over such portals, several times even with logs containing sensitive information about organization internal machines, user names, and more.

> If your blogs are not technical but social, then they might reveal important details about the credential dictionary.


#### You Socialize

> Being active on Social Networking sites make you give away several user information even without intention.

> Scenario: You upload an image taken with your camera, it might have meta-info on camera hinting the PC-Suite installed on your box. If the picture is edited, it also might have the information regarding the image editor being used.


#### You Subscribe

> Subscribing to mailing lists, rss feeds, user groups, & more give away the technological pursuits of people.


#### You Show/Click Ads

> If you show advertisements for a product, a job, or similar then it shows detail about what technology stack does your organization work with.

> You clicking advertisements reflects your technological area of interests and hence what all services you might be using.


#### Even If You Surf Web

> The websites you visit tell a lot about your online persona and hence about your probable choice of used services &/or probable bucket of credentials.

> The web portals (if crafted well and specifically brought to you) could fetch a hell lot of information from your machine.

***


### Automating the Act

* Paterva Maltego CE
* The Harvester


#### Paterva Maltego CE

##### URL: [http://www.paterva.com/web6/products/maltego.php](http://www.paterva.com/web6/products/maltego.php)

##### What?

* It's an Open Source Intelligence gathering tool which also utilizes the forensic-level information collection from publicly available documents, images, or any kind of data being accessed on/by target machine.

* The elements to be used as data magnets are DNS entries, IP addresses, network blocks, website URLs, e-mail IDs, user-names, phone numbers, textual data of high emphasis.

* Once, you provide Maltego Client with your data magnet, it places different data mining algorithms over its collected public domain intelligence from any and every source.

* It has awesome capability of Link Analysis between different data points and bring out relationships.

* Then, it provides a fine linked graph representation of all collected intelligence regarding the data magnet element.

* It has two Editions out. Community Edition is Free and comes with its own limitation. It also has a paid account for Commercial use.


##### How?

* On first run, it brings up a startup-wizard which will itself ask you to log-in/register. You need an account for Free usage.

* Once you are past the 'Login Result', it asks you to select 'Transform Seeds' which decides

* Transforms are like taking a 'hint' from user and map it to asked query type and show the linked information. For instance give hint of the 'dns name' of any target, ask for all the sub-doamins, ip addresses serving them, and more.

* You can merge multiple graph datas and find the mapped links.

* The main power of this utility is the wide range of Transforms provided. So to get expertise over what all information you can gather using Maltego, take quick look at all the Transforms it provides. Details can be seen on need.

* Then there are 3rd Party Transforms available to enhance the information gathering task even more easier and specialized.  Like [PacketNinjas](http://packetninjas.net/) provide extension called [SocialNet](http://packetninjas.net/tools/socialnet.html) which lets you link the data on graph with data from varied Social Network portals like Facebook. Then say using the link analysis power of Maltego you can mine data like common friends, groups, and respective data to Social Network they are part of.
  There is a short [video on how one can create custom transforms](http://www.youtube.com/watch?v=42KhnNQS8AU).


##### Quick Tips

> You can try it out over live disc of your Kali (earlier BackTrack) distro.

> Paterva maintains a [YouTube Channel : PatervaMaltego](http://www.youtube.com/watch?v=3zlbUck_BLk&feature=share&list=PLC9DB3E7C258CD215)


##### Example Usage:

* It has a nice GUI, and if you have used IDEs like Netbeans before then interface is all similar in usage.

* You just need to create a new graph and plot the element on it regarding which you want the open data to be mined and being shown in a graphical linked format.

* You can set the type of information to be churned out of entire data stack.

* read "./HowTo/F1_Maltego.md" for help

***

#### The Harvester

##### URL: [http://code.google.com/p/theharvester](http://code.google.com/p/theharvester)

##### What?

* It's a tool (written in python) for helping Penetration Testers in collecting information related to any domain.

* You could provide it with the Domain name, search partners, depth-level to search and even DNS server to be used.

* It filters out a knowledge base of user names, e-mail ids, hostnames, and sub-domains linked to it.
***

##### Example Usage:

```Shell
python theHarvester.py -d google.com -b all -l 1000 -e 8.8.8.8 -vnct
```

* here '-d' switch determines the Domain to be harvested; then '-b' specifies the KB to be used and it could be 'google', 'bing', 'pgp', more or simple 'all'

* {yet to be added} read "./HowTo/F1_TheHarvester.md" for help

***
***
