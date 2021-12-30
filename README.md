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
### Uninstall
`venopkg rm [-p] [package-name]`

If installed package with name [package-name] is found, the following will be returned.
`venopkg: Package found. This package is currently taking up [storage-space] of drive space. If uninstallation continue, this space will be freed up. Uninstall? (Y/N)`

`Y/N`
 
If `Y`, the program will be uninstalled. If  the option `-p` was selected in the first step, all dependencies will be uninstalled as well. If `N`, uninstallation will be aborted.

## Installing venoPKG

TODO: This section. Cannot be filled out until packaged and rolled out to GH
