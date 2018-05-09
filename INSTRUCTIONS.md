# Table of Contents

* [Release Instructions](#32B21988C17C11E687F7003EE1B763F8)
    * [Major Reviews](#3449D4BEC17C11E68DD1003EE1B763F8)
        * [Informal Approval](#37D9C8B4C17C11E6AE38003EE1B763F8)
        * [Code Cleanup and Release Preparation](#3981656EC17C11E6B2AE003EE1B763F8)
        * [File an ARL Form 1](#4066B47EC17C11E6BFC7003EE1B763F8)
        * [Intellectual Property Review](#45A6CE62C17C11E6A6C0003EE1B763F8)
        * [Obtain Invention Evaluation Committee (IEC) Approval](#433214A2C17C11E6952E003EE1B763F8)
        * [Distribution Methods](#476F65D4C17C11E69E2F003EE1B763F8)
        * [Final Release and Principal Developer Responsibilities](#49715508C17C11E69019003EE1B763F8)
    * [Minor Reviews](#4ADBEADCC17C11E6B9BC003EE1B763F8)
    * [Incorporating External Contributions](#4D5F4B34C17C11E6ADBB003EE1B763F8)
    * [A Note on Impact and Metrics](#A_Note_on_Impact_and_Metrics)
        * [Evidence of Impact](#5092761CC17C11E6B23A003EE1B763F8)
        * [Software Maturity and Software Engineering](#53A23266C17C11E6BEEE003EE1B763F8)
* [Contributor License Agreement (CLA)](#D3DC705AC3C411E6BBB4003EE1B763F8)
* [Legal Analysis - Software Protection & Release Mechanisms](LEGAL_ANALYSIS.md)
* [Glossary](GLOSSARY.md)
* [Footnotes](#93338EDCC17C11E6B720003EE1B763F8)

# <a name="32B21988C17C11E687F7003EE1B763F8"></a>Release Instructions

These instructions MUST be followed when ARL personnel release software to, or
accept contributions from, the general public.  If a project does not yet have
any software associated with it (such as when a project is being initially
formulated) and the project is intended to be released to the general public,
then this process MUST still be followed.

## <a name="3449D4BEC17C11E68DD1003EE1B763F8"></a>Major Reviews

The major review process MUST be followed if any of the following are true:

* This is the first release of the project.
* It has been more than 1 year since the last time a major review has been
  done and the project is still active (material is being published to the
  public by ARL employees).
* The principal developer(s) feel they have accomplished something of note and
  wish to get credit for it in their performance metrics.
* The project's scope has changed sufficiently that any of the principal
  developers, their OPSEC officers, or anyone in their chains of command
  believe a new one ought to be filed.
* There are legal issues that need to be reviewed.
* New inventions (inventions that have not already been disclosed in a prior
  major review) are being described.
* The project is being archived.  In this case, this is likely to be the final
  review of the project.
* A project that was archived is being restarted.

### <a name="37D9C8B4C17C11E6AE38003EE1B763F8"></a>Informal Approval

Before developer(s) release software, they MUST obtain informal approval from
their supervisor(s).  If their supervisor(s) do not approve release of the
software, then the software MUST NOT be released.  Do not continue with this
process.  When deciding if a project can be released, review the section
[Issues Related to Releasing Source Code](#25060DEEC17C11E6B53F003EE1B763F8)
to decide if it will be possible to release the code.  If you have questions,
consult ARL's Chief Counsel's Office for help.  Projects that cannot be given
a release statement of "Approved for public release; distribution unlimited"
MUST NOT go through this process.

### <a name="FBD310E6377C11E891F1003EE1B763F8"></a>Complete ARL Form TBD

ARL Form TBD is used to perform a Major Review.  The guidance in this section
supplements the instructions in that form.

#### <a name="3981656EC17C11E6B2AE003EE1B763F8"></a>Code Cleanup and Release Preparation

This section applies to everything that is being released, including any older
commits in any repositories.  By design, repositories preserve history, which
can include material that should not be published.  It is the responsibility
of the project's developers to ensure that both the current code and any
history in any repositories that are proposed for release have been properly
scrubbed before the material is reviewed for release.  Remember that a formal
review can only be done on what is actually being released, so cleaning up the
code after the formal review is not an option.  If a project is being
formulated, but does not yet have any code associated with it, this section
SHOULD be used as a guide for how to write the software.

Fast-moving projects often accumulate useless, nonfunctional, or otherwise
undesirable code and other material that needs to be cleaned up.  Before
moving forward with the rest of the process, the project MUST be cleaned up to
ensure it meets certain minimum standards.  Software that is released to the
public is similar to a publication and SHOULD be treated like one.  The
developer(s) MUST ensure that there is no embarrassing, disparaging, or
otherwise unprofessional language in what is released. Language that would not
be used in a professional journal MUST NOT be used in software.  Direct any
questions about this to the ARL Public Affairs Office (PAO).

Where possible, it is wise to follow best practices in software engineering.
Because of the wide variety of programming languages in use, project goals,
etc., ARL wants to avoid forcing a single process on any developers or group.
For this reason, ARL has chosen a minimal set of requirements and provides
some best practice suggestions.  Individual implementation of the voluntary
portions is RECOMMENDED as they may have an effect on impact and performance
metrics.  See [A Note on Impact and Metrics](#A_Note_on_Impact_and_Metrics)
for details on performance metrics.

As discussed at [Licensing and the ARL Contributor License Agreement (ARL
CLA)](#2DF49A4AC17C11E69E3A003EE1B763F8), all projects will have their
material licensed under both the CC0 license, and a license that is both
approved by OSI and the ARL Chief Counsel's Office. The developer(s) MUST
consult with the ARL Chief Counsel's Office when selecting an OSI-approved
license. All contributions that have copyright attached MUST be licensed to
ARL under the OSI-approved license chosen by the project's developer(s), and
they MUST be redistributed under the same license when the software is
redistributed. Works that do not have copyright attached MUST be accepted and
redistributed under the CC0 license. All contributions MUST be irrevocable
under the given license.  Questions about this can be directed to ARL Legal
for clarification.

Once the license is chosen, the developer(s) MUST provide copies of the
license text in a file named `LICENSE.txt` at the root of the project's
repository. This MUST contain both the text of the OSI-approved license and
the CC0 license.  The `LICENSE.txt` file MUST also contain a notice that those
portions of the material that do not have copyright attached within the
jurisdiction of the United States of America are distributed under the terms
of the CC0 license, and that all other portions of the work are distributed
under the terms of the OSI-approved license in the `LICENSE.txt` file.  An
example of how this can be done for the CC0 license and the [Apache
2.0](http://apache.org/licenses/LICENSE-2.0) license is given in the
[LICENSE.txt](LICENSE.txt) file of this guidance.

The `LICENSE.txt` file MUST be a plain-text file in either ASCII or UTF-8
encoding.  The README file (described below) MUST state the name of the file
that contains the complete license<sup>[1](#Footnote_1)</sup>.  If the project
has a webpage, the licenses being used MUST be stated somewhere on the
webpage, with a link pointing to the project's `LICENSE.txt` file.

A "README" file MUST be created in the top level directory of the project. The
"README" file MUST be a plain-text file in either ASCII or UTF-8 encoding. The
file may be named "README", "README.txt", or "README.md".  As a note, if the
developers choose to use [GitHub](https://github.com) as the distribution
method, it is RECOMMENDED that the file be named "README.md", and that the
file be written in [GitHub-flavored
Markdown](https://guides.github.com/features/mastering-markdown/).  Throughout
this document the file will be called "README" regardless of what suffix is
used on the actual file.  The "README" file must contain at least the
following in it:

* The intended purpose of the software.
* A note pointing to the license or contract covering the software.
* At least some basic documentation on how to build and use the software.
* An explanation that external contributors MUST execute a CLA before their
  contributions will be accepted.  See
  [Incorporating External Contributions](#4D5F4B34C17C11E6ADBB003EE1B763F8)
  for more information.

In addition, the "README" SHOULD describe what valuable contributions the
principal developers would welcome from the community.  This will help the
public focus on efforts that are most likely to be accepted into the project.

While only the "README" file is mandatory, other documentation is highly
desirable.  This can include comments in the source code, high-level design
documentation, etc.  There are many methods and tools to support this type of
documentation.  Where reasonable, please document both high- and low-level
design details, as well as how the software should be used.

Example code is also a form of documentation.  If the project is a library, it
can be useful to provide small, complete, and well-documented programs that
illustrate how to use the software.  If possible, refer to publications and
projects that used or referred to this code; they can become additional
examples of how to use the code, as well as testimonials for why the code
should be used.

Unit tests are strongly RECOMMENDED.  They can not only increase confidence
that the code was written correctly, but they can also convince a user that
the code is behaving as expected on the system on which it is installed.  This
will increase the likelihood that others will be willing to use the code,
which can increase the overall impact of the project. In addition, unit tests
can serve as examples of how to use the code; this can be invaluable when a
user is trying to understand the documentation.

For legal reasons, all language talking about the project MUST be prefixed
with "ARL".  For example, if a project is named WhizBang, then all literature
in the package MUST refer to it as "ARL WhizBang" or the "ARL WhizBang
project." "ARL" is a federally registered trademark and using it in this
manner adds some degree of trademark protection to a project.

Create a file called `code.json` in the root directory of your project.  This
file MUST follow the schema described
[here](https://code.gov/#/policy-guide/docs/compliance/inventory-code). An
example of a correctly formatted `code.json` file is provided
[here](code.json).  Download and modify it to fit your project.

#### <a name="4066B47EC17C11E6BFC7003EE1B763F8"></a>File an ARL Form 1

An ARL Form 1 MUST be filed.  In the process described in this document, the
primary purpose of the ARL Form 1 is for OPSEC review, but it also serves the
secondary purposes of describing releases for publicity and metrics.  To
support this, a short abstract describing the software MUST be written.  The
abstract SHOULD be at most one page in length and provide the following
information:

* The name of the project.
* A description of the project.  This includes what it does and what its
  intended purpose is.  This SHOULD be as complete as is reasonably possible.
  Portions of the "README" file MAY be copied here.
* If this is not the first time that this project has undergone a major
  review, list what necessitated the current review.  Reasons might be simple
  such as "annual review", or may be more complicated, such as the scope of a
  project changing sufficiently that a security review is warranted.  Major
  accomplishments are also a good reason for a review as a major review is the
  only way to document performance for performance metrics (see
  [A Note on Impact and Metrics](#A_Note_on_Impact_and_Metrics) for more
  information).
* Answers to the following questions so that the ARL Chief Counsel's Office
  can do an intellectual property review (see
  [Intellectual Property Review](#45A6CE62C17C11E6A6C0003EE1B763F8) for more
  information):
    * A list of all contributors and their employment affiliation at the time
      of their contribution.  Note that a contribution is material given to
      the project directly; it doesn't include code copied by the project's
      owners from external sources.
      * If there is more than one contributor, did they each intend to merge
        their contributions at the time they made them into a unified joint
        work? (yes/no).  If you have questions about this, consult the ARL
        Chief Counsel's office.
    * Does the software contain, or is it based on, code not owned by the U.S.
      Government?  (e.g., an ARL contractor, an Open Source contributor, code
      copied from external sites).  If the project does contain code not owned
      by the US Government, list out the code and code's owner.  If the code
      was downloaded under a license (e.g., the Linux kernel, which is
      distributed under the GPL version 2), list the code and the license
      instead of the contributors.  If the software was provided by an ARL
      contractor, provide the contract number.  In general, provide enough
      information so that the ownership and licensing of all code not owned by
      the US Government can be determined.
    * Has any version of the software been previously distributed outside of
      ARL?  If yes, please explain the circumstances.
    * Which OSI-approved license is the code being released under.
* A list of all software-related inventions that the developers believe
  patents could be pursued for, and reasons for why ARL should waive its
  rights to pursue a patent on each.  This will help the Invention Evaluation
  Committee decide whether it would be better to pursue patents, or waive
  ARL's rights.  If there are no software-related inventions claimed, then
  this must be noted (see [sample_abstract3.md](sample_abstract3.md) for an
  example of this).

Examples of how to write abstracts are provided in the files
[sample_abstract1.md](sample_abstract1.md),
[sample_abstract2.md](sample_abstract2.md), and
[sample_abstract3.md](sample_abstract3.md).  Note that the examples
deliberately include information that would cause ARL's Legal Counsel or the
IEC to ask further questions.  When you write your abstract, be as complete as
possible; omitting, obfuscating, or hiding information about the origins of
contributions could expose ARL to litigation.  The information in the abstract
will be used throughout the rest of this process, so it MUST be as accurate
and complete as possible.

As noted above, if this is not the first major review of this project then
developers should document the major accomplishments of this project since the
last major review was done.  This documentation provides supervisors the
information they need to give proper credit on performance reviews.   Note
that while ARL wants to credit developers for the impact the software has
made, it will not "double count" what developers have done by including the
impact from earlier major reviews.  Only the impact made since the last time
the major review process was completed for the project MAY be included.

This abstract, along with everything planned on being released (software,
source code, documentation, etc.), MUST be fully reviewed by a level 1 OPSEC
officer.  If this is not an initial review, the OPSEC officer MAY choose to
only review what has changed since the last review, but both the developer(s)
and the OPSEC officer are responsible for the release as a whole.  Thus, even
if the changes are cleared for public release, if the release as a whole
cannot be cleared for release, then the changes are not cleared for release
either. To be cleared for release, the project as a whole MUST receive an
"Approved for public release; distribution unlimited" statement.

No one is permitted to OPSEC-approve material that he or she created.

#### <a name="45A6CE62C17C11E6A6C0003EE1B763F8"></a>Intellectual Property Review

Although ARL MAY choose to waive ARL's rights to any IP established in
software, if a developer has incorporated contributions from others, those
contributors may have rights to those contributions that restrict ARL's
ability to release the software.  Thus, before the software can be released,
the following questions MUST be addressed:

* Has every part of the proposed release been generated by Government
  employees in the course of their duties?
* If not, is there permission from every other rights holder to release all of
  the other parts under the project's license?

The principal developer(s) MUST consult with ARL Legal to perform an IP review
(this review MAY be done by email or any other convenient and legal means).
If there are external contributions that were not contributed under the
project's license, then the principal developer(s) MUST determine the license
and copyright information for each contribution. Provide these to ARL Legal
for review and final determination if the licenses are compatible with the
license or contract under which the software is being released.  If ARL Legal
determines that there are impediments to releasing the software, whatever
permissions are necessary MUST be obtained before the software is released.
If it is not possible to obtain the necessary permissions, then the software
MUST NOT be released.  Do not continue with the rest of this process.  If ARL
Legal agrees that there are no IP impediments to releasing the software, then
ARL Legal MUST send a digitally signed email to the principal developer(s)
stating so.

Note that copyright protection attaches to all literary works, including
software, when they are created<sup>[3](#Footnote_3)</sup>.  This includes
software copied off of blogs, sites like http://stackoverflow.com/, and any
other sources.  If such code or documentation has been copied into a project
without permission and permission from the rights holder cannot be obtained,
it may not be possible to release the software.

This step MAY be done in parallel with the steps described below.

#### <a name="433214A2C17C11E6952E003EE1B763F8"></a>Obtain Invention Evaluation Committee (IEC) Approval

ARL may have IP interests in the software.  Before the software can be
released, the IEC MUST determine that it is in the best interest of the
Government and ARL to waive any IP rights that ARL might have and release them
to the public.  To do so, the principal developer(s) MUST inform the current
chair of the IEC (or the chair's delegate) of the intention to release the
software by sending the chair a digitally signed email that contains the
following:

* The abstract that was submitted as a part of the ARL Form 1 process above.
  The related software is not sent to the IEC chair (or the chair's delegate)
  unless he or she requests it. As explained in the section
  [File an ARL Form 1](#4066B47EC17C11E6BFC7003EE1B763F8) This MUST contain a
  list of all software-related inventions that the principal developer(s) and
  his or her supervisor believe are contained in the
  work<sup>[2](#Footnote_2)</sup>.  If there are no inventions, then this MUST
  be noted as well so that the IEC will know that this requirement was not
  skipped.
* For each invention, an explanation of why the principal developer(s) and
  their supervisor(s) believe that it is in the best interest of ARL and
  Government to waive ARL's IP rights and place the inventions irrevocably
  into the public domain.

If the chair (or the chair's delegate) agrees that ARL should waive any patent
or other IP interests ARL may have, then the chair (or the chair's delegate)
will reply back with a digitally signed email with a statement similar to the
following:

`<<Software name>> is to be released to the public in the manner (open source
and/or public domain) proposed for promoting its commercial and non-commercial
use. It is in the best interest of the government to waive any and all patent
rights ARL may be able to assert or establish in the software.`

If the principal developer(s) has received approval from IEC chair (or the
chair's delegate), then the principal developer(s) MAY continue with the rest
of this process.

If the IEC chair (or the chair's delegate) believes that ARL has IP interests
that ARL wants protected, then the principal developer(s) and the chair (or
the chair's delegate) MUST discuss the issues to determine how to move
forward.  This discussion MAY be performed by email, telephone, or any other
convenient and legal means. Records of the final determination MUST be kept by
the principal developer(s).  If it is determined to be in the best interests
of ARL and the Government to seek patent protection, then the rest of this
process does not apply.  Do not continue with the rest of this process.

To determine the appropriate person to contact within the IEC, consult ARL
Legal.

### <a name="476F65D4C17C11E69E2F003EE1B763F8"></a>Distribution Methods

There are many different ways of distributing software.  The ARL GitHub site
is the RECOMMENDED method, but is not the only method.  The principal
developers MAY choose to distribute by FTP, email, another website, or other
means, in addition to or in place of GitHub.  For any and all distribution
methods chosen, the principal developer(s) are responsible for creating their
own accounts.  If the distribution method uses email addresses as part of the
sign up process, then the principal developer(s) MUST use their Government
email addresses.  All login accounts MUST be reported to the principal
developer(s)' supervisors.  Passwords MUST be kept secret.  If a site uses
cryptographic authentication such as public/private key pairs, principal
developer(s) MAY choose to use this facility in addition to, or instead of,
passwords.  Private keys MUST be treated like passwords and kept secret.

Where possible, it is strongly RECOMMENDED that projects be distributed via
the ARL GitHub site.  This will make it significantly easier to gauge the
impact of the project by the Technology Transfer and Outreach Office (T2O2)
and by a supervisor, which will impact performance metrics.  This will also
simplify compliance with
[M-16-21 MEMORANDUM FOR THE HEADS OF DEPARTMENTS AND AGENCIES](https://code.gov/#/policy-guide/policy/introduction).

### <a name="49715508C17C11E69019003EE1B763F8"></a>Final Release and Principal Developer Responsibilities

If the software is approved for final release and there is not yet a project
for it on GitHub, then the T2O2 will generate a project on the [ARL GitHub
organization site](https://github.com/USArmyResearchLab).  If there is already
a project on the ARL GitHub organization for the software, then the T2O2 will
note the release for metrics purposes, but will take no other action.  If a
developer chooses not to use the ARL GitHub organization site, he or she MAY
request that the T2O2 not create a project.  However, as mentioned in
Distribution Methods, it is strongly RECOMMENDED that GitHub be used to
distribute software.

The principal developer(s) SHOULD put their software on their project's site.
The T2O2 will publicize this site on behalf of the principal developer(s). The
software MAY also be distributed by any and all other methods the principal
developer(s) see fit.  The principal developer(s) MAY promote their projects
on their own, but SHOULD do so in consultation with the T2O2, to both ensure
that all promotions are professional in nature and minimize any duplication of
effort.

If the principal developer(s) choose to use GitHub as a distribution method
for their software, then the principal developer(s) are responsible for
generating a digital object identifier (DOI) for the release.  The
instructions to do so are at
https://guides.github.com/activities/citable-code/.
It is RECOMMENDED that all releases have a DOI associated with them to
facilitate citations of the software.

## <a name="4ADBEADCC17C11E6B9BC003EE1B763F8"></a>Minor Reviews

Minor reviews are for the publication of any material that the principal
developer(s), their OPSEC officer(s), and their supervisor(s) do not believe
require a major review.  These include bug fixes and minor updates.  A level-1
OPSEC officer must review the material before it is published.  These reviews
are called "minor reviews" and are subject to the following:

* The OPSEC officer MAY also be the technical reviewer for the release.
* Only if the project as a whole, including the minor changes being proposed
  for release, receives an "Approved for public release; distribution
  unlimited" statement can the changes be released.

The process for a minor release is as follows:

* The person who created the material sends it to the OPSEC reviewer.
* The OPSEC reviewer reviews the material and sends a digitally signed email
  back to the creator stating whether or not it may be released.
* If the material may be released, then the creator pushes the material out to
  the public.

Note that there are numerous methods of sending the material.  If the material
is stored under git, and both the creator and the OPSEC officer have access to
the same private repository<sup>[4](#Footnote_4)</sup>, then the creator MAY
choose to push to the private repository and ask the OPSEC officer to pull it
and review the changes.  Alternatively, git bundles MAY be used, or one could
even email text files.  Regardless of the method chosen, there are two
requirements that MUST be met:

* The chosen method MUST uniquely identify the set of changes under
  discussion.  Examples include the complete git commit hash under discussion,
  emails with the complete change set, or any cryptographically signed
  method.  This ensures non-repudiation or confusion.
* The OPSEC reviewer MUST track what he or she has approved.  This MAY be done
  by saving the digitally signed emails that were sent.

These steps are REQUIRED for audit purposes.  Without them, ARL cannot prove
to the Department of the Army that it is properly reviewing material before it
is released.

If the principal developer(s), the OPSEC officer, or any of their superiors
determine that significant changes to the scope of the project or violation of
any of the checks described in this document have occurred or are about to
occur, then a Major Review must be performed instead of a Minor Review.

## <a name="4D5F4B34C17C11E6ADBB003EE1B763F8"></a>Incorporating External Contributions

Once the software has passed the process outlined above and has been publicly
distributed, any contributions to the project MUST be subject to its license.

External contributions do not need to undergo OPSEC review as they are assumed
to be public at the time of contribution.  They SHOULD be reviewed for quality
purposes before being accepted into a project to ensure that they are
professional in nature and perform as expected.  All external contributors
MUST have a CLA (see [ARL CLA](#2DF49A4AC17C11E69E3A003EE1B763F8)) on file
before their contributions are accepted into the project.  A CLA only needs to
be executed once by each legal entity for a given project.  Project owners
MUST turn over executed CLAs to the T2O2 for record keeping.  Project owners
MUST explain in the README file that external contributors MUST execute a CLA
before their contributions will be accepted.

## <a name="A_Note_on_Impact_and_Metrics"></a>A Note on Impact and Metrics

Publishing software as a regular business practice is new territory for ARL,
and how to measure a project's impact is still a matter for debate.  While
GitHub gathers numerous statistics on projects, from the number of downloads,
to the number of followers, etc., these are, at best, suggestions of what a
project's true impact is.  For the sake of metrics, a project's principal
developer(s) MUST describe what impact their project has had since the last
[Major Review](#3449D4BEC17C11E68DD1003EE1B763F8) when they submit their next
Major Review.  The report MUST describe what the principal developer(s) think
the impact of project is, and provide evidence to back up any claims.  The
greater impact a project has had, the better it is for metrics and performance
evaluation.  Brief examples of how this can be done are shown in
[sample_abstract2.md](sample_abstract2.md) and
[sample_abstract3.md](sample_abstract3.md), and further instructions are
provided in the [Major Review](#3449D4BEC17C11E68DD1003EE1B763F8) section.

To be absolutely clear, impact is based on major reviews (releases that follow
the procedure outlined in [Major Reviews](#3449D4BEC17C11E68DD1003EE1B763F8)).
[Minor Reviews](#4ADBEADCC17C11E6B9BC003EE1B763F8) might lead toward a major
review, but will not count toward a principal developer(s) performance
metrics. If the principal developer(s) want releases to count toward their
metrics, the procedures outlined in Major Reviews MUST be followed.

For performance metric purposes, supervisors MAY treat a major review as being
up to the equivalent of a major accomplishment for the year, similar to the
publication of a paper in a high-impact peer-reviewed journal.  To obtain
recognition, principal developer(s) MUST provide evidence of impact as
explained in [Evidence of Impact](#5092761CC17C11E6B23A003EE1B763F8) and
[Software Maturity and Software Engineering](#53A23266C17C11E6BEEE003EE1B763F8).
The greater impact the software has had since the last major review, the more
credit MAY be given (up to the equivalent of a major accomplishment).  If a
given major review has had no impact, then it MUST NOT be given any credit for
performance metric purposes.

### <a name="5092761CC17C11E6B23A003EE1B763F8"></a>Evidence of Impact

It is up to the principal developer(s) to decide what types of evidence to use
when describing the impact of a project.  As noted in
[File an ARL Form 1](#4066B47EC17C11E6BFC7003EE1B763F8), ARL will not "double
count" the impact; ARL is primarily interested in the impact since the last
major review.  That said, some forms of evidence are difficult to express as a
difference from a prior major review.  In that case, the principal
developer(s) MAY wish to express both the current absolute numbers and the
changes since the project was last filed.

Below are some examples of evidence principal developer(s) MAY wish to
consider giving:

* The number of citations of different releases.  It is possible to cite
  releases on GitHub just as papers might be cited.  See
  https://guides.github.com/activities/citable-code/ for more information on
  how to do this.
* If a project is a library or something else that is intended to be
  incorporated into other projects, list those projects and describe their
  importance.
* Customers that are using the software, provided they permit their names to
  be listed.
* The number of followers, including the level of interest as measured by
  issues opened and persons contacting the principal developer(s).
* The number of forks.
* The number of contributions from outside (non-ARL) sources.
* Letters of acknowledgment, thanks, or other forms of recognition.
* Software maturity.

The principal developer(s) should not feel that they are limited to these
pieces of evidence, nor should they feel the need to include evidence from all
of these categories.  ARL is still learning which metrics to use when
determining the impact of a project. The principal developer(s) should feel
free to use any metric they wish, but should note that supervisors and others
will make the final decision on how heavily to weight the chosen metrics.  For
example, the number of citations for a software project is more important than
the number of downloads it has. If a project is a library, then the number and
importance of projects using the library will have greater weight than the
number of people that have forked the project<sup>[5](#Footnote_5)</sup>.

In general, supervisors will want to know how a project has made a difference
in the world and how important that difference has been since its last major
review.  The better evidence provided, the easier this becomes.

### <a name="53A23266C17C11E6BEEE003EE1B763F8"></a>Software Maturity and Software Engineering

ARL would like to be a world leader in computer science research.  To be a
world leader means that ARL must have an impact, and to have an impact means
that ARL's software must be used.  Poorly written software that is
incomprehensible or difficult to compile or use will not be used, and will
have little, if any, impact.  Thus, if the primary improvement to a project
involves bringing it in line with generally accepted best practices in
software engineering to facilitate its transition to others, then this is also
of value and MUST be credited.  Examples of this include, but are not limited
to, the following:

* Providing a well-designed, thoroughly documented application programming
  interface (API) or other interface.
* Adding tests (unit tests, regression tests, integration tests, etc.) that
  increase confidence that your software is performing correctly.
* Increasing code coverage of tests.
* Adding examples and high-level documentation.  This includes ensuring that
  all examples and documentation are up to date with the current software.
* Simplifying building and installation of software.

These are just some examples of mature software.  If there is other evidence
of the maturity or quality of software, principal developer(s) should feel
free to use it when describing the impact of the software.  Supervisors MUST
consider improvements in software engineering when considering the impact of
software, but just as with any other claims of impact, supervisors will have
the final say in determining how important the impact actually is as it
relates to performance metrics.

# <a name="D3DC705AC3C411E6BBB4003EE1B763F8"></a>Contributor License Agreement (CLA)

The ARL Contributor License Agreement (ARL Form 266) can be found
[here](ARL%20Form%20-%20266.pdf)<sup>[6](#Footnote_6)</sup>. Each external
contributor must execute and return a copy for each project that he or she
intends to contribute to.  Once ARL receives the executed form, it will remain
in force permanently.  Thus, external contributors need only execute the form
once for each project that they plan on contributing to.

# <a name="93338EDCC17C11E6B720003EE1B763F8"></a>Footnotes

<sup><a name="Footnote_1">1</a></sup> Some licenses have guidelines that
differ from the ones described here.  For example, the GPL states that the
filename must be COPYING.  This is why your README MUST specify which file
contains the license.

<sup><a name="Footnote_2">2</a></sup> If you have questions about what are
"software-related inventions", consult with ARL Legal.

<sup><a name="Footnote_3">3</a></sup> Excluding works generated by Government
employees in the course of their duties.

<sup><a name="Footnote_4">4</a></sup> A private repository is only accessible
from within ARL; it MUST NOT be publicly accessible!

<sup><a name="Footnote_5">5</a></sup> As an example, if a library is only
used within the Linux kernel, it will have been used by very few projects, but
will have an extraordinary impact.

<sup><a name="Footnote_6">6</a></sup> This form may not preview correctly in
your browser.  If you have trouble opening the file, or if the file has a
phrase similar to "Please wait... If this message is not eventually replaced
by...", then try downloading the form and opening it in the latest version of
Adobe® Acrobat Reader.  ARL is aware of the issue, and is working to correct
the problem.