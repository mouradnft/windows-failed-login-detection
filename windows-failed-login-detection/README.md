# Windows Failed-Login Detection Lab

## Objective
Investigate repeated failed Windows login attempts and document the activity using Windows Event Viewer and PowerShell.

## Tools Used
- Windows 10
- Event Viewer
- PowerShell
- Windows Security Logs

## What I Did
1. Created a local test account named `labuser`.
2. Generated multiple failed login attempts using an incorrect password.
3. Filtered the Windows Security log for Event ID `4625`.
4. Reviewed the failed logon details in Event Viewer.
5. Used PowerShell to query failed login events.
6. Exported the events to a CSV file.
7. Wrote a short incident report documenting the activity.

## Key Findings
The failed login attempts generated Windows Security Event ID `4625`.

The logs showed:
- Account: `labuser`
- Logon Type: `2`
- Failure reason: Unknown user name or bad password
- Source address: `127.0.0.1`

The source address indicated that the failed login attempts originated from the local machine.

## Evidence
Screenshots collected during the investigation include:
- Event ID 4625 list
- Event ID 4625 details
- PowerShell query output
- Exported CSV evidence

## Skills Demonstrated
- Windows log analysis
- Event Viewer
- PowerShell
- Authentication-event investigation
- Incident documentation
- Basic SOC analyst workflow

## What I Learned
This project helped me understand how failed Windows authentication attempts appear in the Security event log and how PowerShell can be used to quickly retrieve and export security events for investigation.