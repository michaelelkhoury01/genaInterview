# LinkedIn Phishing Page

## Phishing Page Preview
First and foremost, the link to the phishing page is the following: https://genatecinterview.firebaseapp.com/

Below is a screenshot of the phishing link that can be reached via the hyperlink provided above.
![Page Screenshot](screenshots/pageScreenshot.png?raw=true)

## Email Preview
I have included the email text and subject in the email.txt file: ![Email text file](email.txt)

Below is a screenshot of the email presumably sent by the CEO:
![Email Screenshot](screenshots/phishingScreenshot.png?raw=true)

## Stealing the Footer from Genatec Employees
In order to get the HTML footer from the employee emails', I used 'Inspect element', and then copied the outer HTML of the table containing the footer of the email, as follows: 
![Copying footer](screenshots/footerCopy.png?raw=true)

I then pasted the HTML table to a text editor, in which I changed links so that they would be accessible via an image hosting website. Note that I also changed both the link pointing to the page, as well as the social media logo in the footer, to the fake phishing LinkedIn address.
![Footer code](screenshots/footerCode.png?raw=true)

## Web Hosting
I used Google Firebase Web Hosting service via command line on Linux, by using npm tool and then installing the Firebase CLI.
After having installed it, I made a folder on my local machine, which would be root on the Firebase app, pointing by default to the index.html page which would be the phishing LinkedIn site.

## Final Notes
I hope that I have covered all the steps I have taken. It is also worth mentioning that I have tried spoofing email addresses in order to trick the receiver into thinking that the email is coming from a legitimate sender address from the company. However, nowadays, Google, Microsoft, and other email services can now verify the sender's authenticity, since SMTP does not offer authentication, by using fully qualified domain addresses (FQDA) which primarily serves as certificate that the company is legit and registered.
