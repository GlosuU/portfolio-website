---
title: AWS CLF and SAA notes and flashcards updated and refreshed
description: It's been one year after I passed both AWS Cloud Practitioner (CLF) and Solutions Architect Associate (SAA). AWS constantly updates and changes its offering. Hence, I completely refreshed my CLF notes and flashcards, and by extension the first two sections of my SAA notes.
date: 2026-07-10
tags: ["AWS Certifications", "AWS Exam Prep", "Flashcards"]
thumbnail_image: "0025_tn_updated-clf-materials.png"
---
<img src="{{ '0025_tn_updated-clf-materials.png' | blogImagePath }}" alt="CLF and SAA materials renewed thumbnail" eleventy:ignore>

A bit over a year ago I passed the [AWS Cloud Practitioner (CLF-C02)](https://www.linkedin.com/posts/christian-greciano-408930bb_aws-certified-cloudpractitioner-activity-7321665443671252992-Q4QP/?rcm=ACoAABmWkUgBrADGb2hc3kca-dUpbUhqWmj14YU) and the [AWS Solutions Architect Associate (SAA-C03)](https://www.linkedin.com/posts/christian-greciano-408930bb_aws-certified-solutionsarchitect-activity-7328808800356855810-pmMV/?rcm=ACoAABmWkUgBrADGb2hc3kca-dUpbUhqWmj14YU) certifications. Upon doing so, I published my notes and flashcards of these certs. Now, one year later, I have refreshed my CLF-C02 materials, updating a lot of reference images and adding, editing, or deleting AWS service features and limits. Since the first 2 sections of my SAA notes are taken straight from my CLF-C02 notes, those sections have also been updated in SAA. Many things can change in one year in AWS/cloud technologies, and I'd like to delve a bit deeper on this topic in this blog post. But if you just wanted to get the updated materials, you can just stop reading and just go to the links:

| Certification | Online Notes (Notion)                                                                                                                     | PDF Notes                                      | Anki Flashcards                                      |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- | ---------------------------------------------------- |
| AWS CLF       | [CLF Notion Link](https://psychedelic-cuticle-e74.notion.site/AWS-Cloud-Practitioner-CLF-C02-1cb86c7395e78094a7cfff1bcec54c81)            | [CLF PDF Link](https://ko-fi.com/s/f0b05f206e) | [CLF-C02 Flashcards](https://ko-fi.com/s/98959903e0) |
| AWS SAA       | [SAA Notion Link](https://psychedelic-cuticle-e74.notion.site/AWS-Solutions-Architect-Associate-SAA-C03-917631d1eb354a1f9bb355154879358d) | [SAA PDF Link](https://ko-fi.com/s/5a15162396) | [SAA Anki Link](https://ko-fi.com/s/2eece23025)      |

Note that if you purchased any of the paid materials before the updates, you can download the updated version from Ko-Fi completely for free!

## The Biggest Problem with Cloud Study Materials: Updates
Cloud technologies evolve and change quite fast. Not quite as fast as modern AI technologies (which are changing at an insane pace), but still fast enough to make training materials age like milk. For example, while updating my materials for the CLF cert, the following features and facts have changed for Amazon S3 in the past year:
- An S3 object used to have a maximum size limit of 5TB. This limit is now **50TB**. Handy for those huuuuuge video files!
- Although S3 buckets live in an AWS region, it was a well-known quirk that when creating an S3 bucket you had to give it a name that was **globally** unique. If it so happened that someone else in the world had named their bucket exactly like you wanted, you had to (annoyingly) find a new, not-yet-taken name. This is finally no longer the case! If you now use **account regional namespaces**, you can create an S3 bucket with a name that must only be unique to your account and region. In order to keep its ARN globally unique, AWS appends a suffix (which is unique to your account and region) to your bucket's name under the hood. Wonderful!
- S3 buckets live within a region... except in the case of the S3 One Zone-Infrequent Access storage class. As the name indicates, buckets of that class live only within a single AZ. Well, there's a new storage class called **S3 One Zone-Express**. In the same vein, buckets of this storage class live only within a single AZ, and they're called Directory Buckets. The appeal of this new storage class is that it offers really high performance for S3 operations, which is very handy for stuff like intensive data apps or ML training.

S3 objects being 5TB max and S3 buckets requiring globally unique names have been established facts for years, but they're no longer true. Most AWS training materials will however not reflect these changes, unless they receive regular updates. This includes the study notes that a kind Redditor shared 4 years ago, the free flashcards uploaded to AnkiWeb that have the most upvotes but were uploaded 6 years ago, and yes, even video courses by popular instructors. If I had to plot the usefulness of cloud training materials versus time, it would look something like this:

<img src="{{ '0025_cloud-materials-usefulness-time-graph.png' | blogImagePath }}" alt="Graph depicting the usefulness of Cloud Training Materials over time, showing a drastic decline after 2-year mark" eleventy:ignore>

So in essence, training materials might hold good value for 1-2 years, but then start to drastically lose value. If they are old, you will need to cross-reference them with AWS documentation to make sure you're learning the latest facts and figures.

## Always Check Date of Latest Update, or Learn to Fact Check
The lesson to learn is to make an effort to learn with updated materials, or get into the habit of fact checking old materials. For example, [Andrew Brown](https://www.linkedin.com/in/andrew-wc-brown/) has plenty of AWS certification courses on YouTube in the [FreeCodeCamp channel](https://www.youtube.com/@freecodecamp). It's easy to determine how old the courses are because YouTube registers the date of when a video is uploaded. And Andrew Brown himself performs periodic refreshes of his AWS courses because they do indeed get outdated.

I have to shout out [Stéphane Maarek](https://www.datacumulus.com/) and his video courses in Udemy. He does an outstanding job of keeping his courses up-to-date with the latest AWS trends and news, better than any other instructor I have seen. In fact, one way you can quickly check what has changed in a certain AWS certification is to redownload his course slides after a while. His slides have version numbers and you'll see how after a while the version will be higher. Then, you can upload both the old slides and the new slides to https://www.ilovepdf.com/compare-pdf and compare both documents. A semantic comparison will reveal what is new and what is no longer relevant!

<img src="{{ '0025_maarek-slides-updated.png' | blogImagePath }}" alt="The files of Maarek's slides include a version number to indicate updates" eleventy:ignore>

## Updating my Materials
I currently offer study notes and flashcards for 5 AWS certifications. While it's true that I created them when studying for each of those certs, I don't want to be yet another person who shares and never updates. I hope to dedicate some time on a yearly basis to keep them updated, but it will of course be a best effort considering this is a side-hustle and not my full-time job. I'm also more self-conscious now that if I add more cert materials in the future, that will add to my workload in the future to keep them updated. 😅

I will always be transparent on what version number my materials are, and each version update will include a log of what the updates are (just like software apps!). If you ever purchase any of my materials in my Ko-Fi shop, you are entitled to get the updated versions for free once I release them (you must log in to Ko-Fi with the same user that purchased my materials, and redownload the purchased materials to get the updated version).

<img src="{{ '0025_aws-notes-version-log-screenshot.png' | blogImagePath }}" alt="I include a version log in all my materials to be transparent as to the latest updates" eleventy:ignore>
