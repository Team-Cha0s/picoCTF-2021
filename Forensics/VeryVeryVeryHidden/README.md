

So this one was actually quite easy I first opened the Wireshark file in network miner and through there I went to the files to saw what was being transferred and managed to see two images, that I found quite interesting so I tried almost all the basic image forensics on both of those images but I had no luck so I started looking in the DNS and found a couple DNS queries about PowerShell and that led me to believe there has to be some sort of PowerShell script that I need to get cause all the other links were dead ends. So I came across this tool right here on GitHub https://github.com/imurasheen/Extract-PSImage which basically extracts a hidden PowerShell script within an image and I used this to do just that by running the two simple commands below:

> PS> Import-Module .\Extract-Invoke-PSImage.ps1
> PS> Extract-Invoke-PSImage -Image [path to the PNG image] -Out [path to the .ps1 file]

After that I analyzed the PowerShell file and I believed that the flag would come out after I ran the script I believed this because of the first variable in the script which indicates that it will put out a flag.txt file. So I deleted all the scrap and kept only the relevant 13 lines which are needed to run the script, and so I ran the script which gave me the flag in flag.txt

> picoCTF{n1c3_job_f1nd1ng_th3_s3cr3t_in_the_im@g3}
