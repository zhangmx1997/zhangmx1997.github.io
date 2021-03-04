---
permalink: /projects/
title: "Research Projects"
author_profile: true
redirect_from: 
  - /projects.html
---
## Detecting and Studying JavaScript Global Identifier Conflicts

Time: 2019.01 -- 2020.03

Modern web browsers execute all scripts in the same execution context.
If a global identifier is defined in multiple scripts, the actual value/type would be unpredictable, leading to unexpected effects, e.g., type errors.<br>
In this project, we developed a Chromium-based framekwork, JSObserver, for detecting JavaScript global identifier conflicts on the web.<br>

JSObserver inserts additional JavaScript code to log the value, type and identifier name involved in each write operation.<br>
We used it to visit Alexa top 100K websites, and found conflicts on 31,615 websites. We further demonstrated the security risks introduced by these conflicts (e.g., a cookie-related function definition conflict could allow an attacker to manipulate the cookie values).<br>
Our findings were published at [ESEC/FSE 2020](https://zhangmx1997.github.io/papers/fse20_js_conflict.pdf), and we have released our tool and dataset [here](https://doi.org/10.5281/zenodo.3923232).

## Investigating Click Interception on the Web

Time: 2018.02 -- 2018.11

Web users commonly interact with web pages by clicking hyperlinks, or other HTML elements (e.g., buttons and images).
Third-party scripts may intercept real user clicks to launch click ad frauds, or send malicious commands to other websites on behalf of the victim user, e.g., by modifying the destination URL of hyperlinks, or tricking users into clicking certain elements. <br>
In this project, we developed a Chromium-based framework, Observer, for studying JavaScript click interception practices.<br> 

Observer tracks the creation of HTML anchor and script elements, records the accesses to the anchor elements, and monitors event listeners. <br>
We used Observer to visit Alexa top 250K websites, and identified 3 techniques for interception user clicks.<br>
Overall, we found third-party scripts intercepting user clicks on 613 websites, which receive 43 million visits per day.<br>
Our findings were published at [Usenix Security Symposium 2019](https://zhangmx1997.github.io/papers/sec19_click_interception.pdf), and we have released our source code [here](https://github.com/cuhk-seclab/observer.git).



