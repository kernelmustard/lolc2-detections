# lolc2-detections
detection rules for attackers leveraging legitimate services for command and control

# Credit
- All credit to the lolc2 contributors (listed below 04/11/2025) for the research
- https://github.com/mthcht
- https://github.com/socketz
- https://github.com/mattdepaepezurich
- [sid ranges](https://community.emergingthreats.net/t/signature-id-allocation-ranges/491) from rgonzalez at the ET Team

# delete me after done
- testing rules `"C:\Program Files\Suricata\suricata.exe" -T -c suricata.yaml`
```
alert any any -> any any (msg:""; <insert rule>; classtype:command-and-control; sid:1000000; rev:1; reference:url,https://lolc2.github.io/; metadata:created_at 2025_04_11, confidence Medium, signature_severity Medium, updated_at 2025_04_11;)
```

# Rule Status
## telegram
### Tested and Passed
### Untested
- 3 suricata rules, 1000000-1000003, suricata/telegram_c2.rules

## counterstrike 1.6
### Tested and Passed
### Untested
- 2 suricata rules, 1000010-1000011, suricata/counterstrike1_6_c2.rules

## cloudflare
### Tested and Passed
### Untested

## strava
### Tested and Passed
### Untested

## google translate
### Tested and Passed
### Untested

## mastodon
### Tested and Passed
### Untested

## whatsapp
### Tested and Passed
### Untested

## microsoft printer
### Tested and Passed
### Untested

## microsoft azure application proxy
### Tested and Passed
### Untested

## asana
### Tested and Passed
### Untested

## x
### Tested and Passed
### Untested

## onedrive
### Tested and Passed
### Untested

## microsoft tasks
### Tested and Passed
### Untested

## jira
### Tested and Passed
### Untested

## twitter
### Tested and Passed
### Untested

## gmail
### Tested and Passed
### Untested

## slack
### Tested and Passed
### Untested

## cisco webex
### Tested and Passed
### Untested

## duckduckgo
### Tested and Passed
### Untested

## microsoft graph
### Tested and Passed
### Untested

## microsoft outlook
### Tested and Passed
### Untested

## microsoft power automate
### Tested and Passed
### Untested

## microsoft azure functions
### Tested and Passed
### Untested

## soundcloud
### Tested and Passed
### Untested

## spotify
### Tested and Passed
### Untested

## microsoft teams
### Tested and Passed
### Untested

## discord
### Tested and Passed
### Untested