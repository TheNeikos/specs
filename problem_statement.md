Problem statement
=================

The concept of open source/free software promotes the idea that any capable
person can contribute to a project. The source of a program can be downloaded
from a project website or hoster. Additionally, the underlying source
repository, specific to the CVS used, can be read.

This way, developers can "clone" (git-ish) or "checkout" (svn-ish) the
repository, stay up-to date and perform modifications to the project. In case of
the latter one, developers often want to make their changes available for
others. At least in the case of distributed VCS like git, this is trivially
possible by pushing the changes to a public remote repository to which the
developer has write-access.

Still, making changes upstream is often not trivial, since only a selected set
of developers will have write-access to the original "upstream" repository. The
maintainer has to incorporate those changes in his or her development
repository after acknowledging the changes. For this to happen, the maintainer
has to be informed of the changes.

Traditionally, patches are sent via email over project mailing lists. When using
git, the maintainer may as well be informed of the changes via a mail containing
a link and a commit hash. The success of platforms like GitHub is in a large
part rooted in the "pull-request" feature, which essentially provides such a
notification.

Filing a PR via commercial platform like GitHub or GitLab naturally requires
contributors to be registered on that specific service. Projects are hence
virtually forced to provide a presence on multiple platforms or accept patches
per mails.

We propose a simple notification mechanism, which will be described in this
document, for notifying a maintainer of code changes to fetch and review. This
mechanism will be contemplated by management and other interfaces, allowing
various kinds of services.

