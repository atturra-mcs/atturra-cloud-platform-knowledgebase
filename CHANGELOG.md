
# Change Log
All notable changes to this project will be documented in this file.
 
The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).
 
## [Unreleased]
 
### Added
- Added new functionality to allow individualised routes for each VPN Client (#51)
- Added and published available knowledgebase including FAQ, architecture design and key configuration information (#60)
- Added and published maintenance plan for kubernetes cluster and containers (#35)

### Removed
- Azure Front Door and Private Links (#54)
 
### Changed
- Changed public ingress to CloudFlare from Azure Front Door (#54)
- Changed Boomi Gateway installation to a container (#33)

### Security
- Action Code Verification Test results (#22, #25, #26, #27)
 
## [1.2.0] - 2024-04-20
 
### Added
- Added the changelog
- Added a Shared Pod - Github Self-Hosted Runner (#52)
- Added a Shared Pod - LetsEncrypt Certrotation (#1)
- Added a Shared Pod - Octopus Deploy Tenticle (#2)
- Added new function to create IP allow-lists per domain (#17)
 
### Changed
- Enabled Firewall logging (#15)
- Enabled Azure Front Door logging (#16)

### Deprecated

### Removed
 
### Fixed
- Fixed an issue preventing Ingress Configuration with Azure Front Door to be automated (#28)
- Fixed an issue in CICD Deployment where Memory and CPU limits were too low (#57)
- Fixed an issue with VPN Client Configuration to avoid communication issues to client network (#50)
- Fixed an issue which prevented custom domains (vanity urls) to access the Web Application Firewall (#18)
- Fixed an issue causing Atom/Molecule Pods to hang (#20)
- Fixed an issue preventing Octopus Deploy Tentacle from updating (#45)
- Fixed an issue preventing pods from pulling images from the Azure Container Registry (#49)

### Security
- Action Code Verification Test results (#23, #24)
- Updated Kubernetes Admin to disallow access from untrusted sources (#14)
- Implemented manual approval steps for deploying to shared services (#21)
