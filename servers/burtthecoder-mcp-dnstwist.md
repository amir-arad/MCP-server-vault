---
type: server
repo_url: https://github.com/BurtTheCoder/mcp-dnstwist
name: DNSTwist MCP Server
owner: BurtTheCoder
stars: 3
last_updated: 2025-02-16
status: active
official: false
verified: false
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/security", "purpose/dns-analysis", "purpose/phishing-detection", "purpose/security-monitoring", "tech/python"]
---

# DNSTwist MCP Server

#status/active #category/security #purpose/dns-analysis #purpose/phishing-detection #purpose/security-monitoring #tech/python

## Description

A Model Context Protocol (MCP) server for dnstwist, a powerful DNS fuzzing tool that helps detect typosquatting, phishing, and corporate espionage.

## Features

- DNS fuzzing capabilities
- Typosquatting detection
- Phishing domain identification
- Corporate espionage monitoring
- Domain permutation generation
- WHOIS record analysis
- DNS record verification
- Domain registration checking
- SSL certificate validation
- Automated reporting

## Installation

```bash
pip install mcp-dnstwist
```

## Usage

```javascript
{
  "mcpServers": {
    "dnstwist": {
      "command": "python",
      "args": ["-m", "mcp_dnstwist"],
      "env": {
        "DNSTWIST_THREADS": "10",
        "DNSTWIST_TIMEOUT": "5",
        "WHOIS_TIMEOUT": "10"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.7
- dnspython
- requests
- tld
- whois
- GeoIP (optional)
- ssdeep (optional)

## Related Servers

- None currently listed