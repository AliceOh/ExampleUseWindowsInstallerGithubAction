# ExampleUseWindowsInstallerGithubAction
 example to show how to use Windows Installer Github Action

## Example usage

1. Create a folder of `application`. Put your exe file, eg, helloworld.exe, and other dependent files if there are, under folder `application`.
2. Create a file of wix.json. You may refer to this example repo's wix.json and replace "helloworld.exe" with your exe name.
3. Add the following in your .github/workflows/yourmain.yaml
```
    - name: Build Windows Installer MSI from exe file
      uses: AliceOh/CreateWindowsInstaller@1.0.0
      with:
        exefile: 'helloworld.exe'
```
You may refer to this example repo's .github/workflows/WinInstaller.yml file.

