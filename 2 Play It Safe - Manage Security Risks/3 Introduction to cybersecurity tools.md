## Common types of logs

- Firewall log: Attempted / established connections for incoming / outgoing requests
- Network log: Log of all connections / devices entering & leaving
- Server log: Actions by services etc

## SIEM tools

- Collect and analyse log data
- Can also be used to create dashboards
- Can also tracks metrics like response time, availability, etc

## SIEM location

- Self-hosted: Locally operated, duh. Good when need to own & control data
- Cloud-hosted: Operated by the org, accessed over internet
- Hybrid: Mixture of slf & cloud hosted.
- Cloud-native: Operated by third party (e.g. Google)

"Security orchestration, automation, and response" (SOAR) is the name for automatically responding to events.

## SIEM examples

### Splunk

- I've used it!
- Splunk Enterprise: Self hosted
- Splunk Cloud: Cloud hosted

#### Dashboards

- Security posture: Displays notable security related events.
- Executive summary: Overall health over time.
- Incident review: Highlights higher risk items that need attention.
- Risk analysis: Shows changes in risk related activity.

### Google Chronicle

- Cloud native

#### Dashboards

- Data ingestion & health: Shows data being ingested.
- IOC matches: Shows top threats / risks / vulns.
- Main: Shows overall sumary.
- Rule detections: Show stats around incidents that are notable.

## Suricata

- Open source network analysis and threat detection software.
  - <https://en.wikipedia.org/wiki/Suricata_(software)>
  - <https://github.com/OISF/suricata>

## Feedback

Second module, still LOTS of focus on individual stories, how you "don't need x", whether that's maths, coding, etc.

Presumably it's to keep those from a less typical background interested, although even I've noticed ~80% of the interviews are with women, as are all the course leaders! There is as much focus on diversity / individual's backgrounds as the actual technical content. Very odd.
