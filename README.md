![Integration tests](https://github.com/EsadCetiner/iredadmin-rule-exclusions-plugin/actions/workflows/integration.yml/badge.svg)

# iRedAdmin-rule-exclusions-plugin
This plugin contains rule exclusions to fix false positives when using iRedMail's iRedAdmin with the OWASP Core Rule Set.

**Disclaimer:** The Pro version of iRedAdmin is not supported but Pull Requests/Issues are welcomed for iRedAdmin Pro users.

## Requirements
- CRS Version 4.0 or newer
- ModSecurity compatable Web Application Firewall

## Installation

For full and up to date instructions on installing plugins, please refer to [How to Install a Plugin](https://coreruleset.org/docs/concepts/plugins/#how-to-install-a-plugin) in the official CRS documentation.

### Conditionally enable plugins for multi-application environments

For full and up to date instructions on how to conditionally enable/disable this plugin on a multisite environment, please refer to [Conditionally enable plugins for multi-application environments](https://coreruleset.org/docs/concepts/plugins/#conditionally-enable-plugins-for-multi-application-environments) in the official CRS documentation.

## Disabling the plugin
The plugin can be disabled by uncommenting rule 9521000 inside ``plugins/iredadmin-rule-exclusions-config.conf`` or by removing the includes for this plugin.

## Reporting false positives
If you find a false positive that this plugin does not cover then please open a new issue or pull request, if creating an issue then please include the following details:

1. CRS Version
2. ModSecurity/Coraza Version
3. modsec audit logs
4. what caused the false positive

## License
Copyright (c) 2023-2025 Esad Cetiner

This plugin is distributed under GNU General Public License V2 (GPLv2), please see the included LICENSE file for details.
