---
title: "AWS Resolved Its Outage 2021"
date: 2021-12-08T21:51:03+08:00
draft: false
---

## The day the internet paused
Amazon Web Services had one of its worst outages ever on Tuesday. The problems cascaded through the company’s retail operation—which uses software and apps that run on AWS—during the holiday shopping rush. Vans sat idle; drivers were sent home; packages piled up at the worst possible time [^1].

Tuesday offered the kind of jolt that reminds us how many products and services are centralized in common data centers run by just a handful of big tech companies like **Amazon, Microsoft and Google**. It’s also a reminder of the vulnerability of much of the infrastructure underpinning day-to-day life online. 

<figure>
  <img src="../images/aws-resolved-its-outage-2021.png" alt="API Error Rates in US-EAST-1">
  <figcaption>Figure 1: AWS has mitigated AWS Error Rate issue that caused some network devices in the US-EAST-1 on Dec 7, 2021. (Source: <a href="https://status.aws.amazon.com">'AWS Service Health Dashboard'</a>)</figcaption>
</figure>

## Prolonged AWS outage takes down a big chunk of the internet
Problems with some Amazon Web Services cloud servers are causing slow loading or failures for significant chunks of the internet. Amazon’s widespread network of data centers powers many of the things you interact with online, including this website, so as we’ve seen in previous AWS outage incidents, any problem has massive rippling effects. People started noticing problems at around **10:45AM** ET, and just **after 6PM ET** the AWS Status showed _"Many services have already recovered, however we are working towards full recovery across services"_ [^2].

Earlier in November Google Cloud suffered outages, and more than **30,000 impacted customers observed Google 404 errors** on their websites [^3], we need to focus on "Outcomes" first and "as a Service" second [^4]. When servers belonging to Fastly went down in June, it proved to be a lesson in the virtue of decentralization—the practice of distributing content across as many servers as possible [^5]. 

The latest problems come as Amazon customers ramp up their Christmas purchases. I’m seeing more _"cloud" disruptions_ these days. I think we’re living in a time where we’re extremely judgmental and quick to treat IT as disposable. We’ve always placed great importance on the mistake. But the next move, what you do after the mistake. We’re all going to make mistakes.

## What Happens Now? 
But what is that next step? And that’s the part I find so much more invigorating and interesting. Tuesday’s disruptions will likely reinvigorate industry debate around _"multi-cloud"_ strategies, an idea that a company should duplicate its services across multiple cloud computing providers so no one crash puts your company out of business.

> Chaos Engineering is the discipline of experimenting on a system in order to build confidence in the system’s capability to withstand turbulent conditions in production - PRINCIPLES OF CHAOS ENGINEERING [^6].

**Chaos engineering** or chaos testing is a Site Reliability Engineering (SRE) technique that simulates unexpected system failures to test a system's behavior and recovery plan. Based on what is learned from these tests, organizations design interventions and upgrades to strengthen their technology.

In the cloud native world, this concept is even more important because the systems are very dynamic _(infrastructure and applications often scale; code changes often occur)_, and we need to ensure that these systems remain resilient. Increased availability and decreased **mean time to resolution (MTTR)** are the two most common benefits enterprises observe. Teams who frequently run chaos engineering experiments enjoy more than **99.9% availability**. Ideally, chaos testing is best run in production. However, I recommend that you learn in a lower environment first and then conduct controlled experiments in production later. 

## External References
[^1]: https://www.bloomberg.com/news/newsletters/2021-12-08/aws-resolved-its-outage-what-happens-now
[^2]: https://www.theverge.com/2020/11/25/21719396/amazon-web-services-aws-outage-down-internet
[^3]: https://status.cloud.google.com/incidents/6PM5mNd43NbMqjCZ5REh
[^4]: https://sergiubodiu.github.io/sergiubodiu/posts/cloud-as-a-service-outlook-2025/#focus-on-outcomes-first-and-as-a-service-second 
[^5]: https://qz.com/2018245/a-fastly-outage-took-down-the-guardian-and-new-york-times/
[^6]: https://principlesofchaos.org
