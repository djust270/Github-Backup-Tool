# Github-Backup-Tool

Introducing the github backup tool. A simple tool to backup all of the Github repositories of a specified Github user. 

![Alt text](GithubBackup.gif?raw=true "GithubBackup.exe")

## Features
Clone all of the Github repostories. Just specify a folder location to clone to and a Github username. Optionally, zip all repos with (username)-(todays date) 
for simple archiving. 

## Prerequisites 
Requires git to be installed
Works on Windows, MacOS and Linux

## Usage
Download and run script or grab the precompiled executable from releases. 

Open your terminal emulator of choice, run GithubBackupTool.exe -s (full folder path save location) -u (Github UserName) 
### Optional flags
**-a** will zip all repos into a single archive at the root of the save location with the name *GitHubUsername-TodaysDate.zip

**-f** will force operation and empty the target folder if it already exists (*save location/Github Username)

### Examples

GithubBackupTool.exe -s C:\users\Dave -u djust270 
* This will clone all github repos from user *djust270* and save to *C:\users\Dave\djust270*

GithubBackupTool.exe -s C:\users\Dave -u djust270 -a
* This will clone and zip all github repos from user *djust270* and save to the *C:\users\Dave\djust270-(Month-Day-Year).zip*
