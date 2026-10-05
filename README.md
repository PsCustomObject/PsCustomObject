# PsCustomObject

**Infrastructure engineering · Cloud · Automation**

Infrastructure engineer with 20+ years of experience in enterprise IT. I turn operational requirements into reusable tools, with a focus on reducing manual work and making automation easier to maintain.

My background spans Windows infrastructure, Active Directory, Microsoft 365, Entra ID, Azure and PowerShell. My current focus is Linux, AWS, Terraform, Ansible and Python, building on that infrastructure experience.

## Selected projects

### [IT-ToolBox](https://github.com/PsCustomObject/IT-ToolBox)

A PowerShell toolkit built from practical enterprise administration work, now being modernized for PowerShell 7.

It brings together logging, validation, timing, password generation and authenticated string encryption. The modernization introduces explicit module boundaries, behavioral tests and CI workflows for Windows, Linux and macOS. Service-specific operations are maintained separately, with compatibility and migration guidance documented in the repository.

### [LogScanner](https://github.com/PsCustomObject/LogScanner)

A lightweight Go CLI that turns manual searches through PowerShell automation logs into repeatable scans.

Built for the format produced by IT-ToolBox’s `New-LogEntry`, it supports recursive directory scanning, severity and message filters, time ranges, summaries and JSON Lines output. Streaming reads keep memory use independent of total log size, while each match retains its source file and line number. Native CLI checks run in CI on Windows, Linux and macOS, with release builds providing standalone binaries.

### [PowerSCP](https://github.com/PsCustomObject/PowerScp)

A PowerShell module built around the WinSCP .NET library for file transfers and remote file management.

It covers uploads, downloads, directory synchronization, checksums and remote content operations across WinSCP-supported protocols, including SFTP, FTP/FTPS, WebDAV and S3. It supports Windows PowerShell 5.1 and PowerShell 7 on Windows, with explicit host-verification settings, opt-in source removal and `-WhatIf` support for changes.

### [PowerShell-Functions](https://github.com/PsCustomObject/PowerShell-Functions)

Standalone utilities for infrastructure automation, available individually without importing a larger module.

The modernized [New-LogEntry](https://github.com/PsCustomObject/PowerShell-Functions/tree/master/New-LogEntry) implementation demonstrates pipeline batching, buffering, file-specific locking, output-stream handling and optional secret redaction, backed by Pester regression tests. Historical functions retain their own compatibility requirements as they are reviewed.

## Engineering approach

- Build from concrete operational needs and keep each tool's purpose clear.
- Test failure paths, resource cleanup and behavior alongside successful execution.
- Make compatibility, dependencies and migration changes explicit.
- Preserve useful project history while improving the code in focused steps.

## Current focus

Maintaining and modernizing these PowerShell projects, building practical automation tools in Go and Python, and deepening my Linux and AWS skills with Terraform and Ansible.
