# Phishers abusing free javascript hosting
Last year I analysed a [phishing email](https://dfworks.xyz/blog/credential_stealer/) that rendered a semi-convincing, html credential stealer locally rather than directing the victim to a site on the internet. Whilst this wasn't a new tactic, in order to avoid being flagged as malware, obfuscated requests to https://www.yourjavascript.com were made to retrieve additional data such as logo images and screenshots.

yourjavascript.com is a free hosting site that relies on donations to continue functioning so probably can't be held accountable for what users host on the site nor have the resource to audit obfuscated code that has been uploaded. That being said, I was curious as to what other ways this free hosting site was being abused by malicious actors.

The [jupyter notebook]() in this repository contains the code required to replicate the following steps (please clone/branch as you wish and amend the steps for your own research):

- Collate all the URLs for uploaded code on yourjavascript.com

- Triage the collected URLs for signs of obfuscation/malicious activity

- Render any potentially malicious html as an image

- Check malicious html for further malicious URLs

- Check for yourjavascript usernames
