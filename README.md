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

# Rule Catalog
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
| Gmail                             | Suricata  | 4, 1000150-1000153   | rules/suricata/16_gmail_lolc2.rules                     |
| Slack                             | Suricata  | 3, 1000160-1000162   | rules/suricata/17_slack_lolc2.rules                     |
| Cisco Webex                       | Suricata  | 1, 1000170-1000170   | rules/suricata/18_cisco_webex_lolc2.rules               |
| DuckDuckGo                        | Suricata  | 3, 1000180-1000182   | rules/suricata/19_duckduckgo_lolc2.rules                |
| Microsoft Graph                   | Suricata  | 4, 1000190-1000193   | rules/suricata/20_microsoft_graph_lolc2.rules           |
| Microsoft Outlook                 | Suricata  | 4, 1000200-1000203   | rules/suricata/21_microsoft_outlook_lolc2.rules         |
| Microsoft Power Automate          | Suricata  | 1, 1000210-1000210   | rules/suricata/22_microsoft_power_automate_lolc2.rules  |
| Microsoft Azure Functions         | Suricata  | 0, 1000220-1000220   | rules/suricata/23_microsoft_azure_functions_lolc2.rules |
| SoundCloud                        | Suricata  | 3, 1000230-1000232   | rules/suricata/24_soundcloud_lolc2.rules                |
| Spotify                           | Suricata  | 5, 1000240-1000244   | rules/suricata/25_spotify_lolc2.rules                   |
| Microsoft Teams                   | Suricata  | 3, 1000250-1000252   | rules/suricata/26_microsoft_teams_lolc2.rules           |
| Discord                           | Suricata  | 3, 1000260-1000262   | rules/suricata/27_discord_lolc2.rules                   |
| Splunk                            | Suricata  | 0, 1000270-1000270   | rules/suricata/28_splunk_lolc2.rules                    |
| Lichess                           | Suricata  | 4, 1000280-1000283   | rules/suricata/29_lichess_lolc2.rules                   |
| Mattermost                        | Suricata  | 1, 1000290-1000290   | rules/suricata/30_mattermost_lolc2.rules                |
| Google Sheets                     | Suricata  | 0, 1000300-1000300   | rules/suricata/31_google_sheets_lolc2.rules             |
| Microsoft Sharepoint              | Suricata  | 0, 1000310-1000310   | rules/suricata/32_microsoft_sharepoint_lolc2.rules      |
| Google Drive                      | Suricata  | 0, 1000320-1000320   | rules/suricata/33_google_drive_lolc2.rules              |
| Google Calendar                   | Suricata  | 0, 1000330-1000330   | rules/suricata/34_google_calendar_lolc2.rules           |
| Google Slides                     | Suricata  | 0, 1000340-1000340   | rules/suricata/35_google_slides_lolc2.rules             |
| GitHub                            | Suricata  | 0, 1000350-1000350   | rules/suricata/36_github_lolc2.rules                    |
| YouTube                           | Suricata  | 0, 1000360-1000360   | rules/suricata/37_youtube_lolc2.rules                   |
| Pastebin                          | Suricata  | 0, 1000370-1000370   | rules/suricata/38_pastebin_lolc2.rules                  |
| Reddit                            | Suricata  | 0, 1000380-1000380   | rules/suricata/39_reddit_lolc2.rules                    |
| Dropbox                           | Suricata  | 0, 1000390-1000390   | rules/suricata/40_dropbox_lolc2.rules                   |
| Instagram                         | Suricata  | 0, 1000400-1000400   | rules/suricata/41_instagram_lolc2.rules                 |
| Zoom                              | Suricata  | 0, 1000410-1000410   | rules/suricata/42_zoom_lolc2.rules                      |
| Virustotal                        | Suricata  | 0, 1000420-1000420   | rules/suricata/43_virustotal_lolc2.rules                |
| Zulip                             | Suricata  | 0, 1000430-1000430   | rules/suricata/44_zulip_lolc2.rules                     |
| Notion                            | Suricata  | 0, 1000440-1000440   | rules/suricata/45_notion_lolc2.rules                    |
| Matrix                            | Suricata  | 0, 1000450-1000450   | rules/suricata/46_matrix_lolc2.rules                    |
| OpenAI                            | Suricata  | 0, 1000460-1000460   | rules/suricata/47_openai_lolc2.rules

# TODO
- review all suricata rule severity and confidence levels
- review all LOLC2 projects more thoroughly for network indicators