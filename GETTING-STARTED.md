# PowerShell Script Runner: launch a script and read its output

## Run a local PowerShell script

1. Download the portable executable from the [official product page](https://aicreatenow.com/scriptrunner.html).
2. Read the `.ps1` script you intend to run and check its own requirements, such as modules, input files and network access.
3. Open Script Runner and approve the Administrator prompt.
4. Select the local script, launch it, and read the console output. The console stays open after execution so errors remain visible.
5. Use **Recent Scripts** to find a previously launched script, or **Remove History** to clear the saved list.

## Common questions

**Does Script Runner fix PowerShell errors?** It launches scripts and keeps their output visible. It does not generate, repair, debug or certify the script's code.

**Does it permanently change execution policy?** The launcher uses `-ExecutionPolicy Bypass` for the child PowerShell process. It does not permanently change the computer's execution policy.

**Where is the recent list?** Up to 20 successfully launched script paths are kept locally at `C:\ProgramData\ScriptRunner\Config\RecentScripts.txt`.

**What should I check if a script fails?** Read the actual console error and confirm the script's required files and modules are available. When requesting launcher support, state whether the same reviewed script runs directly in PowerShell. Share a small example only if needed, after removing private data.

Administrator scripts can change Windows. Script Runner does not inspect them for malicious commands; only launch scripts you understand and trust.

[Back to product overview](README.md) · [Support](SUPPORT.md)
