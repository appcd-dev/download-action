# Appstack IaC Downloader

This repository provides a GitHub Action for downloading Infrastructure as Code (IaC) for a specified appstack. 

## Inputs

- **appstack_uuid**: (required) The UUID of the appstack to download.
- **output**: (optional) The file destination for the zipped IaC code. Defaults to `./iac`.
- **latest**: (optional) Set to `true` to download the IaC of the latest version of the specified appstack. Defaults to `false`.

## Usage

To use this action, include it in your workflow YAML file

```yaml
- name: Download IaC for Appstack
  uses: appcd-dev/download-action@
  with:
    appstack_uuid: 'your-appstack-uuid'
    output: 'iac'
    latest: 'true'
```

