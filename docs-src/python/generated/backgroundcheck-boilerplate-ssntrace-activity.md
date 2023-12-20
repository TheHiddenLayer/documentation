---
id: backgroundcheck-boilerplate-ssntrace-activity
title: Boilerplate Activity code
sidebar_label: Activity code
description: In the Temporal Python SDK programming model, an Activity is an function.
tags:
- go sdk
- code sample
- activity
---

<!-- DO NOT EDIT THIS FILE DIRECTLY.
THIS FILE IS GENERATED from https://github.com/temporalio/documentation-samples-python/blob/main/backgroundcheck_boilerplate/activities/ssntraceactivity_dacx.py. -->

In the Temporal Python SDK programming model, an Activity is a function and can be used as an instance method of a class
You can use asynchronous, synchronous multithreaded, and synchronous multiprocess/other functions to define an Activity.

Below is an example of an Activity defined as a function.

<div class="copycode-notice-container"><div class="copycode-notice"><img data-style="copycode-icon" src="/icons/copycode.png" alt="Copy code icon" /> Sample application code information <img id="i-id80770576" data-event="clickable-copycode-info" data-style="chevron-icon" src="/icons/chevron.png" alt="Chevron icon" /></div><div id="copycode-info-id80770576" class="copycode-info">The following code sample comes from a working and tested sample application. The code sample might be abridged within the guide to highlight key aspects. Visit the source repository to <a href="https://github.com/temporalio/documentation-samples-python/blob/main/backgroundcheck_boilerplate/activities/ssntraceactivity_dacx.py">view the source code</a> in the context of the rest of the application code.</div></div>

```python
from temporalio import activity



@activity.defn
async def ssn_trace_activity(ssn) -> str:
    return "pass"
```