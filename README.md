![photo_2025-04-11 16 03 37](https://github.com/user-attachments/assets/a5497320-59a2-46fc-95bc-d15adc716cb5)
![photo_2025-04-11 16 03 33](https://github.com/user-attachments/assets/09e5e79a-56fe-4ee4-9862-3e7e04ce768b)
![photo_2025-04-11 16 03 30](https://github.com/user-attachments/assets/fddf4cbd-74d3-429d-9969-ae99f1b86c1d)
![photo_2025-04-11 16 03 23](https://github.com/user-attachments/assets/13ced6f9-ff14-4d5c-ac29-2f4feb291c1d)
![photo_2025-04-11 16 03 26](https://github.com/user-attachments/assets/2f70e270-8ce8-4bf0-9bb4-5d5f9a93fc07)
![photo_2025-04-11 16 03 19](https://github.com/user-attachments/assets/06bd6def-b345-4792-b3eb-db019c2071d2)
![photo_2025-04-11 16 03 14](https://github.com/user-attachments/assets/2f4ccbb8-968f-4f47-afb9-182e10c87b90)
# network-analysis
network analysis using wireshark
Company had an incident of data exfiltration and as a member of network analysis team packets were captured during the incident and now we are to analyze and determine who triggered this incident what happened, when and where the incident took place and why the incident occured.
A total of 4509 packets where captured during this incident,during the analysis of the packets received we had noticed a communication between the sever and unknow client on http protocol thus followed up on the http stream of the packet, upon following the http stream of packet number 8 we could tell a document had been moved  thus filtered the packets by http request or response or tls handshake and not ssdp(as there is barely any information on this particular protocol)
after using the filter packet no 45 had been communicating and contained the same ip has packet no 8 which had shown a file was moved, we then followed http stream on this packet number and found out it had a dll attachment file, we then went to check files and saw the host name in the packet and downloaded the file in documents.
after downloading in documents we created a hash value for the file and then checked in on the hashvalue on virustotal.com and found out it was a malicious and concluded in happened in the mail and the mac address of 00:08:02:1c:47;ae was the client who triggered the incident in which mac address of 20:e5:2a:b6:93;f1 had clicked an email sent from the client and this incident took place 16:41:45 GMT and this incident happened due to negligence of the department and now the team has anforced the check policy of malwares before opening of any mail.
