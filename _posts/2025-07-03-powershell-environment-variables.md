# This is just for me because I keep forgetting how to set environment variables in powershell - but it's actually quite simple

## Non-persistent Option
```powershell
$env:MyVariable = "Hello, World!"
Write-Host $MyVariable
```

## Persistent Option
This has to be done per user as scope (I guess otherwise you need admin rights)
```powershell
[System.Environment]::SetEnvironmentVariable("MyUserVariableName", "MyUserVariableValue", "User")
Write-Host $MyUserVariableName
```
