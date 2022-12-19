# Building and deploying VirtualKeyboardControl Nuget package

## Prerequisite

[Get nuget.exe and put it in your path](https://www.nuget.org/downloads)

## Steps

1. Change the version number of the the `wpfKeyBoard` project

2. From the Visual Studio Solution Explorer, right click on the `wpfKeyBoard` project and run **Pack**
 
3. Open Powershell terminal in the base solution directory and then navigate down to `\bin\Release`.

4. Execute `nuget pack .\ClearBible.Engine.nuspec`

5. Execute `  nuget push .\wpfKeyBoard-clear.1.0.0.nupkg -ApiKey <YOUR KEY> -Source https://nuget.pkg.github.com/clear-bible/index.json`