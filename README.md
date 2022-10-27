# Detecting and Predicting countermeasures against Clickjacking

A Clickjacking attack involves creating a malicious web page to deceive the user into making unwanted clicks that benefit the attacker. It spreads malware, steals passwords and cookies, transmits spam, and deletes personal emails, among other things. Clickjacking attacks occur when many programmes or websites share a graphical display: A principal can trick the user into interacting with user interface elements owned by another principal, initiating actions that the user did not expect.

This approach prevents websites from being Clickjacked by detecting the vulnerabilities present in the target website and then returning feedback to the host that includes the measures that could be taken to prevent their websites from being Clickjacked, a numeric value ’Level of Security’ to analyze the relative stability of the website and the possible changes that could be made to increase the ’Level of Security’ of their website.

### Deployment

The model relies on a python script that could run in the command prompt of the computer. A text file has to be created for the task of testing the various websites for any possibility of a Clickjacking attack. The text file contains the name of all the websites that need to be scanned for the Clickjacking attack. The python script scans the text file and presents the expected results in the Terminal window. The task of the script here is to scan the HTML/CSS codes of the websites mentioned in the text file and search for the vulnerabilities in the code that could result in the website being attacked.
