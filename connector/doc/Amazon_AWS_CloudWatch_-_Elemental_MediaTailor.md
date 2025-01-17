---
uid: Connector_help_Amazon_AWS_CloudWatch_-_Elemental_MediaTailor
---

# Amazon AWS CloudWatch - Elemental MediaTailor

You can monitor AWS Elemental MediaTailor metrics using CloudWatch. CloudWatch collects raw data and processes it into readable, near real-time metrics. These statistics are kept for 15 months, so that you can access historical information and gain a better perspective on how your web application or service is performing. You can also set alarms that watch for certain thresholds, and send notifications or take actions when those thresholds are reached.

## About

### Version Info

| **Range** | **Key Features** | **Based on** | **System Impact** |
|-----------|------------------|--------------|-------------------|
| 1.0.1.x   | Initial version  | \-           | \-                |

### Product Info

| Range     | Supported Firmware     |
|-----------|------------------------|
| 1.0.1.x   | \-                     |

### System Info

| Range     | DCF Integration     | Cassandra Compliant     | Linked Components     | Exported Components     |
|-----------|---------------------|-------------------------|-----------------------|-------------------------|
| 1.0.1.x   | No                  | Yes                     | \-                    | \-                      |

## Configuration

This connector is automatically generated by the connector [Amazon AWS CloudWatch](xref:Connector_help_Amazon_AWS_CloudWatch), range 1.0.1.x.

### Connections

#### Virtual Connection

This connector uses a virtual connection and does not require any input during element creation.

## How to Use

The element created with this connector consists of the following data pages:

- **General**: Contains the **Entry ID**, which is a unique identifier for this service. The **Entry Type** provides more insight in the different parts that the Entry ID consists of. The **Polling Interval** can be modified on this page and the **Entry Status** indicates if the service entry is still present. With the **Force Polling** button, you can poll the metrics immediately without having to wait until the interval time has elapsed.
- **Metrics**: The various Metrics pages contain all polled metric values. Polling of the appropriate metric can be enabled via the **Config Poll** page button. It is not possible to set the Poll parameter to *Enabled* for metric parameters that have the *N/A* value. These *N/A* metrics are not present in the provided metrics list for this instance and hence their Poll parameter will remain *Disabled*.
