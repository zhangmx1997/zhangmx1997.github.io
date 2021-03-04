---
permalink: /projects/
title: "Research Projects"
author_profile: true
redirect_from: 
  - /projects.html
---

## Investigating Click Interception on the Web

Time: 2018.02 -- 2018.11

Third-party scripts may intercept real user clicks to launch click ad frauds, or send malicious commands to other websites on behalf of the victim user. <br>
In this project, we developed a Chromium-based framework, Observer, for studying JavaScript click interception practices. It tracks the creation of HTML anchor and script elements, records the accesses to the anchor elements, and monitors event listeners. <br>
We used Observer to visit Alexa top 250K websites, and identified 3 techniques for interception user clicks: 1) modifiying the destination URL of hyperlinks, 2) adding event listeners and 3) visual deception (e.g., transparent overlay).<br>
Overall, we found third-party scripts intercepting user clicks on 613 websites, which receives 43 million visits per day.<br>
Our findings were published at Usenix Security Symposium 2019, and we have released our source code [here](https://github.com/cuhk-seclab/observer.git).

