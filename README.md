# Detecting and Predicting countermeasures against Clickjacking

A Clickjacking attack involves creating a malicious web page to deceive the user into making unwanted clicks that benefit the attacker. It spreads malware, steals passwords and cookies, transmits spam, and deletes personal emails, among other things. Clickjacking attacks occur when many programmes or websites share a graphical display: A principal can trick the user into interacting with user interface elements owned by another principal, initiating actions that the user did not expect.

This approach prevents websites from being Clickjacked by detecting the vulnerabilities present in the target website and then returning feedback to the host that includes the measures that could be taken to prevent their websites from being Clickjacked, a numeric value ’Level of Security’ to analyze the relative stability of the website and the possible changes that could be made to increase the ’Level of Security’ of their website.

## Deployment

The model relies on a python script that could run in the command prompt of the computer. A text file has to be created for the task of testing the various websites for any possibility of a Clickjacking attack. The text file contains the name of all the websites that need to be scanned for the Clickjacking attack. The python script scans the text file and presents the expected results in the Terminal window. The task of the script here is to scan the HTML/CSS codes of the websites mentioned in the text file and search for the vulnerabilities in the code that could result in the website being attacked.

## Implementation

The script scans for the presence of the following elements in the code of the websites being scanned for a Clickjacking attack: **XFrame-Options**, **Content-Security-Policy** and **Samesite cookie attribute**. On the basis of the elements mentioned above, the script comments on the security level of the website’s code to protect itself against Clickjacking attacks.

X-Frame-Options are a set of options that may be used to customise the framing options of a webpage. A browser’s ability to render a page in a frame, iframe, or object tag is determined by the HTTP header. It was created with the express purpose of preventing Clickjacking. For the X-Frame-Options, there are three possible options:

![image](https://user-images.githubusercontent.com/75626387/198178548-463380bc-54c5-47d2-a12a-d2b41169a169.png)

The Content-Security-Policy is a set of guidelines that govern the framing settings of a website. The Content-Security-Policy, part of the HTML5 standard, offers more safety than the X-Frame-Options header (which it replaces). It’s set up so that website owners may whitelist specific domains from which resources (such as scripts, stylesheets, and fonts) can be loaded and domains from which they can embed a page.
Likewise, for the Content-Security-Policy, there are three possible options:

![image](https://user-images.githubusercontent.com/75626387/198178767-cbccb6a1-9b7c-483d-a7cf-b72f1ab448d6.png)

The third element under consideration, Samesite cookie attribute. A cookie with this property is only transmitted to a website if it is opened directly, rather than in a frame or in any other way. If a site, like Instagram, has the samesite property on its authentication cookie, it would look like this: ‘Set-Cookie: authorization=secret; samesite’

## Authors

- Aryaman : [@Aryaman-Arya](https://github.com/Aryaman-Arya)
