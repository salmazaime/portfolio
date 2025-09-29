---
layout: archive
title: "Featured Projects"
permalink: /projects/
classes: wide
---

## Practical Labs and Blue Team Engineering

Welcome to my portfolio of practical cybersecurity projects. Each repository represents hands-on learning, from building secure cloud environments to developing threat detection rules.

Click any project to see the detailed breakdown, learnings, and tools used.

***

{% assign projects = site.pages | where_exp: "item", "item.collection == 'projects'" | sort: "date" | reverse %}

{% for post in projects limit: 3 %}
  {% include archive-single-feature.html type="grid" %}
{% endfor %}

***

## Pinned Repositories

These are my core focus areas. The links below go directly to the GitHub repo.

* **[Blue Team Detection Engineering](https://github.com/salmazaime/blue-team-detection-engineering)**: Focus on SIEM (Splunk/ELK), detection rules (Sigma/YARA), and incident response playbooks.
* **[Cloud Security Lab](https://github.com/salmazaime/cloud-security-lab)**: Securing AWS/Azure configurations, IAM role auditing, and cloud-native monitoring.
* **[AI for Cybersecurity](https://github.com/salmazaime/ai-for-cybersecurity)**: Experiments with ML for security, anomaly detection, and automating data classification.

**Note:** The detailed project pages (linked above) are the "marketing material" for the code in the repos!
