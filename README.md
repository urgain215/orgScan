## orgScan

orgScan runs a simple reverse whois lookup which returns a list of domains owned by people or companies.

This tool is often used for reconnaissance or OSINT (Open Source Intelligence) purposes.

### Installation

`go install github.com/urgain215/goscan@latest`

_This tool requires [golang](https://golang.org/)_

### Options

```console
Usage:
  -n string
        Registrant name, email or domain name of the target (Required)
  -o string
        Output file to write results to (default "domains.txt")
  -p    Print results
```

### Example

```console
$ goscan -n google.com -o google.txt -p

[:] Sending query...
028-hty.com | 2016-05-20 | DROPCATCH.COM 883 LLC
04plan.com | 2020-04-04 | GABIA, INC.
--- snip ---
[:] Writing 500 domain(s) to file google.txt...
[:] Done.
```

&copy; github.com/urgain215
