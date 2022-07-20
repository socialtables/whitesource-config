# whitesource-config

## Manual Scans
In order to trigger the manual scans, a file called scan.json needs to be pushed to the whitesource-config repo. The scan.json file contains a list of repositories to scan:
```
{
  "repositories": [
    {
      "fullName": "orgName1/repoName1",
      "branchName": "main"
    }
  ]
}
```

The repository list is limited to 10. If there are more than 10, no repositories will be scanned, and a check run will be created.

If a branch name is not specified, the default branch will be scanned.
