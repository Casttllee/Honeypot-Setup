# Spiderfoot (OSINT)

## Objective

The primary objective of this lab is to equip participants with the knowledge and skills to utilize SpiderFoot, a powerful open-source intelligence (OSINT) automation tool, for comprehensive cybersecurity investigations. Through hands-on activities, participants will learn to install and configure SpiderFoot, execute various scans, and analyze the gathered intelligence to identify potential security threats and vulnerabilities. By the end of the lab, participants will be proficient in leveraging SpiderFoot to conduct detailed OSINT investigations, interpret the results, and generate actionable reports, thereby enhancing their ability to protect their organizations from cyber threats.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps

*Ref 1*
![up to date 1](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/bbb36144-42b5-4061-a85c-844d49f9a7b0)
  The first step was to update my VM and i did this by by updating my respitories and libraries by using the command "sudo apt-get update && sudo apt-get upgrade -y".

*Ref 2*
![install python pip 2](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/b77d697d-d79d-4ee6-a25e-514e178f5abb)
  I then installed the next preresquiete  Python 3 pip. After updating my respositories, libraries, and pip 3 I then began to install Spiderfoot

*Ref 3*
![spiderfoot github install](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/fe02ad35-ed50-4fed-b974-ddb3549f1f94)
  I started the installation of Spiderfoot by going to the Spierfoot Github page and scrolling down to the "Installing and Running" section. I then went to the "Stable build package release" and copied all of the commands except for the Python 3 command.

*Ref 4*
![spiderfoot good 4](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/9f163d78-6a25-415e-9112-7cb64412cf8d)
  After pasting the commands and the installation was complete, I then ran the last command manually to avoid any problems by typing "python3 ./sf.py -l 10.0.2.15:5001". The command includes my IP address for my Ubuntu machine. I did not use the last command on the Spiderfoot "Stable build package release" because the command is pointing to local host which is 127.0.0.1 which opens Spiderfoot from the host itself. Now Spiderfoot will work on my host machine.

*Ref 5*
![first visualization 5](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/21544b3a-27cd-4f9b-8664-4aeb1f1d039f)
  This screenshot shows me conected to the Spidefoot dashboard.

*Ref 6*
![account for api key 6](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/f817de48-1a74-4eb2-9853-bdf2fbb70e34)
  I then proceded to settings where I added in an API key for added functionality. I went to AbueIPDB where it requested an API key. I proceded to AbuseIPBD.com where I created an account and obtained an API key.

*Ref 7*
![api setting success 7](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/f7b55cfc-ef46-42b6-89e4-cfa2fb186cb6)
  Then, I entered my API key and saved the changes at the top left and it was shown successful.

*Ref 8*
![scan ipbd 8](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/eed3ab09-af93-4112-b710-8a85b53bd556)
  Afterwards I went to the scans section. I named my scan as "Test Scan" and put the scan target as the IP address 124.222.31.94. This IP address is from abuseIPDB for testing purposes. In the module section I deselected all the modules except for AbuseIPDB and ran my scan.

*Ref 9*
![first scan visual dashboard 9](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/4c1ac8aa-91e5-46ce-a5f6-ff85bf0a6bf2)
  This screenshot shows that the data types are an IP address.

*Ref 10*
![scan 2 investigate 10](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/74432157-0865-464c-86de-5460bdccaf1f)
  I then began to start a second scan. I ran this scan by use case Investigate and named it "Test Scan 2" with the same IP address.

*Ref 11*
![scan 2 visual](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/e0bbe072-f2d3-4dd3-ae8c-afd76134985c)
  The next

*Ref 12*
![scan 2 open port 11](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/4a2f3cfe-c47a-4751-993e-6f8173cd50ae)
  Next,

*Ref 13*
![browse second scan 12](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/e4acb1d4-8529-4de1-85f2-4e08ed578ed4)
  Next,

*Ref 14*
![ip visual map second scan 13](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/0057ab1b-b8c9-488f-9997-a7fe4aca91de)
  The last step

## Conclusion

