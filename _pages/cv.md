---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Tianjin, Nankai University, 2022
* B.S. in Tianjin, Nankai University, 2018

Work experience
======
* SEPT.2023 - DEC.2023: System Engineer Intern
  * Zhiyuan Research Institute, Hangzhou
  * Duties includes: Deployment and optimization of object detecting algorithm on embedded platform
    * Based on HUAWEI Atlas 200I A2 platform, developed inference application of yolov5 with NPU
    * Improved end-to-end performance from 20FPS to 30FPS on the embedded platform with multi-threaded pipeline

* JUL.2021 - SEPT.2021: System Engineer Intern
  * Alibaba Cloud, Shanghai
  * Duties included: Security container and OS kernel development with Rust
    * Developed Linux kernel with Rust. Rewrote the PCIe device registry process in Hypervisor
    * Realized the passthrough of the PCIe devices and hotplug of NVIDIA GPUs in the security container
  
Skills
======
* C/C++
* CUDA
* Linux

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  

