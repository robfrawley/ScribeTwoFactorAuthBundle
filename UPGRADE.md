Upgrading
=========

Here's an overview what has been changed between versions and if you have to do any work when upgrading. 

## 1.0.0 to 1.1.0

Nothing to upgrade

### Changes
 - Re-factored Doctrine dependency into persister service

## 0.3.0 to 1.0.0

First officially "stable" release.

Changed case of parameter from `$GoogleAuthenticatorSecret` to `$googleAuthenticatorSecret` in `Scheb\TwoFactorBundle\Model\Google\TwoFactorInterface`

### Changes
 - Made security token class configurable.
 - Made POST/GET parameter names configurable.
 - Added unit tests.
 - Refactored trusted feature into separate class.
 - Renamed and reorganized some classes.

## 0.2.0 to 0.3.0

Nothing to upgrade

If you want to use the trusted computer feature, you have to implement TrustedComputerInterface in your user entity. [Read more](Resources/doc/trusted_computer.md)

### Changes
 - Trusted computers can be flagged with a cookie. Once the authentication process has been completed it will skip two factor authentication.

## 0.1.1 to 0.2.0

Nothing to upgrade

### Changes
 - Major code refactoring
 - Implemented an interface for custom two factor authentcation providers

## 0.1.0 to 0.1.1

The default authentication form template requires a route `_security_logout` to be defined, that directs to your logout URL. Alternatively you can configure a custom template.

### Changes
 - Bugfixes
 - Link added to cancel two factor authentication
