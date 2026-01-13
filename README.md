# Socket GitHub Actions Scanning Demo

This repository demonstrates Socket's GitHub Actions ecosystem scanning feature.

## Purpose

When you fork this repo and connect it to Socket via the GitHub App, Socket will scan the workflow files in `.github/workflows/` and detect security issues with GitHub Actions used in your CI/CD pipelines.

## What Socket Detects

Socket scans your GitHub Actions workflows for:
- Malware and obfuscated code
- Typosquat actions (misspelled action names)
- Unsafe data flows via Argus taint tracking
- License and policy violations

## Testing the Feature

1. Fork this repository to your GitHub organization
2. Ensure Socket's GitHub App is installed on your org
3. Make sure GitHub Actions scanning is enabled (contact Socket support)
4. Open a PR or trigger a scan
5. Check the Socket dashboard for alerts under the `github` ecosystem

## Demo Workflow

The workflow in this repo intentionally uses a typosquat action (`acitons/checkout` instead of `actions/checkout`) to demonstrate Socket's detection capabilities.

**Note:** The workflow will fail to run because the typosquat action doesn't exist, but Socket will still detect and flag it during the scan.

## Learn More

- [Socket GitHub Actions Scanning](https://socket.dev/blog/introducing-github-actions-scanning-support)
- [Socket Documentation](https://docs.socket.dev)
