# Contributing

## Requesting a Package

To request a package, simply **fork this repository**, clone the forked repo, and create *yaml* configuration files for the package.

It should be packaged for each of the following platforms and architectures that the project provides binary releases for:

- linux/x86_64
- linux/aarch64 (arm64)
- darwin/x86_64
- darwin/aarch64 (arm64)

**NO INCOMPLETE SUBMISSIONS WILL BE ACCEPTED, unless the project itself does not publish binaries for that platform/architecture**

Create a **pull request**, and fill out the template.

Wait for it to be reviewed, and hopefully **merged**!

## Example package configuration

```yaml
name: "example"               # (path to) binary name
repo: indium114/wares         # GitHub repo
asset: "example*Linux*x86_64" # pattern to match asset name against
removetoplevel: false         # remove top level dir of archive
multiple: false               # denotes that *all* files must be symlinked
```
