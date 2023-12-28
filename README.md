# Clash SS Patch for RC4 method

<img src="logo.png" width="50%" height="auto" alt="Clash-Core">

`Clash` patch, adding `SS` `RC4` cipher support

### Requirement

Clash target version: `1.18`

go require version: `1.21`

### Tested Environment

OS: `Windows 11 22H2`

go version: `go version go1.21.5 windows/amd64`

### Usage

1) copy `config`, `transport` folder to the clash source code folder root, and overwrite files
   ```
   # use patch file to overwrite source file
   cp -rv {config,transport} /clash-source-root/
   ```
2) copy ss_rc4_patch.patch file to the clash source code folder root, and run apply patch command
   ```
   # dryrun, show file changes
   git apply --stat ss_rc4_patch.patch

   # apply changes
   git apply ss_rc4_patch.patch
   ```

### Startup

1) run clash
   ```
   go run /clash-source-root/main.go
   ```

### error

if got this error, upgrade your GoLang version > 1.21

![clash-run-error](2023-12-28_112048.png)

### Go Download

<img src="https://go.dev/images/go-logo-white.svg" alt="Go">

https://go.dev/dl/
