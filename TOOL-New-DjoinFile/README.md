[NewDjoinFile01]: https://github.com/lazywinadmin/PowerShell/blob/master/TOOL-New-DjoinFile/media/New-DjoinFile01.png
New-DjoinFile
===================
## Related Article(s)
[Blog article on lazywinadmin.com](http://www.lazywinadmin.com/2016/07/offline-domain-join-recreating-blob.html)

## Description

The New-DjoinFile function create a Blob file from the String Generated by Djoin.
This blob file can then be passed to djoin to join the machine to the Active Directory domain.

## Usage

```PowerShell
# Load the function (Dot Sourcing)
. C:\MyScripts\New-DjoinFile.ps1

# Blob generated 
$Blob = "<Blob generated previously on the domain machine>"

# Recreate djoin file
New-DjoinFile -Blob $blob -DestinationFile $home\desktop\blob.txt -Verbose
```

![alt text][NewDjoinFile01]
