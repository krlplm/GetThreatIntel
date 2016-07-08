# GetThreatIntel
Can be used to gather ThreatIntel information about URL, IPs and MD5s

**Description:**
This tool can be used to passively gather the IP, URL and Hash information just from command line which in turn pulls information from the known sources which would help the Security Analysts to reduce the time that they spend on collecting data.

**Deployment:**
1.	Copy “dist.7z” under some folder location say, which we would refer as FOLDER
2. Extract “dist.7z” under FOLDER which would create a folder structure.
3. Traverse to “FOLDER\dist\GetThreatIntel\” where you would find a group of files and an EXE named as “GetThreatIntel.exe”
4. These files are pretty important for various functions of the tool which shouldn’t be removed.

**Usage:**
1. Open CMD (command prompt)
2. Traverse to the FOLDER\dist\GetThreatIntel location by,
   cd FOLDER\dist\GetThreatIntel
3. Run the tool as below,
   GetThreatIntel.exe <options> <target>
   Options 	-	There are a list of options which can be used
   Target 		-	Can be an IP, Domain, Hash
   Eg : GetThreatIntel.exe  --proxy pr-test-dist.net:3128 google.com 
   Note : There are spaces in between each of the arguments above
4. Once the above command is run, you will see the results in the CMD.
5. There are various switches that can be used to have the output in CSV, CEF and html output formats which we will discuss below.

**Getting Help:**
1. Run the command with “–h” switch to see the help.
2. GetThreatIntel.exe -h
 
**Input:**
1. This tool shall accept a list or group of IPs, Domains and Hashes in a text file separated by new line as Inputs apart from standalone target.
2. Pass the complete file path including the filename as “target”
3. Eg: GetThreatIntel.exe ThreatIntel\list.txt
 
**Output:**
1. As discussed above, there are various output options possible through the usage of different switches.
 * GetThreatIntel.exe  -f  output.CEF 	- 	Outputs to a CEF file
 * GetThreatIntel.exe  -w  output.html 	- 	Outputs to a HTML file
 * GetThreatIntel.exe  -c  output.csv	-	Outputs to a CSV file
 
**Queries:**
* Reach out to me for any queries on the usage or if you have any ideas to further improve this tool.
