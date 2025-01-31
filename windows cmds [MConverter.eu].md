# Windows commands {#windows-commands .unnumbered}

## Ipconfig

> **Syntax: ipconfig**
>
> **Function:** cmd to show the NIC ip config and basic details.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/ipconfig)
>
> **Example:** ![](media/image1.png){width="7.5in"
> height="4.3284722222222225in"}

### ipconfig /all

> **Syntax: ipconfig /all**
>
> **Function:** cmd to show the all NIC details.

### ipconfig /flushdns

> **Syntax: ipconfig /flushdns**
>
> **Function:** cmd to clear the DNS cache.

## Ping

### 2.1 Ping: {#ping-1 .unnumbered}

> **Syntax: ping** \<ip address\>
>
> **Function:** cmd to check weather the destination computer is
> reachable or not.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/ping)
>
> **Example:**
>
> ![](media/image2.png){width="7.5in" height="2.4577471566054245in"}

### 2.2 Ping with timestamp: {#ping-with-timestamp .unnumbered}

**Syntax: ping -t** \<ip address\> **\|Foreach{\"{0} - {1}\" -f
(Get-Date),\$\_}**

> **Function:** it will work in PowerShell. Normal ping cmd show the
> reply details of the destination computer but cmd will show the replay
> with timestamp.
>
> **More details:** [Refer
> Spiceworks](https://community.spiceworks.com/how_to/154193-ping-with-timestamp-and-log)
>
> **Example:**
>
> ![](media/image3.png){width="7.5in" height="2.7in"}

## Path ping

> **Syntax: pathping** \<ip address\>
>
> **Function:** cmd to check the packet loss and no of hops between
> source and destination.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/pathping)
>
> **Example:**![](media/image4.png){width="7.5in"
> height="4.959027777777778in"}

## Tracert

> **Syntax: tracert** \<ip address\>
>
> **Function:** cmd to check the hops and no of router between source
> and destination.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/tracert)
>
> **Example:**
>
> ![](media/image5.png){width="7.5in" height="2.8965277777777776in"}

## Nslookup

> **Syntax: nslookup** \<domain name\>
>
> **Function:** cmd to resolve the dns name to ip.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/nslookup)
>
> **Example:**
>
> ![](media/image6.png){width="7.5in" height="2.4791666666666665in"}

## Wifi Qrcode generator

> **Syntax: new-qrcodewifiaccess -SSID \"**\<wifi name\>**\" -Password
> \"**\<wifi password\>**\" -outpath \"**\<file path location to save
> file\>**\"**
>
> **Function:** cmd to genetrate wifi qrcode in powershell
>
> **Installation cmds:** Install-Module -Name QRCodeGenerator
>
> Import-Module QRCodeGenerator
>
> **More details:** [Refer Generate QR Code with PowerShell in Windows
> 10](https://winaero.com/generate-qr-code-powershell-windows-10/)
>
> **Example:** ![](media/image7.png){width="7.5in"
> height="6.238194444444445in"}

## Attrib Command

> **Syntax: attrib "**\<folder name\>**" +s +h +r**
>
> **Function:** folder is hidden and isn\'t visible when we select to
> show all files and folders.
>
> **s** System
>
> **h** Hidden
>
> **r** Read-only
>
> **Syntax: attrib "**\<folder name\>**" -s -h -r**
>
> **Function:** folder is visible when we select to show all files and
> folders.
>
> **More details:** [Refer
> www.c-sharpcorner.com](https://www.c-sharpcorner.com/UploadFile/fd0172/how-to-hide-or-unhide-folders-using-attrib-command/)
>
> **Example:** ![](media/image8.png){width="7.5in"
> height="2.7423611111111112in"}

## Title

> **Syntax: title** \<string\>
>
> **Function:** To change the Command Prompt title.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/title)
>
> **Example:**
>
> ![](media/image9.png){width="7.5in" height="1.2361111111111112in"}

## Prompt

> **Syntax: prompt** \<text\>
>
> **Function:** To change executing path name in command prompt.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/prompt)
>
> **Example:** ![](media/image10.png){width="7.5in"
> height="1.6402777777777777in"}

