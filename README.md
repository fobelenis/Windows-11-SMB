# Windows-11-SMB

How to remove SMBv1 via PowerShell

Here are the steps to detect, disable and enable SMBv1 client and server by using PowerShell commands with elevation.

Note

The computer will restart after you run the PowerShell commands to disable or enable SMBv1.

    Detect:
    PowerShell 

Get-WindowsOptionalFeature -Online -FeatureName SMB1Protocol

Disable:
PowerShell

Disable-WindowsOptionalFeature -Online -FeatureName SMB1Protocol

Enable:
PowerShell

Enable-WindowsOptionalFeature -Online -FeatureName SMB1Protocol
