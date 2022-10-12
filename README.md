# WindowsHardening

# Disclaimer
Test, test, test before you go into production.  Don't just apply these security settings without testing in a lab environment.  If you use these to secure your home computer, make sure you have a backup.  The free version of Macrium is an excellent choice for backing up your computer.  Remember kids, always know how to undo whatever you do or at least understand the point of no return.

The only testing I've done for you is apply them to my Windows 10 home PCs and run about a year.  Tested on a few VMs here and there.  

# Overview
These Policy Files were created from DISA group policies published at https://public.cyber.mil/stigs/gpo/
If you do not plan to tailor the policies, it would probably be easier to download those policies from DISA and import them using the instructions found there.

The files were created using the GPO2PolicyRules tool released by Microsoft.  This tool is part of the Security Compliance Toolkit.  Learn more here: https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-security-configuration-framework/security-compliance-toolkit-10

Download the Security Compliance Toolkit here: https://www.microsoft.com/en-us/download/details.aspx?id=26ecf5c5-69a3-47d4-877e-49f7706ef092

These policy files are useful as a fairly easy to read, portable, editable way to harden the Windows Operating System and some of the more popular applications.  They are much less cumbersome than dealing with the GPO backups.

The policy files are imported using the lgpo tool released by Microsoft.  This tool is also part of the Security Compliance Toolkit. Download it here: https://www.microsoft.com/en-us/download/details.aspx?id=26ecf5c5-69a3-47d4-877e-49f7706ef092

# Usage
Example of importing settings from a Policy Analyzer .PolicyRules file:

lgpo /p C:\path\sample.PolicyRules  

# License
MIT License

Copyright (c) 2022 CyberSubversive

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
