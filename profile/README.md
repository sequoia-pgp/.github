# Sequoia PGP

Sequoia is a project to provide encryption, verification, and
authentication tools to users and developers to improve their privacy,
and security.  Sequoia is built around the [the OpenPGP
standard](https://datatracker.ietf.org/doc/html/rfc4880), but it is
much more than just a reimplementation of the standard; it is a whole
ecosystem.

Sequoia was started in 2017 by three former GnuPG developers.
Unsurprisingly, its architecture is based on their experiences working
with GnuPG, and interacting with GnuPG's community.

Sequoia's design philosophy is to provide low-level, policy-free (or
policy-light) mechanisms that are secure by default, and cater to
users' needs.  These low-level mechanisms are augmented by higher
level APIs, which progressively add more policy.  This design allows
users to choose the mechanisms and abstractions that are appropriate
for their project.

Sequoia also takes a library-first approach.  Our primary command-line
frontend, `sq`, exposes a lot of functionality, but the libraries are
more flexible.  They also don't call out to the command line tool.

More information about the project is on [our
homepage](https://sequoia-pgp.org/).  Most development is done on
[Gitlab](https://gitlab.com/sequoia-pgp/).

Some of our projects include:

  - [sequoia-openpgp](https://gitlab.com/sequoia-pgp/sequoia/-/tree/main/openpgp):
    Our low-level library.
  - [`sq`](https://gitlab.com/sequoia-pgp/sequoia-sq): Our primary
    command-line frontend.
  - [`gpg`
    chameleon](https://gitlab.com/sequoia-pgp/sequoia-chameleon-gnupg):
    A faithful reimplementation of the `gpg` command-line interface
    using Sequoia's libraries.
  - [Thunderbird
    Octopus](https://gitlab.com/sequoia-pgp/sequoia-octopus-librnp): A
    drop-in replacement of `rnp` for Thunderbird, which restores its
    `gpg` integration, and web of trust support.
  - [Sequoia
    git](https://gitlab.com/sequoia-pgp/sequoia-octopus-librnp): A
    specification, and tool for managing a commit signing policy, and
    checking that commits follow the policy.
  - [OpenPGP interoperability test
    suite](https://gitlab.com/sequoia-pgp/openpgp-interoperability-test-suite):
    An OpenPGP interoperability test suite.
