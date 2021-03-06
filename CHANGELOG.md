﻿2017-05-15  Version 2.1.2
  Fix 
   In the manifest the key 'VariableToExport' need Export-ModuleMember -Variable * -Function * -Alias *

2017-05-15  Version 2.1.1
  Fix 
    Start-Log4Net: XmlConfigurator use [Environment]::CurrentDirectory not the Powershell location
   
  Add
    Function New-Log4NetCoreLevel : Create a personalized level.
    Comment about the ETS members
    French tutoriel about Log4net with Powershell
         
  Change
    Throw to $PSCmdlet.ThrowTerminatingError.
    
2017-05-14  Version 2.1.0
  Fix 
    PSSA rules
    Creating indirectly the default repository 
    
  Add
    Support for .NET Core 1.0
    Build tasks
    Translation
    Log4net licence 
     
  Change
    Start-Log4Net : Add Test-Path for the xml configuration file.
    Pester tests
    Throw to $PSCmdlet.ThrowTerminatingError.
    Remove Export-ModuleMember use instead the manifest
    Export functions 'Set-LogDebugging' and 'Get-LogDebugging'
    Use Log4Net version 2.0.8.0
    Core : Now we must create the default repository 'log4net-default-repository'
    Use Publish-Module instead PSNuspec

2017-05-13  Version 2.0.1
  Change
      Reorganization of the repository for the build

2017-02-11  Version 2.0.1
  Fix: 
     function Initialize-Log4NetModule : the call of New-item must use the -PATH parameter.

2016-09-24  Version 2.0.0
  Fix: 
     the initialization of the code injection
     build script
     the the log file name into demo files.

  Add:
     functions Set-LogDebugging and Get-LogDebugging
     Nuspec4 file
     icon for nuget package
     Changelog.md et releasesnotes.md file

  Change:
     Start-Log4Net now fire Error instead Warning (prevent silent failure of log4net)
     the assembly directories (On Github only)
     Pds1 key 'FunctionsToExport'

  Remove :
     Commented code (PSObjectRenderer)
     Alias 'swtafn' 
     

2016-08-06  Version 1.2.0.0
   Refactoring : loading dll by the dotnet version ($psversiontable.CLRVersion) 

2014-03-27  Version 1.1.0.0
   Add PSDebug method, refactoring : use a Log4net repository for each module

2014-03-01  Version 1.0.0.0
    Original version
