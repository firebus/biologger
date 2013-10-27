biologger
=========
Author: Ed Hunsinger

Biologger is intended to be a simple to use life logging tool for quantified
self sort of tracking. It's being designed primarily for my own use, but may
be useful for others.

My goals:
* Should be easy and quick to use on an iPhone.
* User interface is bare bones for data input.
* Does not provide any analysis of data, merely records it.
* Logs to text files that are consumable by Splunk Storm.

## Dependencies

This does use iWebKit, whose Framework/ directory which should be placed in iwebkit/ (or appropriate files
should be updated with the correct path).
iWebKit is available here: http://snippetspace.com/portfolio/iwebkit/

## Tracking events

Biologger can track two types of events:

### Activities

* Activities are events with a count - like number of reps or number of miles run.
* The list of Activities is configured in valid_activities.bio

### One-touch activities

* One-touch activities don't have a count.
* The list of One-touch activities is configured in valid_onetouch.bio

## Configuration

* Copy settings_example.php to settings.php and set a location for the activities, one-touch, and log file.
* Enter the list of activities and one-touch activities you want to track in the .bio files, one activity per line 

## Disclaimers

Please note: Security is not implemented in this on purpose for ease of use.
Security is up to the user if this is used on a publicly available server