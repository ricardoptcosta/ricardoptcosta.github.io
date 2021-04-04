---
layout: post
author: ricardo
title: What is the difference between observability and monitoring?
completedness: Needs final touches
---

Monitoring:
  - We monitor applications to detect known failures (problems like storage running out of disk space or failure from an I/O bound service)
  - For unknown unknowns or unpredicted failures, monitoring is not enough.

Observability:  
  - Originated from control theory, measures how well you can understand a system’s internal states from its external outputs.
  - Observability provides insights that aid monitoring. Monitoring is what you do after a system is observable.
  - Observability helps you find answers to questions like:
    - What services did a request go through, and what were the performance bottlenecks?
    - How was the execution of the request different from the expected system behavior?
    - Why did the request fail?
    - How did each microservice process the request?
  - Three observability pillars:
    - Logs
    - Metrics (foundation of monitoring)
    - Traces

References:
https://www.thundra.io/hubfs/WP-%20Monitoring%20vs%20Observability/WP-MO.pdf


