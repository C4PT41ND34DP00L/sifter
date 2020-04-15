# NB
	* Please be aware there will be some issues with internal tools as python2 is phasing out.
	* While these tools are replaced or ported to python3 please just keep this in mind.
	* But I am constantly working to ensure all tools work correctly.
	* If local install causes too many errors please use the docker image.

<p align="center">
	<img align="center" src="https://raw.githubusercontent.com/s1l3nt78/sifter/master/docs/sifter.PNG">
<br>
  	<img align="center" src="https://img.shields.io/github/issues/s1l3nt78/sifter">
  	<img align="center" src="https://img.shields.io/github/forks/s1l3nt78/sifter">
  	<img align="center" src="https://img.shields.io/github/stars/s1l3nt78/sifter">		  
<br>
  	<img align="center" src="https://img.shields.io/badge/Version-6-red">
	<img align="center" src="https://img.shields.io/badge/Build-RubY-blue">
<br>
	 <img align="center" src="https://img.shields.io/badge/Author-s1l3nt78-yellowgreen">
</p>

# Sifter
<strong><em>s1l3nt78</em></strong>
<br>
* *Because the first step, is enumeration*
<br>
<br>
Sifter is a osint, recon & vulnerability scanner. It combines a plethara of tools within different module sets in order to quickly perform recon tasks, check network firewalling, enumerate remote and local hosts, and scan for the 'blue' vulnerabilities within microsft and if unpatched, exploit them.  It uses tools like blackwidow and konan for webdir enumeration and attack surface mapping rapidly using ASM.
<br>
Gathered info is saved to the results folder, these output files can be easily parsed over to <a href="https://github.com/s1l3nt78/TigerShark">TigerShark</a> in order to be utilised within your campaign. Or compiled for a final report to wrap up a penetration test.

# Coming soon in Version 6

	* Phasing out tools that use python2 and
 	* replacing them with suitable python3 tools


<a href="https://www.youtube.com/watch?v=YU-LYLjyO6c&t=8s">Setup Video</a>
<br>
<a href="https://youtu.be/QgAfqbxqbK0">Demo Video</a>
<br>
Its long, but you can skip through to get the general idea. Most modules are explained along with demos of a lot of the tools
<br>
<br>
NOTE!! IF A SCAN DOESN'T WORK PLEASE ENTER TARGET WITHOUT http:// protocol ADDED!!
<br>
<br>
eg. target.com
<br>
instead of http://target.com
<br>
<br>
# Please, if you fork this repo ensure to keep it updated.
<br>
<br>

# Installation

	* This will download and install all required tools
	*
	$ git clone https://github.com/s1l3nt78/sifter.git
	$ cd sifter
	$ chmod +x install.sh
	$ ./install.sh


	* For tool install issues please run extras/FRESH-INSTALL.sh
	* to completely remove and reinstall the tools
	*
	*
	* Sifter is also available on docker.
	* Please run extras/docker-install.sh. This will pull the newest sifter
	* container with all tools fully installed and working. This will also
	* move extras/sifter to your env-path.
	* This script will automatically start the container and attach you directly into the program.
	* No extra commands necessary.
	* The docker script also exports results directly to Desktop for easy review of files.

	* Alternatively you can copy and paste the following command to install SifteR on docker without
	* cloning the whole directory
	$ wget https://raw.githubusercontent.com/s1l3nt78/sifter/master/extras/docker-install.sh && wget https://raw.githubusercontent.com/s1l3nt78/sifter/master/extras/sifter && chmod +x docker-install.sh sifter && ./docker-install.sh && rm docker-install.sh




<h2>Menu</h2>
	<p align="center">
		<img align="center" src="https://raw.githubusercontent.com/s1l3nt78/sifter/master/docs/menu.PNG">
	</p>
<br />
<br>

