# lolc2-detections
detection rules for attackers leveraging legitimate services for command and control. DO NOT USE ALL THESE RULES!!1 Most of the Suricata rules are crap if you typically use that service in your network.

# Credit
- All credit to the lolc2 contributors (listed below 04/11/2025) for the research
- https://github.com/mthcht
- https://github.com/socketz
- https://github.com/mattdepaepezurich
- [sid ranges](https://community.emergingthreats.net/t/signature-id-allocation-ranges/491) from rgonzalez at the ET Team

# delete me after done
- testing rules `cls; cmd /c "C:\Program Files\Suricata\suricata.exe" -c .\suricata.yaml -T`
```
alert any any -> any any (msg:""; <insert rule>; classtype:command-and-control; sid:1000000; rev:1; reference:url,https://lolc2.github.io/; metadata:created_at 2025_04_11, confidence Medium, signature_severity Medium, updated_at 2025_04_11;)
```

# Rule Status
| LOLC2 Method                      | Rule Type | Number, Range of IDs | Rule File Path                                          |
| ---                               | ---       | ---                  | ---                                                     |
| Telegram                          | Suricata  | 3, 1000000-1000002   | rules/suricata/1_telegram_lolc2.rules                   |
| CounterStrike 1.6                 | Suricata  | 2, 1000010-1000011   | rules/suricata/2_counterstrike1_6_lolc2.rules           |
| CloudfLare                        | Suricata  | 8, 1000020-1000027   | rules/suricata/3_cloudflare_lolc2.rules                 |
| Strava                            | Suricata  | 6, 1000030-1000035   | rules/suricata/4_strava_lolc2.rules                     |
| Google Translate                  | Suricata  | 5, 1000040-1000044   | rules/suricata/5_google_translate_lolc2.rules           |
| Mastodon                          | Suricata  | 2, 1000050-1000051   | rules/suricata/6_mastodon_lolc2.rules                   |
| WhatsApp                          | Suricata  | 8, 1000060-1000067   | rules/suricata/7_whatsapp_lolc2.rules                   |
| Microsoft Printer                 | Suricata  | 3, 1000070-1000072   | rules/suricata/8_microsoft_printer_lolc2c2.rules        |
| Microsoft Azure Application Proxy | Suricata  | 7, 1000080-1000086   | rules/suricata/9_microsoft_azure_app_proxy_lolc2.rules  |
| Asana                             | Suricata  | 3, 1000090-1000093   | rules/suricata/10_asana_lolc2.rules                     |
| X (twitter)                       | Suricata  | 6, 1000100-1000105   | rules/suricata/11_x_lolc2.rules                         |
| OneDrive                          | Suricata  | 7, 1000110-1000116   | rules/suricata/12_onedrive_lolc2.rules                  |
| Microsoft Tasks                   | Suricata  | 4, 1000120-1000123   | rules/suricata/13_microsoft_tasks_lolc2.rules           |
| Jira                              | Suricata  | 3, 1000130-1000132   | rules/suricata/14_jira_lolc2.rules                      |
| Twitter (X)                       | Suricata  | 3, 1000140-1000142   | rules/suricata/15_twitter_lolc2.rules                   |
| Gmail                             | Suricata  | 0, 1000150-1000150   | rules/suricata/16_gmail_lolc2.rules                     |
| Slack                             | Suricata  | 0, 1000160-1000160   | rules/suricata/17_slack_lolc2.rules                     |
| Cisco Webex                       | Suricata  | 0, 1000170-1000170   | rules/suricata/18_cisco_webex_lolc2.rules               |
| DuckDuckGo                        | Suricata  | 0, 1000180-1000180   | rules/suricata/19_duckduckgo_lolc2.rules                |
| Microsoft Graph                   | Suricata  | 0, 1000190-1000190   | rules/suricata/20_microsoft_graph_lolc2.rules           |
| Microsoft Outlook                 | Suricata  | 0, 1000200-1000200   | rules/suricata/21_microsoft_outlook_lolc2.rules         |
| Microsoft Power Automate          | Suricata  | 0, 1000210-1000210   | rules/suricata/22_microsoft_power_automate_lolc2.rules  |
| Microsoft Azure Functions         | Suricata  | 0, 1000220-1000220   | rules/suricata/23_microsoft_azure_functions_lolc2.rules |
| SoundCloud                        | Suricata  | 0, 1000230-1000230   | rules/suricata/24_soundcloud_lolc2.rules                |
| Spotify                           | Suricata  | 0, 1000240-1000240   | rules/suricata/25_spotify_lolc2.rules                   |
| Microsoft Teams                   | Suricata  | 0, 1000250-1000250   | rules/suricata/26_microsoft_teams_lolc2.rules           |
| Discord                           | Suricata  | 0, 1000260-1000260   | rules/suricata/27_discord_lolc2.rules                   |
