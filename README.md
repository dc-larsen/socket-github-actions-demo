# Socket Dependency Scanning Demo

This repository demonstrates Socket's dependency scanning capabilities.

## Purpose

When you fork this repo and connect it to Socket via the GitHub App, Socket will scan the dependencies and detect security issues.

## What Socket Detects

This demo includes `lodahs@0.0.1-security`, a known typosquat of the popular `lodash` package. Socket will flag this as:
- **Possible typosquat attack** - Package name is similar to `lodash`
- **Known malware** - This specific version is marked as a security test package

## Testing the Feature

1. Fork this repository to your GitHub organization
2. Ensure Socket's GitHub App is installed on your org
3. Open a PR or push to trigger a scan
4. Check the Socket dashboard for alerts

## Learn More

- [Socket Documentation](https://docs.socket.dev)
- [Socket Security](https://socket.dev)
