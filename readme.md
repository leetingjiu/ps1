# about
# Add a new script file named profile.ps1 under the path "C:\Windows\System32\WindowsPowerShell\v1.0".
$Host.UI.RawUI.WindowTitle="Tom"
$colors = @{}
$colors['Variable'] = [System.ConsoleColor]::DarkCyan
$colors['Member'] = [System.ConsoleColor]::Blue
$colors['Command'] = [System.ConsoleColor]::Blue
$colors['Number'] = [System.ConsoleColor]::DarkGreen
$colors['None'] = [System.ConsoleColor]::Black
$colors['Parameter'] = [System.ConsoleColor]::DarkGray
$colors['Keyword'] = [System.ConsoleColor]::Red
$colors['Type'] = [System.ConsoleColor]::DarkBlue
$colors['String'] = [System.ConsoleColor]::DarkGreen
$colors['Operator'] = [System.ConsoleColor]::DarkGray
Set-PSReadLineOption -Colors $colors
