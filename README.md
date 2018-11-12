# hello_powershell

### Description
Script that prints "hello"

### List of files in the repository and their purpose
- `hello.ps1` - Scrip that prints 'hello'.
- `test.sh` - Script that calls hello.ps1 and checks if the test pass or fails. 
- `.travis.yml` - Script for continous integration
- `Vagrantfile` - Configuration file for creating test environment to test the script.

### How to use this repository.
#### In this example I will use Ubuntu test enviroment if you don't have Windows enviroment to test the script.
* Clone the repository to your local computer: `git clone git@github.com:nikcbg/hello_powershell.git`.
* Go to the cloned repo in your computer: `cd hello_poweshell`.
* Create your test Ubuntu machine by typing: `vagrant up` .
* Login to the newlly created Ubuntu box by typing: `vagrant ssh`.
* You need to download and isntall `powershell` on the Ubuntu box in case to test the script. 
* Run the following lines of code on your Ubuntu test machine:
  * `wget -q -P /tmp https://packages.microsoft.com/config/ubuntu/16.04/packages-microsoft-prod.deb`
  * `sudo dpkg -i /tmp/packages-microsoft-prod.deb`
  * `sudo apt-get update`
  * `sudo apt-get install -y powershell`
* Once you install `powershell` on the Ubuntu box you can test the `powershell`script.
* Execute `bash test.sh` command to see if the `test.sh` script passes or fails.
* When you done testing you can exit the test Uuntu box by typing `exit` command. 
* If you no longer need the Ubuntu box you can delete it by typig `vagrant destroy` command.
