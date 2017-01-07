# TA-w32time for Splunk

This CIM compliant TA can be used with Splunk (Enterprise Security) and provides
field extractions, aliases, eventtypes and tags for w32tm debug logging.
It provides an alternative to using script://win_timesync_status.bat

It extracts fields and maps to the following Splunk CIM datamodels:

- Performance -> OS -> Timesync

## Installation

Install this TA on your Splunk (Enterprise Security) search head, indexers and
Windows server. Make sure to name it TA-w32time otherwise ES won't eat it. 

## Configuration

This TA expects w32time debug logging to be sourcetyped `w32time`.  If you use a
different sourcetype, you should change `props.conf` accordingly in this TA.

