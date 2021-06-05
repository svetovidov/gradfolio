---
layout: post
title: TarSpark
description: Towards efficient debugging in DISC systems
---

![image](/assets/images/bigdata4.png)

Many real-world tasks rely on massive amounts of data nowadays, and using Data-Intensive Scalable Computing (DISC) systems such as Apache Spark is necessary. However, debugging of such systems remains a challenging task due to the parallel and distributed nature of processes in DISC systems.

This project is our attempt to make fault localization in distributed systems faster and more reliable. We integrated the spectra-based technique called Tarantula ([paper](https://dl.acm.org/doi/10.1145/1101908.1101949){:target="_blank"}) into the weather data analysis parallel [pipeline](https://github.com/maligulzar/bigdebug/tree/titian-bigsift/examples/src/main/scala/org/apache/spark/examples/bigsift/benchmarks/weather){:target="_blank"}). This method identifies the line of code causing an error by finding the line with the highest proportion of fail test cases went through it to passing test cases. In order to do this, we aggregate the trace of passed/failed test cases for each line of code and calculate the "suspiciosuness" score.

My contribution is as follows:

	* Co-implemented fail/pass aggregation method
	* Automated collection of line numbers
	* Evaluated the system performance

Project [repo](https://github.com/brendanmolin/TarSpark){:target="_blank"}

*Tools used: Java, Scala, Git*