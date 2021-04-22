# timestamp

**INTERNAL USE ONLY:** This GitHub action is not intended for general use.  The only reason why this repo is public is because GitHub requires it.

Obtains the current UTC date/time as a string.

## Examples

```
steps:
- name: timestamp
  uses: nforgeio-actions/neon-timestamp 
- name: use-timestamp
  shell: pwsh
  run: Write-Output "TIMESTAMP IS: " + ${{ steps.get-timestamp.timestamp }}
```
