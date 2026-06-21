# Mazey

**Mazey** is an early-stage CLI reconnaissance tool for threat triage. It takes _inbound noise_ such as automated scans, bots, misconfigured devices and enriches them using various threat intelligence API's like Virus Total, Shodan, etc...

## Why the name?

`Mazey` is named in tribute to my cat. This is a personal project with long-term goals! 🐈

## Tech stack

- Go (Golang) for the CLI application
- go-fuzzyfinder for interactive selection in the terminal
- Various threat intelligence APIs for data enrichment (e.g., Virus Total, Shodan)

## Usage

```shell
mazey <COMMAND> <ARGUMENT>
```

## Commands

- `blacklist [COUNT]` Shows a list of IP addresses using the `go-fuzzyfinder` library to allow the user to select an IP from the list
- `ipreport <IP_ADDRESS>` Show a report for a specific IP address
- `filereport <FILE_HASH>` Show a report for a specific file hash


## Set environment variables

```bash
VT_API_KEY=<API_KEY>
SHODAN_API_KEY=<API_KEY>
```

## Example

https://github.com/user-attachments/assets/a25ccc85-72b3-4d70-907e-5ece6c838808
