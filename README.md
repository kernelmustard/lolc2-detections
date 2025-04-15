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
- 3 suricata rules, 1000000-1000003, suricata/telegram_c2.rules

## counterstrike 1.6
- 2 suricata rules, 1000010-1000011, suricata/counterstrike1_6_c2.rules

## cloudflare
- 8 suricata rules, 1000020-10000027, suricata/cloudflare_c2.rules

## strava
- 6 suricata rules, 1000030-1000035, suricata/strava_c2.rules

## google translate
- 8 suricata rules, 1000040-1000047, suricata/google_translate_c2.rules

## mastodon
- 2 suricata rules, 1000050-1000051, suricata/mastodon_c2.rules

## whatsapp


## microsoft printer


## microsoft azure application proxy


## asana


## x


## onedrive


## microsoft tasks


## jira


## twitter


## gmail


## slack


## cisco webex


## duckduckgo


## microsoft graph


## microsoft outlook


## microsoft power automate


## microsoft azure functions


## soundcloud


## spotify


## microsoft teams


## discord
