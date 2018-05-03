# Week 9 Project: Honeypot
## Overview and setup

The goal of this lab was to deploy a honepot usng the Modern Honey Network (MHN) netwok and collect data about the attack.
For this, we had to set up two VM's: one was the admin VM and the other was the honeypot VM

We used the Google Cloud Platform (GCP to set everything up. This was done by following the instructions given in the assignmnet for week 9. 
Another resource used was [this link](https://hackmd.io/s/SkWWWHa0W) to set everything up, as well as to export the data

## Results

Honeypot deployed: Dionaea with HTTP

Total number of attacks: > 37,500

Most attacked port: 3389

Gif showing results:
<img src="https://github.com/mpai000/websec_week9/blob/master/honeypot1.gif">

There is also a session.json file, which is an export of the data collected from the honeypot.

## Issues encountered

While creating the firewall, I initially kept getting errors. However the way to fix this was by
'''
git auth login
'''
to get the correct authorization needed.

The first time I deployed my honeypot, no attackes were observed, ad I couldn't run the nmap command successfully on my terminal. I'm not sure as to why that occurred. However, wehn I deleted my VM's and basically ran through the step again to set it up, it worked properly.
