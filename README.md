### ℹ️ About
This is a fork of [tomnomnom/inscope](https://github.com/tomnomnom/hacks/tree/master/inscope) with this PR Added: https://github.com/tomnomnom/hacks/pull/40
```bash
[Diff]
[+] Added `-s | --scope` flag to manually provide a .scope file
[+] Added `-t | --threads` flag to specify number of concurrent workers
[+] Added `-v | --inverse` flag to print OOS (https://github.com/tomnomnom/hacks/pull/40)
```

### 🖳 Installation
Use [soar](https://github.com/pkgforge/soar) & Run:
```bash
soar add 'inscope#github.com.pkgforge-security.inscope'
```

### 🧰 Usage
```mathematica
❯ inscope --help
Filters in scope and out of scope urls (subdomains) from stdin.
Requires you have .scope in CWD or Parent or passed via -s | --scope <file>
To generate one: https://github.com/pkgforge-security/scopegen
For a Bash Alternative: https://github.com/pkgforge-security/scopeview

Options:
 <no options> look for .scope file and filter input (STDIN)
 -v, --inverse Prints out of scope items (default: false)
 -s, --scope <file> Path to scopefile (default: looks for .scope)
 -t, --threads <number> Number of worker threads (default: 8)
```