# Modules:
	# Information Modules
	  = Enterprise Information Gatherers
		  -theHarvester  - https://github.com/laramies/theHarvester
		  -Osmedeus - https://github.com/j3ssie/Osmedeus
		  -ReconSpider - https://github.com/bhavsec/reconspider
		  -Maryam - https://github.com/saeeddhqan/Maryam

	 = Targeted Information Gatherers
		  -Seeker - https://github.com/thewhiteh4t/seeker
		  -Sherlock - https://github.com/sherlock-project/sherlock
		  -xRay - https://github.com/evilsocket/xray

	# Domain Recon Gathering
		-Omnibus - https://github.com/InQuest/omnibus
		-DnsTwist - https://github.com/elceef/dnstwist
		-DomainFuzz - https://github.com/monkeym4ster/DomainFuzz
		-Armory - https://github.com/depthsecurity/armory


	# Exploitation Tools
	  = MS Exploiters
		  -ActiveReign - https://github.com/m8r0wn/ActiveReign
		  -iSpy - https://github.com/Cyb0r9/ispy
		  -SMBGhost - https://github.com/gabimarti/SMBScanner

	  = Website Exploiters
		  -Dark Star - https://github.com/s1l3nt78/Dark-Star
		  -NekoBot - https://github.com/tegal1337/NekoBotV1
		  -xShock - https://github.com/capture0x/XSHOCK
		  -SayDog - https://github.com/saydog/saydog-framework

	= Exploit Searching
		  -FindSploit - https://github.com/1N3/Findsploit
		  -ShodanSploit - https://github.com/shodansploit/shodansploit

	   -TigerShark (Phishing) - https://github.com/s1l3nt78/TigerShark

	   -WPForce/Yertle - https://github.com/n00py/WPForce

	   =FuzzyDander (Obtained through issue request.)
	   	-FuzzBunch
		-Danderspritz

	   -BruteDUM (Bruteforcer) - https://github.com/GitHackTools/BruteDum

	# Network Scanners
		-Nmap - https://nmap.org
		-AttackSurfaceMapper - https://github.com/superhedgy/AttackSurfaceMapper
		-aSnip - https://github.com/harleo/asnip
		-Arp-Scan

	# HoneyPot Detection Systems
		-HoneyCaught - https://github.com/aswinmguptha/HoneyCaught
		-SniffingBear - https://github.com/MrSuicideParrot/SniffingBear


	# Vulnerability Scanners
		-Flan - https://github.com/cloudflare/flan
	  	-Rapidscan - https://github.com/skavngr/rapidscan
		-Yuki-Chan - https://github.com/Yukinoshita47/Yuki-Chan-The-Auto-Pentest


	# WebApplication Scanners
		  -Sitadel - https://github.com/shenril/Sitadel
		  -wafw00f - https://github.com/EnableSecurity/wafw00f
		  -AapFinder - https://github.com/Technowlogy-Pushpender/aapfinder
		  -BFAC - https://github.com/mazen160/bfac


	# Website Scanners & Enumerators
		  -Nikto - https://github.com/sullo/nikto
		  -Blackwidow - https://github.com/1N3/blackwidow
		  -WPScan - https://github.com/wpscanteam/wpscan
		  -Konan - https://github.com/m4ll0k/Konan
		  -Dirb

# Sifter Help Menu

  $ sifter	runs the programs bringing up the menu in a cli environment
  <br>
  $ sifter	-c will check the existing hosts in the hostlist
  <br>
  $ sifter	-a 'target-ip' appends the hostname/IP to host file
  <br>
  $ sifter 	-m Opens the Main Module menu
  <br>
  $ sifter	-e Opens the Exploitation Modules
  <br>
  $ sifter	-i Opens the Info-based Module menu
  <br>
  $ sifter 	-d Opens the Domain Focused Modules
  <br>
  $ sifter 	-n Opens the Network Mapping Modules menu
  <br>
  $ sifter	-w Opens the Website Focused Modules
  <br>
  $ sifter	-wa Opens the Web-App Focused Module menu
  <br>
  $ sifter	-v Opens the Vulnerability Scanning Module Menu
  <br>
  $ sifter	-r Opens the results folder for easy viewing of all saved results
  <br>
  $ sifter	-u Checks for/and installs updates
  <br>
  $ sifter	-h This Help Menu


Any suggestions for extra modules are welcome.
Just submit an issue with your tool suggestion
Otherwise for developers just submit a pull request.
