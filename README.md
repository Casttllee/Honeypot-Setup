# Spiderfoot (OSINT)

## Objective

The primary objective of this lab is to equip participants with the knowledge and skills to utilize SpiderFoot, a powerful open-source intelligence (OSINT) automation tool, for comprehensive cybersecurity investigations. Through hands-on activities, participants will learn to install and configure SpiderFoot, execute various scans, and analyze the gathered intelligence to identify potential security threats and vulnerabilities. By the end of the lab, participants will be proficient in leveraging SpiderFoot to conduct detailed OSINT investigations, interpret the results, and generate actionable reports, thereby enhancing their ability to protect their organizations from cyber threats.

### Skills Learned

- Cybersecurity Analysis: Understanding of cybersecurity tools and techniques for reconnaissance and threat assessment.
- Vulnerability Assessment: Identifying potential vulnerabilities through analysis of open ports and software versions.
- Correlation Analysis: Ability to correlate different data points to derive meaningful insights.
- Report Writing: Communicating findings effectively through written reports or summaries.
- API Integration: Experience in integrating and using APIs, such as AbuseIPDB, for obtaining data.

### Tools Used

- Spiderfoot: Used for automated reconnaissance and information gathering.
- Python 3 and pip: Used for managing Python packages and dependencies.
- Text Editor: Used for modifying configuration files, writing scripts, or editing command outputs.
- Linux Terminal: Utilized for running commands and managing system configurations.

## Steps

*Ref 1*
![up to date 1](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/bbb36144-42b5-4061-a85c-844d49f9a7b0)
  The first step was to update my VM. I did this by updating my repositories and libraries using the command 'sudo apt-get update && sudo apt-get upgrade -y'.

*Ref 2*
![install python pip 2](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/b77d697d-d79d-4ee6-a25e-514e178f5abb)
  I then installed the next prerequisite, Python 3 and pip. After updating my repositories, libraries, and pip3, I began installing Spiderfoot.

*Ref 3*
![spiderfoot github install](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/fe02ad35-ed50-4fed-b974-ddb3549f1f94)
  I started the installation of Spiderfoot by visiting the Spiderfoot GitHub page and scrolling down to the 'Installing and Running' section. Then, I navigated to the 'Stable build package release' section and copied all of the commands except for the Python 3 command.

*Ref 4*
![spiderfoot good 4](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/9f163d78-6a25-415e-9112-7cb64412cf8d)
  After pasting the commands and completing the installation, I manually ran the last command to avoid any problems by typing 'python3 ./sf.py -l 10.0.2.15:5001'. This command includes the IP address of my Ubuntu machine. I did not use the last command from the Spiderfoot 'Stable build package release' because it points to localhost (127.0.0.1), which opens Spiderfoot from the host itself. Now, Spiderfoot will work on my host machine.

*Ref 5*
![first visualization 5](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/21544b3a-27cd-4f9b-8664-4aeb1f1d039f)
  This screenshot shows me successfully connected to the Spiderfoot dashboard on my Ubuntu machine. It demonstrates that the installation was completed correctly and that Spiderfoot is running smoothly on my specified IP address, 10.0.2.15, and port 5001.

*Ref 6*
![account for api key 6](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/f817de48-1a74-4eb2-9853-bdf2fbb70e34)
  I then proceeded to the settings where I added an API key for additional functionality. I went to AbuseIPDB, which requested an API key. I created an account on AbuseIPDB.com and obtained the API key.

*Ref 7*
![api setting success 7](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/f7b55cfc-ef46-42b6-89e4-cfa2fb186cb6)
  Next, I entered my API key into the designated field and saved the changes by clicking the save button at the top left of the settings page. A confirmation message appeared, indicating that the API key was successfully added and the changes were saved. This confirmed that the integration with AbuseIPDB was correctly set up and functional.

*Ref 8*
![scan ipbd 8](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/eed3ab09-af93-4112-b710-8a85b53bd556)
  Afterward, I navigated to the scans section. I named my scan 'Test Scan' and set the scan target to the IP address 124.222.31.94, which is from AbuseIPDB for testing purposes. In the module section, I deselected all modules except for AbuseIPDB and then ran the scan.

*Ref 9*
![first scan visual dashboard 9](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/4c1ac8aa-91e5-46ce-a5f6-ff85bf0a6bf2)
  This screenshot displays the included data types, which primarily consist of IP addresses with minimal correlations.

*Ref 10*
![scan 2 investigate 10](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/74432157-0865-464c-86de-5460bdccaf1f)
  After completing the initial scan, I proceeded to start a second scan. Using the 'Investigate' use case, I named this scan 'Test Scan 2' and configured it with the same IP address, 124.222.31.94, obtained from AbuseIPDB for testing purposes. I then initiated the scan to gather additional data and insights.
  
*Ref 11*
![scan 2 visual](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/e0bbe072-f2d3-4dd3-ae8c-afd76134985c)
  This screenshot provides an overview of the various data types associated with the analysis, including IP addresses, domain names, and related metadata.
*Ref 12*
![scan 2 open port 11](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/4a2f3cfe-c47a-4751-993e-6f8173cd50ae)
  After completing the initial scan, I proceeded to explore the correlations section. There, I found a correlation titled 'Software version revealed on open port SSH'. Upon examining this correlation, I inferred that the IP address in question had port 22 open, based on the information provided.

*Ref 13*
![browse second scan 12](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/e4acb1d4-8529-4de1-85f2-4e08ed578ed4)
  After exploring the correlations, I proceeded to the Browse section. In this section, I found detailed information such as country names associated with the IP addresses, BGP (Border Gateway Protocol) data, and email addresses. Additionally, the section provided insights into blacklisted IPs and listed open ports, offering a comprehensive view of the analyzed data.

*Ref 14*
![ip visual map second scan 13](https://github.com/Casttllee/Spiderfoot-OSINT-/assets/137667912/0057ab1b-b8c9-488f-9997-a7fe4aca91de)
  The final step I took was to investigate the IP address graph. This graph visually represents all entities related to the IP address (denoted by a red dot). Notably, one data point shows an email address connected to three other data points, as well as connections to two different IP network ranges.
  
## Conclusion
  In conclusion, this project involved a comprehensive analysis using Spiderfoot on an IP address obtained from AbuseIPDB. Through multiple scans and investigations, I gained insights into various data types including IP addresses, domain names, and associated metadata. The correlations section highlighted significant findings such as open ports and software versions, providing insights into potential vulnerabilities. The Browse section further enriched the analysis with details on country names, BGP data, email addresses, and blacklisted IPs. Finally, the IP address graph visually depicted the intricate relationships among entities, underscoring the interconnected nature of digital footprints. Overall, this project demonstrated the effectiveness of Spiderfoot in conducting thorough reconnaissance and gathering actionable intelligence for cybersecurity and investigative purposes.
