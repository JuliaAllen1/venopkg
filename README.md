# VenoPackage
VenoPackage, shortened to __venopkg__, and oficially stylized as venoPKG, is a command line utility that acts as what can be called a "package manager aggregator." venoPKG allows installation from several package managers, such as snap, pip, apt-get, and others to come basede on user feedback.
## Syntax
### Install
`venopkg install [package-name]`
If valid package is found, a list of package managers and the repos containing the respective package will be listed. After this, input is allowed. From there:
`[package-manager]`
`>>If installed, [amounnt-of-space] of drive space will be taken up. Install? (Y/N)`
`[Y/n]`
The package will be installed (or not, depending on user choice.)
### Uninstall
`venopkg rm [-p] [package-name]`
If installed package with name [package-name] is found, the following will be returned.
`venopkg: Package found. This package is currently taking up [storage-space] of drivge space. If uninstallation continue, this space will be freed up. Uninstall? (Y/N)`
`Y/N`
 
