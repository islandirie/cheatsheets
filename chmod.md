| Permission  | Numeric Value | Symbolic Representation | Description                 | Example                                    |
|-------------|---------------|-------------------------|-----------------------------|--------------------------------------------|
| Read        | 4             | r                       | Read files or list directory contents     | `chmod 444 file.txt` (Read-only for all)   |
| Write       | 2             | w                       | Write to files or create/modify directory contents | `chmod 222 file.txt` (Write-only for all) |
| Execute     | 1             | x                       | Execute files or enter directory          | `chmod 111 script.sh` (Execute-only for all) |
| No Permission | 0           | -                       | No permission               | `chmod 000 file.txt` (No permission for all) |

| User        | Numeric Value | Symbolic Representation | Description                 | Example                                    |
|-------------|---------------|-------------------------|-----------------------------|--------------------------------------------|
| Owner       | 4             | r                       | Owner's read permission     | `chmod 400 file.txt` (Read-only for owner) |
|             | 2             | w                       | Owner's write permission    | `chmod 200 file.txt` (Write-only for owner) |
|             | 1             | x                       | Owner's execute permission  | `chmod 100 script.sh` (Execute-only for owner) |
| Group       | 4             | r                       | Group's read permission     | `chmod 040 file.txt` (Read-only for group) |
|             | 2             | w                       | Group's write permission    | `chmod 020 file.txt` (Write-only for group) |
|             | 1             | x                       | Group's execute permission  | `chmod 010 script.sh` (Execute-only for group) |
| Others      | 4             | r                       | Others' read permission    | `chmod 004 file.txt` (Read-only for others) |
|             | 2             | w                       | Others' write permission   | `chmod 002 file.txt` (Write-only for others) |
|             | 1             | x                       | Others' execute permission | `chmod 001 script.sh` (Execute-only for others) |
