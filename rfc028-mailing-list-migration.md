---
RFC: 28
Author: Julian C. Dunn <jdunn@aquezada.com>
Status: Completed
Type: Informational
---

# Mailing List Migration

The Mailing Lists have been migrated to Google Groups.

* [chef@lists.chef.io](https://groups.google.com/a/lists.chef.io/forum/#!forum/chef)
* [chef-dev@lists.chef.io](https://groups.google.com/a/lists.chef.io/forum/#!forum/chef-dev)

Details about the migration can be found the blog posts about the migration:

* [Our mailing lists have moved!](https://www.chef.io/blog/2015/02/10/our-mailing-lists-have-moved/)
* [Mailing List Migration](https://www.chef.io/blog/2015/02/04/14389/)

This RFC proposes the migration of all existing Chef mailing lists
(namely, `{chef,chef-dev}@lists.opscode.com`) into Google Groups.

## Motivation

    As a user of Chef,
    I want the Chef mailing lists on a reliable and easy-to-use platform,
    So that I can easily collaborate with others in the community.

    As a system administrator working at Chef Software, Inc.,
    I want to retire the old mailing list system & not manage one in-house,
    So that I can focus my attention on higher-priority infrastructure issues.

## Specification

This RFC proposes to migrate the existing Sympa-run mailing lists at
`lists.opscode.com` to Google Groups.

There are only two mailing lists of note: `chef` and `chef-dev`. The
desired group names would be the same, but if `chef` is already taken,
we propose that the new group name become `chef-users`.

### Subscriber Migration

All existing subscribers on the current mailing list(s) would be
migrated to their counterparts on Google Groups.

### Archive Migration

Chef Software, Inc. will make a reasonable attempt to migrate the
archives of each of these mailing lists out of Sympa, potentially
using a tool like [sympa-data-exporter](https://github.com/cdelacroix/sympa-data-extract) and into Google Groups.

However, we recognize that this may not be feasible. If it is not,
we will simply create a static HTML site of the old Sympa archives
and publish that.

## Rationale

The existing mailing list system at [lists.opscode.com](http://lists.opscode.com), Sympa, is very old and fragile.
Additionally, it is not a delightful experience for end-users of
Chef, who must navigate a non-intuitive interface to subscribe to,
unsubscribe from, and view the archives of the Chef user and developer
mailing lists.

There have been [previous efforts dating to 2012](http://archive.lists.chef.io/sympa/arc/chef-dev/2012-06/msg00029.html) to try and migrate off Sympa,
but no action has been taken thus far. By codifying the direction in
this RFC, we hope to pave the way for this migration to be done in
an expeditious way.

## Copyright

This work is in the public domain. In jurisdictions that do not allow for this,
this work is available under CC0. To the extent possible under law, the person
who associated CC0 with this work has waived all copyright and related or
neighboring rights to this work.