## Netsh \#wifi password

> **Syntax: netsh wlan show profile**
>
> **Function:** To show a list of network names that we already connect
> to.
>
> **Syntax: netsh wlan show profile name= "**\<Wi-Fi name\>"
> **key=clear**
>
> **Function:** To show the password of the given wi-fi name
>
> **More details:** [Refer Microsoft
> Learn](https://www.geeksforgeeks.org/how-to-find-the-wi-fi-password-using-cmd-in-windows/)
>
> **Example:** ![](media/image11.png){width="7.5in"
> height="3.3118055555555554in"}
>
> ![](media/image12.png){width="7.5in" height="7.084027777777778in"}
>
> **Syntax: netsh wlan show interface**
>
> **Function:** To show wifi interface details.
>
> **More details:** [Refer Udemy
> video](https://www.udemy.com/course/complete-wifi-hacking-course/learn/lecture/30598776#overview)

**Example:**

![](media/image13.png){width="7.5in" height="3.8506944444444446in"}

> **Syntax: netsh wlan show wlanreport**
>
> **Function:** To create the wireless network report. For execute this
> cmd run the command prompt as administrator mode.
>
> **More details:** [Refer Microsoft
> support](https://support.microsoft.com/en-us/windows/analyze-the-wireless-network-report-76da0daa-1db2-6049-d154-7bb679eb03ed)

**Example:**

![](media/image14.png){width="7.524165573053368in"
height="4.169160104986877in"}

## Manage-bde Bitlocker  {#manage-bde-bitlocker}

### Unlock: {#unlock .unnumbered}

> **Syntax: Manage-bde -unlock** \<drive letter\>**: -password**
>
> **Function:** run command prompt in Admin mode to unlock the bitlocker
> drive.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/manage-bde)
>
> **Example:**
>
> ![](media/image15.png){width="7.5in" height="2.238888888888889in"}
>
> **Here enter the password of Bitlocker dirve.**

### Lock: {#lock .unnumbered}

> **Syntax: Manage-bde -lock** \<drive letter\>**:**
>
> **Function:** run command prompt in Admin mode to lock the bitlocker
> drive. If any application or file is opened in that drive location it
> will not lock.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/manage-bde)
>
> **Example:**
>
> ![](media/image16.png){width="6.942268153980752in"
> height="2.1251837270341207in"}

### Force lock: {#force-lock .unnumbered}

> **Syntax: Manage-bde -lock** \<drive letter\>**: -forcedismount**
>
> **Function:** run command prompt in Admin mode to lock the bitlocker
> drive. If any application or file is opened in that drive location
> then also it will lock the drive.
>
> **More details:** [Refer Microsoft
> Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/manage-bde)
>
> **Example:**
>
> ![](media/image17.png){width="6.808923884514436in"
> height="2.3335356517935257in"}

## Activate Windows watermark temporary remove

> **Syntax: bcdedit -set TESTSIGNING OFF**
>
> **Function:** run command prompt in Admin mode, enter the command and
> reboot the computer. use this command to temporarily hide the Activate
> Windows watermark.
>
> **More details:** [I find in
> YT](https://www.youtube.com/shorts/FAwoU2hVFjs)
>
> **Example:**

**  
**

> [Before]{.mark}
>
> ![7 Methods To Remove "Activate Windows Watermark" --
> RoyalCDKeys](media/image18.png){width="7.5in" height="4.375in"}
>
> [After]{.mark}
>
> ![How to Create a Desktop Shortcut on
> Windows](media/image19.jpeg){width="7.5in"
> height="4.220138888888889in"}

## Display the content of a file in Command Prompt and PowerShell

### Using Command Prompt: {#using-command-prompt .unnumbered}

**Syntax: type "**\[\<drive\>**:**\] \[\<path\>\] \<file
name.extension\>**"**

> **Function:** To view a text file without modifying it and show the
> file content in the CMD prompt. It limit the lines while display file
> content. Use MORE cmd with pipe symbol now now press spacebar to shows
> all the line in the large file.

**More details:** [Refer Microsoft
Learn](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/type)

**Example:**

![](media/image20.png){width="7.5in" height="4.854166666666667in"}

### Using PowerShell: {#using-powershell .unnumbered}

**Syntax: Get -content -Path "**\[\<drive\>**:**\] \[\<path\>\] \<file
name.extension\>**"**

> **Function:** To view a text file without modifying it and show the
> file content in PowerShell Window. It show's the all line of the file
> it doesn\'t limit lines while display. Use MORE command with pipe
> symbol now press spacebar to shows all the line in the large file.

**More details:** [Refer Microsoft
Learn](https://www.windowscentral.com/how-save-command-output-file-using-command-prompt-or-powershell)

**Example:**

> ![](media/image21.png){width="7.5in" height="3.5009722222222224in"}

## Create and Delete files and directories form windows command prompt

### Create empty file: {#create-empty-file .unnumbered}

**Syntax: type nul \> "**\[\<drive\>**:**\] \[\<path\>\]
\<filename\>**"**

**Function:** it create the empty file in using command prompt.

**More details:** [Refer
wikihow](https://www.wikihow.com/Create-and-Delete-Files-and-Directories-from-Windows-Command-Prompt)

**Example:**

![](media/image22.png){width="7.5in" height="3.3756944444444446in"}

### Create a blank file in certain size: {#create-a-blank-file-in-certain-size .unnumbered}

**Syntax:** **fsutil file createnew "**\[\<drive\>**:**\] \[\<path\>\]
\<filename\>**"** \<length\>

**Function:** To create a blank text file based on byte size.

**More details:** [Refer
Wikihow](https://www.wikihow.com/Create-and-Delete-Files-and-Directories-from-Windows-Command-Prompt)

**Example:**

![](media/image23.png){width="7.5in" height="5.768055555555556in"}

## Open files using command prompt

**Syntax: "**\[\<drive\>**:**\] \[\<path\>\] \<filename\>**"**

> **Function:** type the file path in command to open any type of file
> using command prompt with default application which is installed in
> computer.

**More details:** Google Search

**Example:**

![](media/image24.png){width="7.183345363079615in"
height="4.125768810148731in"}

## Command output save to a file using Command Prompt and PowerShell

### Using Command Prompt: {#using-command-prompt-1 .unnumbered}

***[Create new output file:]{.underline}***

**Syntax:** \<your-command\> **\> "**\[\<drive\>**:**\] \[\<path\>\]
\<filename\>**"**

> **Function:** command to save the command output to a text file.
> **\>** is the symbol for create a new text file or over write in
> existing file to save the output.

**More details:** [Refer Windows
Central](https://www.windowscentral.com/how-save-command-output-file-using-command-prompt-or-powershell)

**Example:**

![](media/image25.png){width="7.5in" height="3.7180555555555554in"}

***[Continue output in existing file:]{.underline}***

**Syntax:** \<your-command\> **\>\> "**\[\<drive\>**:**\] \[\<path\>\]
\<filename\>**"**

> **Function: :** command to save the command output to a text file.
> **\>\>** is the symbol for write existing file to save the output.

**More details:** [Refer Windows
Central](https://www.windowscentral.com/how-save-command-output-file-using-command-prompt-or-powershell)

**Example:**

![](media/image26.png){width="7.5in" height="3.6326388888888888in"}

### Using PowerShell: {#using-powershell-1 .unnumbered}

**Syntax: ipconfig \| Out-File -FilePath "**\[\<drive\>**:**\]
\[\<path\>\] \<filename\>**"**

**Function:** To save the command output to a text file with PowerShell.
It will over write the existing file.

**More details:** [Refer Windows
Central](https://www.windowscentral.com/how-save-command-output-file-using-command-prompt-or-powershell)

**Example:**

![](media/image27.png){width="7.5in" height="6.490972222222222in"}
