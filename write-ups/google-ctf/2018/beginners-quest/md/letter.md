# Beginners Quest: Letter 
### Garbo-can

[]()</p><table align="right"><thead><th colspan="2"><h3 align="center">
Properties </h3></th></thead><tbody><p><tr><td><p>
**Author** </p></td><td><p>
[Google](:ctf:archive:filter=author#google) </p></td></tr><tr><td><p>
**Tags** </p></td><td><p>
[misc](:ctf:archive:filter=tags#misc) </p></td></tr><tr><td><p>
**Year** </p></td><td><p>
[2018](:ctf:archive:filter=year#2018) </p></td></tr><tr><td><p>
**Difficulty** </p></td><td><p>
Easy </p></td></tr><tr><td><p>
**Attachment** </p></td><td><p>
[Download](https://storage.googleapis.com/gctf-2018-attachments/5a0fad5699f75dee39434cc26587411b948e0574a545ef4157e5bf4700e9d62a) </p></td></tr><tr><td><p>
**Point Value** </p></td><td><p>
Null </p></td></tr>
</tbody></table>

## Description
You really went dumpster diving? Amazing. After many hours, SUCCESS! Between what looks like a three week old casserole and a copy of "Relative-Time Magazine", you found this important looking letter about the victims PC. However the credentials aren't readable - can you still obtain them?

[]()</p><table align="left"><thead><th><h3 align="center">
Table of Contents </h3></th></thead><tbody><p><tr><td><ul><li>
[Description](#description) </li><li>
[Write-Up](#write-up) </li><ul><li>
[Download](#download) </li><li>
[New Directory](#new-directory) </li><li>
[Unzip](#unzip) </li><li>
[Open .pdf](#open-pdf) </li><li>
[Grab Credentials](#grab-credentials) </li><li>
[Victory](#victory) </li><li>
[Tips](#tips) </li></ul><li>
[Solution](#solution) </li><ul><li>
[Flag](#flag) </li></ul><li>
[Notes](#notes) </li><li>
[References](#references) </li><li>
[External Links](#external-links) </li></ul></td></tr>
</tbody></table>

## Write-Up

> __Click [HERE](#solution) for bare-bones solution with no explanations.__

#### Download
In the challenge description it says we'll be dealing with a document with text that has been obscured in some way. Lets download the file attached to the challenge.

#### New Directory
Upon downloading we see that it is a .zip file. First things first lets put the file in a new directory so that we can keep track of what comes out of it.

#### Unzip
Next lets unzip the file. You can do this by running: ``` unzip "file".zip ``` or by running ``` unzip *.zip ``` while in the directory the file is in. **Be careful though running ``` unzip *.zip ``` will unzip all files in the directory the command is run in.** If you don't have unzip installed you can install by running ``` sudo apt-get install unzip ```.

#### Open .pdf
Now that we have unzipped the file we have downloaded we see that there was a .pdf document inside. Go ahead and open the file with whatever default deals with .pdf files on your computer. If you don't have a program for .pdf files web browsers like Google Chrome<sup>[1](#references)</sup> or Firefox<sup>[2](#references)</sup> can open the file.

#### Grab Credentials
On looking at the pdf we see what the challenge description mentioned. The two fields "Username" and "Password" are unreadable because they have been blacked out.
Go ahead and select and copy the fields and paste them into your favorite text editor (pasting them into the browsers search bar works as well). After pasting the fields we see that we have the text the was obscured. This works because the pdf document only visually blocks the text but doesn't remove it, so we still can select it.

#### Victory
Looking at the pasted text we see that the "Username" field had no useful information, but the "Password" field has exactly what we are looking for. Now go submit the flag and claim your first victory!

> __Click [HERE](#solution) for bare-bones solution with no explanations.__

### Tips
- Create a new directory for your CTF files to keep them organized.
- When submitting a don't forget to send THIS{___} with it.

## Solution
1. Download Attachment
2. Unzip .zip file ``` unzip "file".zip ```
3. Open "challenge.pdf"
4. Copy blacked-out flag text in "Password" field
5. Submit flag
### Flag
<details><summary>Spoiler!</summary>

```CTF{ICanReadDis}```
</details>

## Notes
- This is the first challenge of [Google CTF 2018](:ctf:2018:google-ctf)<sup>[3](#references)</sup> [Beginners Quest](:ctf:2018:google-ctf:beginner-ctf)<sup>[4](#references)</sup>
## References
1. <sup>[^](#open-pdf)</sup> ["Google Chrome Web Browser"](https://www.google.com/chrome/). *google.com*. Google, Inc. 2019.
2. <sup>[^](#open-pdf)</sup> ["Firefox"](https://www.mozilla.org/en-US/firefox/new/). *mozilla.org*. Mozilla Foundation. 2019.
3. <sup>[^](#notes)</sup> ["Google CTF"](https://capturetheflag.withgoogle.com/). Google, Inc. 2018.
4. <sup>[^](#notes)</sup> ["Google CTF Beginners Quest"](https://capturetheflag.withgoogle.com/#beginners/). Google, Inc. 2018.

## External Links
- [Google CTF](https://capturetheflag.withgoogle.com/)
- [Google CTF Beginner Quest: Letter](https://capturetheflag.withgoogle.com/#beginners/misc-letter)
- [About Google](https://www.google.com/intl/en/about/)