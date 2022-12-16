# Export controls

The topic of export cotrols is quiet old. In the mid 90s a group of 16 states introduces the [Wassenaar agreement](!https://www.wassenaar.org), which is a mutual agreement on coordinting the efforts and legistlation on export controls. Meanwhile 42 states joined the club. However, on an annual basis they develop two lists, the **Munition List** and and the list for **Conventional Arms and Dual Use Goods**. For Software development this starts bein interesting when it comes to specifc use, e.g. jamming capabilities (see ML21), image processing (cameras, infrared, radar sensor, etc.) (see ML15) and all sorts of software which is designed to operate or maintain specific primary purpose military goods. 
Relatively important becomes the scope of ML21.b.5, which also includes all sorts of software designed to *...cyber reconnaissance and cyber copmmand and control "software"...*. Thus it may address also simple network managemnet tools.
However, even more of interest is the *List for Dual Use Goods*. Chapter 5 covers software, especially cryptography (see 5.D.Part 1)A exemption is given only, if it can be purchased as a simple retail transaction (online, offline, whatever), does not allow to change encryption and may be used and setup without further support by the supplier. Section 5.A.Part 2 gives a handful of additinal use cases that may free you from the regulations. However, this only will apply for the Wassenaar member states. 
Thus, Dealing with software, even open source, it will be benficial to get an idea of the included encrypton capabilities. If you have an understanding of what is contained, you will gain two benefits:
a) you have a chance to manage the security of your product (just becaus a tool implements encryption does not mean it is secure!) by creating allow/deny lists across your organisation
b) you can trigger pro-actively action when exporting in crypto-sensitive states (e.g. China or Saudi-Arabia)

# Links and Resources

The following websites contain / collect or provide additional information on export control regulations.
- http://www.cryptolaw.org/
one of the most comprehensive free resources, compiled be Bert-Jappe Koops, a researcher during his PHD in the 90s. He stopped maintaining it in 2013. Thus the information may be outdated. But the site also conatins a plethora of contact information and links to regulatory authorities, so that it will at least be an excellent start for every investigation. 



# Tools
Since the topic became relevant in the early 1990s, it is quiet a while since software vendors have to cope witht he challenges. Some of them shared the results of their effforts and provde their tooling. Find here a list of cool tools:

- **Crypto-Detector** by Wind-River
provides an automated and efficient code parser that can determine, with a certain confidence, that a piece of code contains restricted encryption algorithms. The output could then be verified by a human expert.  It supports two assessments: Using keywords and using API indicators. The lists arae available and can be modified/extended. The tool can be used to scan repos, packages and local sources. It is licensed under Apache-2.0.

- **minr** from SCANOSS:
Can be found [here](https://github.com/scanoss/minr) is a Linux-based service, that allos to identify for a huge list of encryption algorithms in source code. It will write the results in a DB accompanied with the tooling to allow later assessment. Minr contains a definition  The tool can be used to scan  Licensed under GPL-2.0

- **ts-deepscan** from [TrustSource](!https://www.trustsource.io)
DeepScan has been designed to assess repositoriestakes the capabilities 

- **Application-Inspector** from Microsoft
Is a Dot-Net based solution and can be found [here](!https://github.com/microsoft/ApplicationInspector), that assesses source code for its capabilities. The results are documented and provided as a report. Application inspector uses regex patterns for it analysis. 

# License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Info-Collection on `export controls`</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/trutssource/exportcontrols" property="cc:attributionName" rel="cc:attributionURL">TrustSource Research</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
