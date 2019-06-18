# InstantDreams-rwo

The Hugo configuration, including themes, for the static site at http://instantdreams.remotewebaccess.com/


## Features

Hugo will use these files to generate a simple landing page.


## Prerequisites

None


## Installation

A simple clone of the repository is all that is required:

* On the [GitHub page for this repository](https://github.com/instantdreams/InstantDreams-rwo) select "Clone or Download" and copy the web URL
* Open your Git Bash of choice and enter the following commands:
	* cd {base location of your scripts folder} (e.g. /d/ServerFolders/Company/Scripts)
	* git clone {repository url} (e.g. https://github.com/instantdreams/InstantDreams-rwo.git)

This will install a copy of the scripts and files in the folder "InstantDreams-rwo" under your script location.


## Configuration

None


## Running

To run the script, open a PowerShell window and use the following commands:
```
Remove-Item -Path "[script location]\public" -Recurse -Force
hugo
Remove-Item -Path "[web page location]\*" -Recurse -Force
Copy-Item -Path "[script location]\public\*" -Destination "[web page location]" -Recurse
```

For example:
```
Remove-Item -Path "D:\Scripts\InstantDreams-rwo\public" -Recurse -Force
hugo
Remove-Item -Path "C:\inetpub\wwwroot\*" -Recurse -Force
Copy-Item -Path "D:\Scripts\InstantDreams-rwo\public\*" -Destination "C:\inetpub\wwwroot" -Recurse
```


## Troubleshooting

This is intended for use on one particular page. Get your own. :)


## Author

* **Dean W. Smith** - *Script Creation* - [instantdreams](https://github.com/instantdreams)


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details


## Security

This project has a security policy - see the [SECURITY.md](SECURITY.md) file for details