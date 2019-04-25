# Terraforming Rails

A collection of tools and guides to help you turn legacy code into [legendary code](https://twitter.com/cackhanded/status/1019216124729352192?s=21).

Based on the RailsConf 2019 talk ["Terraforming legacy Rails applications"](https://railsconf.com/program/sessions#session-832) (slides and video are coming soon).

<a href="https://evilmartians.com/">
<img src="https://evilmartians.com/badges/sponsored-by-evil-martians.svg" alt="Sponsored by Evil Martians" width="236" height="54"></a>

## Tools

### Unrealesed scripts

These scripts have been created during the development of different Rails projects at [Evil Martians](http://evilmartians.com).

They're not universal enough to be extracted into libraries (some depend on particular Rails version or rely on project-specific assumptions), but they could be used a starting point for building tools for your project.

- [Lint/Env](./tools/lint_env) – RuboCop cop (restrict the usage of `ENV` and `Rails.env` in the app)
- [FactoryLinter](./tools/factory_linter) – lint factory definitions
- [TimecopLinter](./tools/timecop_linter) – make sure you always travel back in time when using Timecop
- [TemplatesTracker](./tools/templates_tracker) – track unused templates
- [GemTracker](./tools/gem_tracker) - track potenially unused gems.

### Gems

#### Tests
- [TestProf](http://test-prof.evilmartians.io) – analyze and improve test suite performance

#### Security
- [bundler-audit](github.com/rubysec/bundler-audit) – check deps for known CVEs
- [brakeman](https://brakemanscanner.org) – detect the app code's security issues

#### Database
- [database_validations](github.com/toptal/database_validations) – validations consistent with the DB constraints
- [database_consistency](github.com/djezzl/database_consistency) - check the consistency of the DB constraints and models validations
- [isolator](https://github.com/palkan/isolator) – detect transactions with side-effects (_non-atomic_)

#### Dead code elimination

- [traceroute](github.com/amatsuda/traceroute) – detect unused routes/controller actions

### Automation Tools

- [lefthook](https://github.com/Arkweid/lefthook) – language-agnostic git hook manager
- [danger](http://danger.systems) – code review automation helper

## Resources

- [Fight the flaky tests](./guides/flaky.md)

## License

The code is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
