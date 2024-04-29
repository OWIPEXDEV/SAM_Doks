|------------------------------------------------------------------------------|
| Grün: Information / Orientierung                                              |
| Gelb: Eingaben                                                               |
| Rot: Anzupassende Module                                                      |
|------------------------------------------------------------------------------|

 1. [Grün] ssh owipex_adm@192.168.100.100
 2. [Rot] @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
 3. [Rot] @    WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!     @
 4. [Rot] @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
 5. [Grün] IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!
 6. [Grün] Someone could be eavesdropping on you right now (man-in-the-middle attack)!
 7. [Grün] It is also possible that a host key has just been changed.
 8. [Grün] The fingerprint for the ECDSA key sent by the remote host is SHA256:2/CTidOk62JZa+L7dEl7DkRDLcvLIOasdw0T8V+lAag.
 9. [Grün] Please contact your system administrator.
10. [Grün] Add correct host key in C:\\Users\\owipexDoku/.ssh/known_hosts to get rid of this message.
11. [Rot] Offending ECDSA key in C:\\Users\\owipexDoku/.ssh/known_hosts:1
12. [Grün] ECDSA host key for 192.168.100.100 has changed and you have requested strict checking.
13. [Grün] Host key verification failed.
14. [Grün] rm C:\\Users\\owipexDoku/.ssh/known_hosts
15. [Grün] ssh owipex_adm@192.168.100.100
16. [Grün] The authenticity of host '192.168.100.100 (192.168.100.100)' can't be established.
17. [Grün] ECDSA key fingerprint is SHA256:2/CTidOk62JZa+L7dEl7DkRDLcvLIOasdw0T8V+lAag.
18. [Grün] Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
19. [Grün] Warning: Permanently added '192.168.100.100' (ECDSA) to the list of known hosts.
20. [Gelb] owipex_adm@192.168.100.100's password: OW!p3x?
21. [Grün] Welcome to Ubuntu 22.04.3 LTS (GNU/Linux 5.15.0-94-generic x86_64)
22. [Grün]  * Documentation:  https://help.ubuntu.com
23. [Grün]  * Management:     https://landscape.canonical.com
24. [Grün]  * Support:        https://ubuntu.com/advantage
25. [Grün] This system has been minimized by removing packages and content that are
26. [Grün] not required on a system that users do not log into.
27. [Grün] To restore this content, you can run the 'unminimize' command.
28. [Grün] Last login: Wed Mar  6 08:31:13 2024 from 192.168.100.185
29. [Grün] Prüfen ob /owipex ordner in /etc vorhanden ist wenn ja klammer ausführen
30. [Grün] (
31. [Grün] owipex_adm@9240021:~$ sudo rm -r /etc/owipex/
32. [Gelb] [sudo] password for owipex_adm: OW!p3x?
33. [Grün] Steuerung ausstecken und erneut starten
34. [Grün] )
35. [Grün] owipex_adm@9240021:~$ dir
36. [Grün] owipex-sps  total_flow.json
37. [Grün] owipex_adm@9240011:~$ dir
38. [Grün] owipex-sps
39. [Grün] owipex_adm@9240011:~$ sudo rm -r owipex-sps/
40. [Gelb] [sudo] password for owipex_adm: OW!p3x?
41. [Grün] owipex_adm@9240011:~$ dir
42. [Grün] owipex_adm@9240011:~$ git clone https://github.com/KARIM-Technologies/owipex-sps.git
43. [Grün] Cloning into 'owipex-sps'...
44. [Grün] remote: Enumerating objects: 721, done.
45. [Grün] remote: Counting objects: 100% (351/351), done.
46. [Grün] remote: Compressing objects: 100% (210/210), done.
47. [Grün] remote: Total 721 (delta 173), reused 281 (delta 135), pack-reused 370
48. [Grün] Receiving objects: 100% (721/721), 183.59 KiB | 564.00 KiB/s, done.
49. [Grün] Resolving deltas: 100% (338/338), done.
50. [Grün] owipex_adm@9240011:~$ dir
51. [Grün] owipex-sps
52. [Grün] owipex_adm@9240011:~$ cd owipex-sps/installer/initial/
53. [Grün] owipex_adm@9240023:~/owipex-sps/installer/initial$ dir
54. [Grün] adaptSkript.txt          autoInstallVirginSys.sh  initialScript.py.old  setupBot.py
55. [Grün] autInstallVirginSys.txt  bootSpeeder.sh           moveData.sh           workflow.txt
56. [Grün] owipex_adm@9240023:~/owipex-sps/installer/initial$ sudo chmod +x bootSpeeder.sh
57. [Grün] owipex_adm@9240023:~/owipex-sps/installer/initial$ sudo ./bootSpeeder.sh
58. [Rot] Job for systemd-networkd-wait-online.service failed because the control process exited with error code.
59. [Rot] See "systemctl status systemd-networkd-wait-online.service" and "journalctl -xeu systemd-networkd-wait-online.service" for details.
60. [Grün] Die Bootzeit-Konfiguration wurde aktualisiert. Timeout gesetzt auf 1s.
61. [Grün] owipex_adm@9240011:~$ /owipex-sps/installer/initial$ sudo python3 setupBot.py
62. [Gelb] [sudo] password for owipex_adm: OW!p3x?
63. [Gelb] Möchten Sie die Dateien jetzt verschieben? (ja/nein): ja
64. [Grün] Dateien werden verschoben...
65. [Grün] calibration_data.json wurde nach /etc/owipex verschoben.
66. [Grün] run_time.txt wurde nach /etc/owipex verschoben.
67. [Grün] total_flow.json wurde nach /etc/owipex verschoben.
68. [Grün] Setup abgeschlossen.
69. [Gelb] Bitte geben Sie den gewünschten Hostnamen ein (924XXXX): 9240011
70. [Grün] ** (generate:1376): WARNING **: 09:51:42.687: `gateway4` has been deprecated, use default routes instead.
71. [Grün] See the 'Default routes' section of the documentation for more details.
72. [Grün] ** (process:1374): WARNING **: 09:51:43.211: `gateway4` has been deprecated, use default routes instead.
73. [Grün] See the 'Default routes' section of the documentation for more details.
74. [Grün] ** (process:1374): WARNING **: 09:51:43.227: `gateway4` has been deprecated, use default routes instead.
75. [Grün] See the 'Default routes' section of the documentation for more details.
76. [Grün] ** (process:1374): WARNING **: 09:51:43.447: `gateway4` has been deprecated, use default routes instead.
77. [Grün] See the 'Default routes' section of the documentation for more details.
78. [Grün] ** (process:1374): WARNING **: 09:51:43.448: `gateway4` has been deprecated, use default routes instead.
79. [Grün] See the 'Default routes' section of the documentation for more details.
80. [Rot] Der Schlüssel wird unter edge verwalten -> Neue Nummer generiert
81. [Gelb] Bitte CLOUD_ROUTING_KEY eingeben: 3ad8ef42-5a7a-7464-5992-c329cdacd3c5
82. [Gelb] Bitte CLOUD_ROUTING_KEY eingeben:  wiederholen: 3ad8ef42-5a7a-7464-5992-c329cdacd3c5
83. [Gelb] Bitte CLOUD_ROUTING_SECRET eingeben: utb4nv6xzho6mp5i16xs
84. [Gelb] Bitte CLOUD_ROUTING_SECRET eingeben:  wiederholen: utb4nv6xzho6mp5i16xs
85. [Gelb] Bitte SPRING_DATASOURCE_PASSWORD eingeben: OW!p3x?
86. [Gelb] Bitte SPRING_DATASOURCE_PASSWORD eingeben:  wiederholen: OW!p3x?
87. [Grün] .env Datei existiert bereits.
88. [Grün] Erstelle Systemd-Service-Datei für powerWatchdog...
89. [Grün] Lade Systemd-Konfiguration neu...
90. [Grün] Aktiviere powerWatchdog Service...
91. [Grün] Starte powerWatchdog Service...
92. [Grün] powerWatchdog Service erfolgreich eingerichtet und gestartet.
93. [Grün] Anpassungen abgeschlossen.
94. [Gelb] Möchten Sie den Rechner jetzt neu starten? (ja/nein): ja
95. [Grün] Der Rechner wird neu gestartet...
96. [Grün] Connection to 192.168.100.100 closed by remote host.
97. [Grün] Connection to 192.168.100.100 closed.
98. [Grün] PS C:\\Users\\owipexDoku>
