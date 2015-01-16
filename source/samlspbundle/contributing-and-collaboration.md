---
layout: samlspbundle
title: SamlSpBundle
---

Contributing and collaboration
============

Aerialship/SamlSpBundle is open source project under MIT license and contribution is welcome. Considering its youth and pre v1 state, its final v1 details not yet well known and the contribution procedures are not still well structured. But some general principles must be applied.

Announcements
-------------
You can follow announcements on twitter [@aerialship](https://twitter.com/aerialship)

LightSaml
---------
Aerialship/SamlSpBundle is based on the SAML data model implemented by [aerialship/lightsaml](/lightsaml).
It was done that way to enable SAML usage in non-symfony projects.
That in these early steps of those two projects introduce small complication and effort to distinguish the origin of
the issue. Please consider this before making and issue in this project and vise verse.


Questions
---------
You can create an issue on [Aerialship/SamlSpBundle github issues page](https://github.com/aerialship/SamlSPBundle/issues) with a question, and core team or wider community will respond when possible.
Please mark question issues with the "question" label.


License
-------
Before you start, you must know that all the patches you are going to submit must be released under the *MIT license*.

PR Reviews
----------
Everybody using the bundle is welcome to review and test a pull request. Better do it before the merge, spare yourself of broken functionality and us reverting the merge.


Code changes
------------
In case you need a code change, you are kindly asked first to make an issue on [Aerialship/SamlSpBundle github issues page](https://github.com/aerialship/SamlSPBundle/issues) with full specification. That issue will be discussed and confirmed if and what kind if implementation is required to fulfill it. Without it, you're risking your PR is not compatible with the common project goal and that it will be rejected. Even in case your PR is not accepted, the issue will still remains opened with solution specification for others or yourself to make a new PR on the same issue.

Please follow these rules:

Bugs
-----
 * Use the title field to clearly describe the issue
 * Specify it's a bug - either labeling it "bug" or clearly state it's a malfunction within first first lines of comment
 * Give as much detail as possible about your environment (PHP version, Symfony version, SamlSPBundle hash, Metadata files you're working with...)

New features
------------
 * Use the title field to clearly describe the issue
 * Specify it's a new features - either label it "enhancement" or clearly state it's a new feature within first few lines of comment
 * Tell it's purpose and problems it would solve,
 * Describe step by step the use case it should implement