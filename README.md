1) Build "src\ClassLibrary1\ClassLibrary1.sln" in Debug mode
2) Open a command promp in "scripts"
3) Run "scriptcs run.csx -loglevel debug"
4) See that it outputs "Nothing" as string (as expected)
5) Run "scriptcs run.csx -loglevel debug -debug" (or alternative use :openvs "run.csx" and start debug from there)

```
ERROR: [ScriptCs.Engine.Roslyn.CSharpScriptCompilerEngine] An error occurred when executing the scripts.
ERROR: [ScriptCs.ExecuteScriptCommandBase] Script execution failed. [System.IO.FileNotFoundException] Could not load file or assembly 'ClassLibrary1, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null' or one of its dependencies. The system cannot find the file specified.
   at Submission#0..ctor(Object[] submissionArray, Object& submissionResult)
   at Submission#0.<Factory>(Object[] submissionArray)
```