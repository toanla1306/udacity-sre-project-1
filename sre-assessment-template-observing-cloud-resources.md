### Categorize Responsibilities
|Prometheus and Grafana Screenshots|
|---|
|Provide a screenshot of the Prometheus node_exporter service running on the EC2 instance. Use the following command to show that the system is running: sudo systemctl status node_exporter|
|---|
|![default ns](/image_screenshot/node_exporter_available.png)|
|---|


|Host Metric (CPU, RAM, Disk,  Network)|Dashboard|
|---|---|
|CPU Node|![default ns](/image_screenshot/cpu-node.png)|
|---|---|
|Available Memory Bytes|![default ns](/image_screenshot/available-memory-bytes.png)|
|---|---|
|Disk I/O|![default ns](/image_screenshot/disk-io.png)|
|---|---|
|Network Received in Bytes|![default ns](/image_screenshot/network-received-in-bytes.png)|
|---|---|

|Responsibilities|
|---|
|1. The development team wants to release an emergency hotfix to production. Identify two roles of the SRE team who would be involved in this and why.|
|---|
|DevOps and SysAdmin. Because DevOps Engineer will manage release and SysAdmin Engineer will monitoring the new hotfix will run well on production|
|---|
|2. The development team is in the early stages of planning to build a new product. Identify two roles of the SRE team that should be invited to the meeting and why.|
|---|
|DevOps and SysAdmin. Because SysAdmin have a knowledge about the architecture so they will provide solution faster and DevOps will know infrastructure that will map with the new feature and release more faster|
|---|
|3. The emergency hotfix from question 1 was applied and is causing major issues in production. Which SRE role would primarily be involved in mitigating these issues?|
|---|
|DevOps Engineer because the reponsibility of them is manage release, so they will know about the issue will be come from exactly role|


### Team Formation and Workflow Identification
|API Monitoring and Notifications|
|---|
|Display the status of an API endpoint: Provide a screenshot of the Grafana dashboard that will show at which point the API is unhealthy (non-200 HTTP code), and when it becomes healthy again (200 HTTP code).|
|---|
|![default ns](/image_screenshot/healthy-check.png)|
|---|
|Create a notification channel: Provide a screenshot of the Grafana notification which shows the summary of the issue and when it occurred.|
|---|
|![default ns](/image_screenshot/total-firing.png)|
|---|
|Configure alert rules: Provide a screenshot of the alert rules list in Grafana.|
|---|
|![default ns](/image_screenshot/alert-rule-list.png)|


### Applying the Concepts
|Graph 1|
|---|
|![default ns](/image_screenshot/graph-1-template.png)|
|---|
|4a. Given the above graph, where does it show that the API endpoint is down? Where on the graph does this show that the API is healthy again?|
|---|
|API endpoint is down at 15:28 and it healthy again at 15:37|
|---|
|4b. If there was no SRE team, how would this outage affect customers?|
|---|
|The API endpoint of customers will not be known and maybe the downtime will be more than the metrics|
|---|
|4c. What could be put in place so that the SRE team could know of the outage before the customer does?|
|---|
|I think the SRE team rely on metrics healthcheck of instance to know when server outage|
|---|
|Graph 2|
|---|
|![default ns](/image_screenshot/graph-2-template.png)|
|---|
|5a. Given the above graph, which instance had the increase in traffic, and approximately how many bytes did it receive (feel free to round)?|
|---|
|Reply|
|---|
|5b. Which team members on the SRE team would be interested in this graph and why?|
|---|
|Reply|