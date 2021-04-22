# timestamp

**INTERNAL USE ONLY:** This GitHub action is not intended for general use.  The only reason why this repo is public is because GitHub requires it.

Obtains the current UTC date/time as a string formatted like: **YYYY-MM-DD HH-MM:SSZ**.

## Examples

```
steps:
- id: get-timestamp
  uses: nforgeio-actions/timestamp 
- id: use-timestamp
  shell: pwsh
  run: Write-Output "TIMESTAMP IS: " + ${{ steps.get-timestamp.outputs.value }}
```
