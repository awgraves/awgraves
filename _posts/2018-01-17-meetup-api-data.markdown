---
layout: post
title: User Friendly Python Script to Gather Meetup.com API Data
date: 2018-01-17 13:32:20
description: 
img: meetup_logo.png # Add image post (optional)
tags: [python, api, data cleaning]
---
<p align = "center">
<b>
Save yourself time by automatically generating a cleaned dataset of all registered meetup groups at a given location!</b></p>


## Which information is included?

The script outputs a CSV file containing the following information on each group:

* Basic Info
	* name of group
	* group id
* Location
	* city name
	* precise latitude of meetup location
	* precise longitude of meetup location
* Group Attributes
	* meetup category (Social, Tech, Arts, etc.)
	* date & time of group creation (in local timezone)
	* join mode (open / approval)
	* status (active / grace)
	* number of current members
* Past Events
	- number of previous events
	- date & time of most recent past event (in local timezone)
	- number of 'yes' rsvps for most recent past event

## How to use it

> **Note that you must have python 3.6 installed along with the necessary libraries and modules described in the readme file of this script. I recommend the [Anaconda distribution](https://github.com/awgraves/meetup_api/blob/master/meetup_csv_gen.py) of Python which includes everything you will need.**

1. Visit my [github](https://github.com/awgraves/meetup_api) to clone the repo (i.e. download the zip file).

2. Open up a terminal and navigate to the unzipped folder.

3. Run:
	````
	python meetup_gen_csv.py
	````
4. You will be prompted for your meetup.com API key the first time. ***You will need to register a normal user account with [meetup.com](http://www.meetup.com/register) to obtain a key.***  This is only necessary the first time because the script will remember your key for any subsequent uses.

	![first]({{site.url}}/assets/img/meetup_api_imgs/enter_api.png)

5. Then enter your desired zip code and search radius.
	
	![search zip]({{site.baseurl}}/assets/img/meetup_api_imgs/zipcode.png)
	
6. If all your inputs were valid, the script will make all the necessary server requests, clean and organize the data, then export a CSV file in the same folder.

	![terminal output]({{site.baseurl}}/assets/img/meetup_api_imgs/successful_output.png)
	
7. That's it!  Your are now ready to open the file in your favorite program and discover what insights it has to offer.

	![jupyter csv]({{site.baseurl}}/assets/img/meetup_api_imgs/jupyter_csv.png)

**If you want to see how it works under the hood, [check out the code](https://github.com/awgraves/meetup_api/blob/master/meetup_csv_gen.py) for yourself.  Don't worry, I was courteous with line comments.**

