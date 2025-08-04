###ADUSER
To find account in AD that uses ReversibleEncryption
```ps1
Get-ADUser -Filter 'AllowReversibleEncryption -eq $true' -properties AllowReversibleEncryption
```
Finding accounts where Password never expires neatly
```ps1
Get-ADUser -filter {PasswordNeverExpires -eq $true} -properties PasswordNeverExpires | Select-Object Name, SamAccountName, PasswordNeverExpires
```
Finding account Descriptions
```ps1
Get-ADUser -filter * -Properties Description | Select-Object Name, Description
```
View all files on something like a share for ex
```ps1
Get-ChildItem -Recurse -File -Force
```
Finding RID of a user
```ps1
Get-ADUser -Identity 'krbtgt' -Properties Description
```
Finding based on a phone number
```ps1
Get-ADUser -filter * -properties TelephoneNumber | where Telephonenumber -match "336-6754"
```
SCP from a share 
```ps1
scp 'Full\File\Path' andy.dwyer@10.10.0.2:C:\
```
Then RDP into YOUR ADMIN IP, and look for the file

Finding a user with only part of their name
```ps1
Get-ADUser -Filter "samaccountname -like 'Tiffany*'"
```
