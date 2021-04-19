# timestamp

**INTERNAL USE ONLY:** This GitHub action is not intended for general use.  The only reason why this repo is public is because GitHub requires it.

Obtains the current date/time as a string.

## Examples

```
steps:
- name: timestamp
  uses: nforgeio-actions/neon-timestamp 
- name: use-timestamp
  shell: pwsh
  run: Write-Output "TIMESTAMP IS: " + ${{ steps.get-timestamp.timestamp }}
```

## Implementation Note

This action assumes that it's being run on a specially configured self-hosted (Windows) jobrunner with the relevant neonFORGE repos already cloned to specific directories.  Generic jobrunners are not supported.
