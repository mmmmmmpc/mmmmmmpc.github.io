---
title: "Agentic AI on SLES 16: Getting Started with mcphost"
date: 2026-02-06
description: "Explore the new Agentic AI capabilities in SLES 16 using mcphost and the Model Context Protocol (MCP)."
excerpt: "Learn how mcphost and MCP enable Agentic AI to troubleshoot and analyze SLES 16 systems effectively."
layout: single
header:
  teaser: "/assets/images/miguel_pc-square-mini.jpg"
categories: [Linux, AI]
tags: [Linux, AI, SLES16]
---

Technology should serve people, and sometimes that means giving our systems tools to help us troubleshoot and understand them. In SLES 16, we've introduced **mcphost**, which implements the Model Context Protocol ([MCP](https://en.wikipedia.org/wiki/Model_Context_Protocol)). This protocol is an open standard that enables connecting different capabilities to [Large Language Models or LLMs](https://en.wikipedia.org/wiki/Large_language_model).

I’ve put together two videos to show you how this bridge between Linux and AI actually works. 

### Part 1: Installation and the Power of Context

In the first video, I walk through how simple it is to get started. We believe that powerful tools shouldn't be difficult to set up.

* **Simple Setup:** I show how you can install `mcphost` with a single `zypper` command [00:01:02].
* **The "Brain" Connection:** We look at the minimal configuration needed—just a few lines in a YAML file and an API key from Google AI Studio [00:01:32].
* **A Clever Trick:** I demonstrate a "pipe trick" [00:04:49] where we pass the output of `ps awx` directly to the AI. It’s amazing to see the AI analyze the running processes and give helpful advice on system health and hardening [00:06:58].

**Watch Part 1 here:** [SLES 16 - Install and Intro AI - MCP demo](https://youtu.be/7qep_-89wMw)
<iframe width="560" height="315" src="https://www.youtube.com/embed/7qep_-89wMw?si=BkaYZkq0uqvZ4Lx9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Part 2: Agentic AI and the Filesystem

The second video goes deeper into "Agentic AI." This is where the AI becomes more than a chatbot; it becomes an agent that can safely explore your system to find problems. To do that we configure MCP servers to provide read-only access to important parts of the filesystem.

* **Configuring Access:** I show how to set up MCP servers to give the AI read-only access to critical areas like `/etc`, `/var/log`, and `/proc` [00:01:42].
* **Proactive Analysis:** You can watch as the AI automatically inspects system services like Apache and Tomcat [00:03:52].
* **The "Aha!" Moment:** In a real-world troubleshooting demo, the AI detects a missing JAR file that was preventing Tomcat from starting correctly [00:07:13]. It didn't just guess; it "looked" at the logs and found the root cause.

**Watch Part 2 here:** [Agentic AI demo with MCP host in SLES 16](https://youtu.be/ZDQwIqFeY_4)

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZDQwIqFeY_4?si=4LaP38KTSVprF-I7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Why This Matters

We put a lot of care into ensuring that SLES 16 isn't just "another release," but a platform that embraces the future. By bringing Agentic AI closer to the OS, in an open and standardized manner, we are making it easier for everyone—from students to experts—to keep their systems resilient and secure.

If you have a chance to try `mcphost` on SLES 16, I'd love to hear about the "aha!" moments you discover.

Happy hacking!

— M*
