"Monitoring has become an umbrella term whose meaning strongly depends on the context. 
Most broadly, it refers to the process of becoming aware of the state of the system. 
This is done in two ways, proactive and reactive.
The former involves watching visual indicators, such as timeseries and dashboard, and is sometimes what administrators mean by _monitoring_.
The latter involves automated ways to deliver notifications to operators in order to bring to their attention a grace change 
in system's state; this is usually referred to as _alerting_"

"Monitoring is the process of maintaining surveillance over the existence and magnitude of state change and data flow in a system. Monitoring aims to identify faults and assist in their subsequent elimination. The techniques used in monitoring of information systems intersect the fields of real-time processing, statistics, and data analysis. A set of software components used for data collection, their processing, and presentation is called a monitoring system.
Alerting is the capability of a monitoring system to detect and notify the operators about meaningful events that denote a grave change of state. The notification is referred to as an alert and is a simple message that may take multiple forms: email, SMS, instant message (IM), or a phone call. The alert is passed on to the appropriate recipient, that is, a party responsible for dealing with the event. The alert is often logged in the form of a ticket in an Issue Tracking System (ITS), also referred to simply as ticketing system."

# Baselining

"Monitoring provides an immediate insight into a system’s current state. This data often takes quantitative form and, when recorded on timeseries, become a rich source of information for baselining.
Establishing standard performance levels is an important part of your job. It finds application in capacity planning, leads to formulation of data-backed Service-Level Agreements (SLAs) and, where inconsistencies are detected, can be a starting point for in-depth performance analysis."

# Metrics and Timeseries

"Watching and evaluating timeseries, chronologically ordered lists of data points, is at the core of both monitoring and alerting.
 
Monitoring consists of recording and analyzing quantitative inputs, that is, numeric measurements carrying information about current state and its most recent changes. Each data input comes with a number of properties describing it: the origin of the measurement and its attributes such as units and time at which sampling took place.
 
The inputs along with their properties are stored in the form of metrics. A metric is a data structure optimized for storage and retrieval of numeric inputs. The resulting collection of gathered inputs may be interpreted in many different ways based on the values of their assigned properties. Such interpretation allows a tool to evaluate the inputs as a whole as well as at many abstract levels, from coarse to fine granularity.
 
Data inputs extracted from selected metrics are further agglomerated into groups based on the time the measurement occurred. The groups are assigned to uniform intervals on a time axis, and the total of inputs in each group can be summarized by use of a mathematical transformation, referred to as a summary statistic. The mathematical transformation yields one numeric data point for each time interval. The collection of data points, a timeseries, describes some statistical aspect of all inputs from a given time range. The same set of data inputs may be used to generate different data points, depending on the selection of a summary statistic."

# Coverage

"Complete monitoring should cover three major groups of metrics: resource availability, software performance, and, where applicable, user behavior."

# Frequently Encountered Anomalies

"A flattening effect is manifested when the line on the plot reaches an artificially steady level, compared to historical data points (Figure 2-7). The effect may occur in many different types of metrics and for various reasons, but it almost never brings good news. It usually signifies a saturation of a resource or discontinuation of flow."

"Some concrete examples include:
 * A sudden flattening on a counter metric indicates a discontinuation of flow. Its rate of change series is equal to flow metric continuously recording a 0 value.
 * A flattening at 200 ms of p99 in a response time metric may be a fallout of high packet loss combined with a retransmission timeout setting of 200 ms.
 * Flat lines in CPU utilization point to resource saturation."
