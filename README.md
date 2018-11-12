# hello_powershell

### Explanantion
Script that prints "hello"

### List of files in the repository and their purpose
1. hello.ps1 - Scrip that prints 'hello'.
2. test.sh - Script that calls hello.ps1 and checks if the test pass or fails. 
3. travis.yml - Script for continous integration

### How to use this repository:
* Login to your account in travis.si.org.
* Under repositories find the repsoitory you want to check in trravis in this case "hello_powershell".
* Click the grey activate button so it becomes green.
* Create a pull request in GitHub so travis CI can test your repository. 
* Check travis if the test passes or fails. 
* If the test passed you are good to go.
* If the test failed check travis error messages and fix the error/s and run the test again.
