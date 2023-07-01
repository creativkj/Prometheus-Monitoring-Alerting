# Prometheus Monitoring and Alerting for Multiple EC2 Instances in Multiple Accounts with Slack Integration

## Technologies: EC2, Prometheus, Alert, Alert Manager, Slack

## Problem Statement: 
Our organization has a number of Amazon EC2 instances running in multiple accounts, and we need a way to monitor their status and receive alerts when any of them go down. We also want to be able to easily collaborate with our team members when issues arise. Currently, we do not have a reliable system in place to do this, and as a result, we are at risk of experiencing prolonged downtime and reduced visibility into the performance and health of our instances. To address this, we want to set up a Prometheus-based monitoring and alerting system that integrates with Slack, so that we can receive notifications when any of the instances go down and collaborate on resolving any issues that arise.

## Approach: 
**To create a Prometheus monitoring system for multiple Amazon Elastic Compute Cloud (EC2) instances in multiple accounts and send alerts to a Slack community when any of the servers are down, you will need to perform the following steps:**
1. Set up a Prometheus server on one of the EC2 instances. This can be done by following the instructions in the Prometheus documentation.
Set up one or more Prometheus exporters on each of the other EC2 instances that you want to monitor. An exporter is a piece of software that runs on a host and exposes metrics in a format that Prometheus can scrape. There are many exporters available for different types of systems, such as the Node Exporter for Linux servers and the MySQL Exporter for databases.
2. Configure the Prometheus server to scrape metrics from the exporters. This can be done by modifying the configuration file for the server and adding a job configuration for each exporter.
3. Set up an alerting rule in Prometheus to send a notification to a Slack channel when a server goes down. This can be done by modifying the configuration file for the server and adding an alerting rule that specifies the condition under which the alert should be triggered and the Slack webhook to which the alert should be sent.
4. Test the system to ensure that it is working as expected. This can be done by simulating a server failure and verifying that the alert is sent to the Slack channel.
## Results:
The result of setting up a Prometheus monitoring system for multiple EC2 instances in multiple accounts and sending alerts to a Slack community when any of the servers are down should be a system that can monitor the status of the EC2 instances and send notifications to the Slack channel if any of the servers are down. 

Some potential benefits of this system may include: 

**1.Improved uptime:** By monitoring the status of the EC2 instances and being alerted when any of them go down, you can take action to restore service as quickly as possible.

**2.Increased visibility:** The Prometheus server and exporters will collect a wide range of metrics about the performance and health of the EC2 instances, which can help you identify trends and issues that may not be immediately apparent.

**3.Enhanced collaboration:** By sending alerts to a Slack channel, you can make it easier for team members to stay informed about the status of the EC2 instances and collaborate on resolving any issues that arise.

Overall, the result of this system should be a more reliable, transparent, and collaborative way to manage the EC2 instances in your environment.



![instances](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/f40022e3-ce53-4f7b-a623-1507605ed18a)



![prom_instance](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/b9f4de3d-e7cf-4e62-be0b-314826a31caa)



![prometheus_status](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/43b19e80-889c-4194-89e3-db559d815ee7)



![node_exporter instance](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/a38fe945-8bf5-4c3a-b3cf-0084e4572532)



![node_exporter_status](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/da68bd77-b106-4743-9096-2cfe4199a6b9)



![node_exporter2_instance](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/6d1305f8-e154-420e-9e38-9c63e8931239)



![alerts_allUP](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/9d37ad7b-a836-4a1e-9ac1-b7f7fd4de45a)



![both node_exporter DOWN](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/528bf68c-b53d-4e85-9288-34912962f2cf)



![one node_exporter DOWN](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/fd890d5d-63b1-44df-ba39-8eb0e67f4978)



![slack](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/9aefa13e-4470-498a-bd35-d9a5dbc60265)



![slack_node_exporter DOWN](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/19bc686e-3aae-45e1-a18a-439f19cdda27)



![slack_resolved state](https://github.com/creativkj/Prometheus-Monitoring-Alerting/assets/121052351/f9ec3506-cc1c-4cd0-a340-475f18d9118c)




