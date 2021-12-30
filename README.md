# VenoPackage
VenoPackage, shortened to __venopkg__, and oficially stylized as venoPKG, is a command line utility that acts as what can be called a "package manager aggregator." venoPKG allows installation from several package managers, such as snap, pip, apt-get, and others to come basede on user feedback.
## Syntax
### Install
`venopkg install [package-name]`
If valid package is found, a list of package managers and the repos containing the respective package will be listed. After this, input is allowed. From there:

`[package-manager]`

`>>If installed, [amount-of-space] of drive space will be taken up. Install? (Y/N)`

`[Y/n]`

The package will be installed (or not, depending on user choice.)

If no package with name `[package-name]` is found, process will be aborted.
### Uninstall
`venopkg rm [-p] [package-name]`

If installed package with name [package-name] is found, the following will be returned.

`venopkg: Package found. This package is currently taking up [storage-space] of drive space. If uninstallation continue, this space will be freed up. Uninstall? (Y/N)`

`Y/N`
 
If `Y`, the program will be uninstalled. If  the option `-p` was selected in the first step, all dependencies will be uninstalled as well. If `N`, uninstallation will be aborted.

If no package with name `[package-name]` is found, process will be aborted.

## Installing venoPKG

TODO: This section. Cannot be filled out until packaged and rolled out to GH

### Upgrading 
`venopkg vup`

When run, venopkg will search for its install directory, check the contents of `/pkgmngdb` in this repo against `venopkg/pkgmngdb`. If it matches, nothing will occur. If it does not match, `/pkgmngdb` will be updated locally to match remote. 

`venopkg vup -full`

When run, the entire local install directory will be replaced with the contents of the remote repo, except for the required files to upgrade.
