# Changelog

## Unreleased

* Remove support for Ruby `< 3.1`
* Remove support for Rails `< 7.0`
* Test against Rails 8.0

## 2.0.2 [☰](https://github.com/activeadmin/arbre/compare/v2.0.1...v2.0.2)

* Prefer `require_relative` for internal requires. [#622][] by [@tagliala][]

## 2.0.1 [☰](https://github.com/activeadmin/arbre/compare/v2.0.0...v2.0.1)

* Drop dependency on ruby2_keywords. [#578][] by [@Earlopain][]
* Performance improvements in HTML generation. [#562][], [#617][] by [@tagliala][]

## 2.0.0 [☰](https://github.com/activeadmin/arbre/compare/v1.7.0...v2.0.0)

* Include empty attributes in HTML output. [#543][] by [@javierjulio][]
* Remove table tag defaults. [#542][] by [@javierjulio][]
* Remove component CSS class name default. [#545][] by [@javierjulio][]

## 1.7.0 [☰](https://github.com/activeadmin/arbre/compare/v1.6.0...v1.7.0)

* Remove upper bound dependency limits from gemspec. [#539][] by [@javierjulio][]
* Allow ActiveSupport 7.1. [#537][] by [@tomascco][]

## 1.6.0 [☰](https://github.com/activeadmin/arbre/compare/v1.5.0...v1.6.0)

* Drop support for Ruby 2.6. [#345][] by [@alejandroperea][]
* Add 'main' to HTML5 elements. [#270][] by [@mynnx][]
* Support nested attribute hashes rendered as hyphenated attributes. [#451][] [@Ikariusrb][]
* Lazy-load rails interactions. [#456][] [@ngan][]

## 1.5.0 [☰](https://github.com/activeadmin/arbre/compare/v1.4.0...v1.5.0)

* Avoid mutating string literals. [#292][] by [@tomgilligan][]
* Allow activesupport 7.0. [#314][] by [@tagliala][]
* Drop ruby 2.5 support. [#315][] by [@alejandroperea][]
* Fix keyword delegation in form component. [#318][] by [@deivid-rodriguez][]

## 1.4.0 [☰](https://github.com/activeadmin/arbre/compare/v1.3.0...v1.4.0)

* Allow activesupport 6.1 prereleases. [#242][] by [@deivid-rodriguez][]

## 1.3.0 [☰](https://github.com/activeadmin/arbre/compare/v1.2.1...v1.3.0)

* Drop ruby 2.3 support. [#152][] by [@deivid-rodriguez][]
* Drop ruby 2.4 support. [#177][] by [@deivid-rodriguez][]
* Fix ruby 2.7 kwargs warnings. [#202][] and [#205][] by [@deivid-rodriguez][]

## 1.2.1 [☰](https://github.com/activeadmin/arbre/compare/v1.2.0...v1.2.1)

* Revert [#64][] to fix several regressions, at the cost of reintroducing [#46][]. [#121][] by [@deivid-rodriguez][]

## 1.2.0 [☰](https://github.com/activeadmin/arbre/compare/v1.2.0.rc1...v1.2.0)

_No changes_.

## 1.2.0.rc1 [☰](https://github.com/activeadmin/arbre/compare/v1.1.1...v1.2.0.rc1)

* Fix deprecation warning about single arity template handlers on Rails 6. [#110][] by [@aramvisser][]
* Fix rendering `link_to` with a block in a arbre template. [#64][] by [@varyonic][]
* Drop support for EOL'd rubies (under 2.3). [#78][] by [@deivid-rodriguez][]

## 1.1.1 [☰](https://github.com/activeadmin/arbre/compare/v1.1.0...v1.1.1)

* Use mime-types 2.x for Ruby 1.9 by [@timoschilling][]
* Verify Ruby 2.3 support. [#59][] by [@dlackty][]

## 1.1.0 [☰](https://github.com/activeadmin/arbre/compare/v1.0.3...v1.1.0)

* Tag option `for` sets the attribute when value is a string or symbol [#49][] by [@ramontayag][]

## 1.0.3 [☰](https://github.com/activeadmin/arbre/compare/v1.0.2...v1.0.3)

* Performance improvements [#40][] by [@alexesDev][]
* Added all void elements as self-closing tags [#39][] by [@OscarBarrett][]
* Missing tags added [#36][] / [#39][] by [@dtaniwaki][] and [@OscarBarrett][]

## 1.0.2 [☰](https://github.com/activeadmin/arbre/compare/v1.0.1...v1.0.2)

* make `Element#inspect` behave correctly in Ruby 2.0 [#16][] by [@seanlinsley][]
* prevent `Arbre::Element#flatten` infinite recursion [#32][] by [@seanlinsley][]
* make `find_by_class` correctly find children by class [#33][] by [@kaapa][]

## 1.0.1 [☰](https://github.com/activeadmin/arbre/compare/v1.0.0...v1.0.1)

* Template handler converts to string to satisfy Rack::Lint [#6][] by [@jpmckinney][]
* Fix to `Tag#add_class` when passing a string of classes to Tag build method
  [#4][] by [@gregbell][]
* Not longer uses the default separator [#7][] by [@LTe][]

## 1.0.0 [☰](https://github.com/activeadmin/arbre/compare/v1.0.0.rc4...v1.0.0)

* Added support for the use of `:for` with non Active Model objects

## 1.0.0.rc4 [☰](https://github.com/activeadmin/arbre/compare/v1.0.0.rc3...v1.0.0.rc4)

* Fix issue where user could call `symbolize_keys!` on a
  HashWithIndifferentAccess which doesn't implement the method

## 1.0.0.rc3 [☰](https://github.com/activeadmin/arbre/compare/v1.0.0.rc2...v1.0.0.rc3)

* Implemented `Arbre::HTML::Tag#default_id_for_prefix`

## 1.0.0.rc2 [☰](https://github.com/activeadmin/arbre/compare/v1.0.0.rc1...v1.0.0.rc2)

* Fixed bug where Component's build methods were being rendered within the
  parent context.

## 1.0.0.rc1

Initial release and extraction from Active Admin

[#4]: https://github.com/activeadmin/arbre/issues/4
[#6]: https://github.com/activeadmin/arbre/issues/6
[#7]: https://github.com/activeadmin/arbre/issues/7
[#16]: https://github.com/activeadmin/arbre/issues/16
[#32]: https://github.com/activeadmin/arbre/issues/32
[#33]: https://github.com/activeadmin/arbre/issues/33
[#36]: https://github.com/activeadmin/arbre/issues/36
[#39]: https://github.com/activeadmin/arbre/issues/39
[#40]: https://github.com/activeadmin/arbre/issues/40
[#46]: https://github.com/activeadmin/arbre/issues/46
[#49]: https://github.com/activeadmin/arbre/issues/49
[#59]: https://github.com/activeadmin/arbre/issues/59
[#64]: https://github.com/activeadmin/arbre/pull/64
[#78]: https://github.com/activeadmin/arbre/pull/78
[#110]: https://github.com/activeadmin/arbre/pull/110
[#121]: https://github.com/activeadmin/arbre/pull/121
[#152]: https://github.com/activeadmin/arbre/pull/152
[#177]: https://github.com/activeadmin/arbre/pull/177
[#202]: https://github.com/activeadmin/arbre/pull/202
[#205]: https://github.com/activeadmin/arbre/pull/205
[#242]: https://github.com/activeadmin/arbre/pull/242
[#270]: https://github.com/activeadmin/arbre/pull/270
[#292]: https://github.com/activeadmin/arbre/pull/292
[#314]: https://github.com/activeadmin/arbre/pull/314
[#315]: https://github.com/activeadmin/arbre/pull/315
[#318]: https://github.com/activeadmin/arbre/pull/318
[#345]: https://github.com/activeadmin/arbre/pull/345
[#451]: https://github.com/activeadmin/arbre/pull/451
[#456]: https://github.com/activeadmin/arbre/pull/456
[#537]: https://github.com/activeadmin/arbre/pull/537
[#539]: https://github.com/activeadmin/arbre/pull/539
[#542]: https://github.com/activeadmin/arbre/pull/542
[#543]: https://github.com/activeadmin/arbre/pull/543
[#545]: https://github.com/activeadmin/arbre/pull/545
[#562]: https://github.com/activeadmin/arbre/pull/562
[#578]: https://github.com/activeadmin/arbre/pull/578
[#617]: https://github.com/activeadmin/arbre/pull/617
[#622]: https://github.com/activeadmin/arbre/pull/622

[@aramvisser]: https://github.com/aramvisser
[@LTe]: https://github.com/LTe
[@OscarBarrett]: https://github.com/OscarBarrett
[@alejandroperea]: https://github.com/alejandroperea
[@alexesDev]: https://github.com/alexesDev
[@deivid-rodriguez]: https://github.com/deivid-rodriguez
[@dlackty]: https://github.com/dlackty
[@dtaniwaki]: https://github.com/dtaniwaki
[@gregbell]: https://github.com/gregbell
[@jpmckinney]: https://github.com/jpmckinney
[@kaapa]: https://github.com/kaapa
[@ramontayag]: https://github.com/ramontayag
[@seanlinsley]: https://github.com/seanlinsley
[@timoschilling]: https://github.com/timoschilling
[@varyonic]: https://github.com/varyonic
[@tagliala]: https://github.com/tagliala
[@tomgilligan]: https://github.com/tomgilligan
[@mynnx]: https://github.com/mynnx
[@Ikariusrb]: https://github.com/Ikariusrb
[@ngan]: https://github.com/ngan
[@tomascco]: https://github.com/tomascco
[@javierjulio]: https://github.com/javierjulio
[@Earlopain]: https://github.com/Earlopain
