# oneclickminer
The tool is designed for dgb-odo mine and auto management on Blackminer F1/F1+/F1-MINI

Procedure:
1. Click oneclickminer.exe
2. Tool will auto get network information and auto scan like 192.168.1.2-254, and find all the miner in local network
3. If user want to config something manuually, click auto stop button to stop auto cycle first
4. during auto cycle, oneclickminer will auto upgrade bitstream when time is up (dgb-odo need upgrade bitstream every 10 days)

How to change password if your miner's password is not root?
User could set passwrod in oneclickminer.exe.config like below:
  <common_web>
    <add key="user" value="root" />
    <add key="pass" value="root" />
  </common_web>
  
How to keep configuration?
Once user change the pool setting (pool url, worker, pwd), oneclickminer will save the information in config.txt file.
Oneclickminer will get url/worker/pwd from config.txt when app launch if config.txt exist

