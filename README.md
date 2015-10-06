# Puppet Plugins

This is a Puppet Community curated list of plugins for Puppet and related tooling like `puppet-lint` and `rspec-puppet`. If you have a Plugin you'd like to contribute, please submit a pull request!

## Table of Contents
- [Puppet Lint](#puppet-lint-plugins)
- [Miscellaneous](#miscellaneous)

## Puppet Lint Plugins
| Plugin Link | Description |
| ---         | ---         |
| [trailing_newline](https://github.com/rodjek/puppet-lint-trailing_newline-check) | Extends puppet-lint to ensure that your manifest files end with newlines. |
| [variable_contains_upcase](https://github.com/fiddyspence/puppetlint-variablecase) | Extends puppet-lint to ensure that your variables are all lower case. |
| [param_docs](https://github.com/domcleal/puppet-lint-param-docs) | A check for puppet-lint that validates all parameters are documented. |
| [roles_and_profiles](https://github.com/mcanevet/puppet-lint-roles_and_profiles-check) | A puppet-lint plugin to check that a node definition declares only a role, a role class does not have any param and only declares profiles, and a profiles class can declare anything but a role. |
| [vim_modeline](https://github.com/robertpearce/puppet-lint-vim_modeline-check) | A puppet-lint plugin to check for vim comment (modeline) as the last line in a manifest. |
| [strict_indent](https://github.com/relud/puppet-lint-strict_indent-check) | Extends puppet-lint to ensure that your manifests follow a strict indentation pattern. |
| [unquoted_string](https://github.com/puppet-community/puppet-lint-unquoted_string-check) | A puppet-lint plugin to check that selectors and case statements cases are quoted. |
| [empty_string](https://github.com/puppet-community/puppet-lint-empty_string-check) | A puppet-lint plugin to check for variables assigned to the empty string. |
| [spaceship_operator_without_tag](https://github.com/puppet-community/puppet-lint-spaceship_operator_without_tag-check) | A puppet-lint plugin to check that spaceship operator is called with a tag. |
| [absolute_classname](https://github.com/camptocamp/puppet-lint-absolute_classname-check) | Puppet-lint plugin to check relative class name inclusions. |
| [leading_zero](https://github.com/puppet-community/puppet-lint-leading_zero-check) | A puppet-lint plugin to check for unquoted numbers with leading zero. |
| [newmericvariable](https://github.com/fiddyspence/puppetlint-numericvariable) | Extends puppet-lint to ensure that your variables are not numeric. |
| [file_ensure](https://github.com/puppet-community/puppet-lint-file_ensure-check) | A puppet-lint plugin to check the ensure attribute on file resources. |
| [trailing_comma](https://github.com/puppet-community/puppet-lint-trailing_comma-check) | A puppet-lint plugin to check for missing trailing commas. |
| [version_comparison](https://github.com/puppet-community/puppet-lint-version_comparison-check) | A puppet-lint plugin to check for versions compared as numbers. |
| [global_resource](https://github.com/ninech/puppet-lint-global_resource-check) | Extends puppet-lint to ensure that your manifests have no global resources. |
| [appends](https://github.com/puppet-community/puppet-lint-appends-check) | A puppet-lint plugin to check that the appends operator (+=) is not used (removed in Puppet 4.0.0). |
| [classes_and_types_beginning_with_digits](https://github.com/puppet-community/puppet-lint-classes_and_types_beginning_with_digits-check) | A puppet-lint plugin to check for types and class names that begin with digits. |
| [file_source_rights](https://github.com/camptocamp/puppet-lint-file_source_rights-check) | A puppet-lint plugin to check file rights when providing a source. |
| [alias](https://github.com/camptocamp/puppet-lint-alias-check) | A puppet-lint plugin to check for alias parameters in resources. |
| [security](https://github.com/floek/puppet-lint-security-plugins) | Checks puppet manifests for security related problems. |
| [usascii_format](https://github.com/jpmasters/puppet-lint-usascii_format-check) | A puppet-lint plugin to check that manifest files contain only US ASCII. |
| [package_ensure](https://github.com/danzilio/puppet-lint-package_ensure-check) | A puppet-lint plugin to check the ensure attribute on package resources. |
| [resource_reference_syntax](https://github.com/tuxmea/puppet-lint-resource_reference_syntax) | Extends puppet-lint to ensure that the reference syntax follows Puppet 4 style. |
| [undef_in_function](https://github.com/camptocamp/puppet-lint-undef_in_function-check) | A puppet-lint plugin to check for undef in function calls. |
| [fileserver](https://github.com/camptocamp/puppet-lint-fileserver-check) | A puppet-lint plugin to check if puppet:/// is used instead of file(). |

# Miscellaneous
| Plugin Link | Description |
| ---         | ---         |
| [guard-puppet-lint](https://github.com/alister/guard-puppet-lint) | As Puppet manifest files change, run puppet-lint on them. |
