
# Resource Template: Aggregate Base

This is a template "base" file to use as a starting point for a new aggregate resource for the Better Scientific Software site.  The comments section of this file includes guidelines on naming conventions and metadata, as provided in the [BSSW Style Guide](../StyleGuide.md).  

Provide introductory text for the topic in this file and then information on various subtopics in separate "subresource" files (possibly contributed by different authors). Use the following format to specify subresources, listed in the order to be shown on front-end BSSW site:

**Subresources:**
- [Name of Subresource1](SubresourceFile1.md)
- [Name of Subresource2](SubresourceFile2.md)
- etc.

The front-end for the BSSW site will then combine the information into an aggregate resource.  Use the following metadata to describe the aggregate resource components:

This file ("base"):  
- Aggregate: base
   - The "base" designation indicates that content and metadata will be included from subresource files, as specified in the bulletted list of subresources.

Subtopic resource files:
- Aggregate: subresource
  - The "subresource" specification indicates that the item will not be displayed as a separate resource on the front-end BSSW site.  We expect this to be the most common usage.  

- Aggregate: stand-alone and subresource
   - The "stand-alone and subresource" specification indicates that the item will be both (1) listed as a separate resource on the front-end site and (2) used as a subresource, as specified by an aggregate "base" resource.

**To add a new resource using this file as a starting point:**
- View this file in Raw mode.
- Copy all text.
- Select `Create New File`.
- Paste text into your new document, as a starting point. Then edit as you like.
- Continue following instructions in [How To Contribute](../HowToContribute.md).

See also [ResourceTemplate.AggregateSubresource](ResourceTemplate.AggregateSubresource.md).

A template for a new resource that can be handled effectively in a single file, rather than as an aggregate, is:
[ResourceTemplate.Basic](ResourceTemplate.Basic.md).

For more information on better scientific software, go to the [Better Scientific Software main page](http://betterscientificsoftware.info).

<!---
Publish: Publish on the BSSw front-end site?
Categories: specify 1 or more categories
Topics: specify 1 or more topics (corresponding to each category)
Tags: specify optional tags
Level: specify level of content
Prerequisites: specify prerequisites
Aggregate: base
--->

<!---
Please follow these guidelines for naming resources and files. Be sure to include metadata with each entry, as this will be used to organize content, provide filters, and support searches on the BSSW site.

Resource Name:

    Brief, essential words only, nothing extra
    For curated content: Follow name of content (e.g., title of book, article, event, site)
    Filename: Same as resource name
        No spaces
        Cap for first letter of each word
        Abbreviations:
            Apps = Applications
            Cse = CSE = Computational Science and Engineering
            Devpt = Development
            Eng = Engineering
            Hpc = HPC = High-Performance Computing
            Perf = Performance
            Sw = Software

Resource Description:

    Concise paragraph explaining resource from the perspective of the CSE community
    Use links to WhatIs and HowTo docs when appropriate for background info
    Image file (e.g., logo) - optional (encouraged when this exists)

Contributor:

    Name(s) of contributor(s), hyperlinked to GitHub profile(s)

Footer: Add the following at the bottom of each page:

For more information on better scientific software, go to the [Better Scientific Software main page](http://betterscientificsoftware.info).

Metadata: Include metadata as formatted comments at the end of the file

    Publish: Publish on the BSSw front-end site?
    Categories: Specify 1 or more categories (primary display via BSSW website)
    Topics: Specify 1 or more topics (visible filters via BSSW website)
    Tags: Specify additional tags as keywords for searches (optional)
    Level: Specify level of content
    Prerequisites: Specify any assumed knowledge on the BSSW site (usually Level 0 and Level 1 BSSW docs)
    Aggregate: Optional info for aggregating content to define a more complex resource

Each aspect of metadata is described below.

Publish: Publish on the BSSw front-end site?
Publish: Yes
Publish: No

Only files designated as 'Publish: Yes' will be published on the front-end BSSw site. Work that has not been finalized or is not intended for the front-end site should be designated 'Publish: No'

Categories: [Primary display via BSSW website interface]

[BSSW curators may add/revise categories as needed over time.]

- Planning
- Development
- Performance
- Reliability
- Collaboration
- Skills

#### Topics: Visible filters via BSSw website interface
- All categories and also finer grain topics within categories
 [Topics: 4-7 per category: family of topics that make sense together. BSSw curators may add/revise topics as needed over time.]

- **Planning**
   - Improving productivity and sustainability
   - Requirements
   - Design
   - Software interoperability
- **Development**
   - Documentation
   - Version control
   - Configuration and builds
   - Deployment
   - Issue tracking
   - Refactoring
   - Software engineering
   - Development tools

- **Performance**
   - High-performance computing (HPC)
   - Performance at leadership computing facilities (LCFs)
   - Performance portability
- **Reliability**
   - Testing
   - Continuous integration testing
   - Reproducibility
   - Debugging
- **Collaboration**
   - Licensing
   - Strategies for more effective teams
   - Funding sources and programs
   - Projects and organizations
   - Software publishing and citation
   - Discussion forums, Q&A sites
- **Skills**
   - Personal productivity and sustainability
   - Online learning

Tags: [optional additional keywords for searches]

    Add/revise topics as needed (important terms from curated content; aim for comprehensive coverage to facilitate searches)
    ATPESC
    Bitbucket
    Computational Science Stack Exchange
    Conference
    Doxygen
    FORCE11
    Git
    Gitlab
    HPC
    Jenkins
    Minisymposium
    SoftwareX
    Software Carpentry
    Software Sustainability Institute
    Strategy
    Team
    Test-driven development
    Travis CI
    TutorialsPoint
    Udacity
    Workshop
    etc.

Levels: Specify level of detail and depth of content

    Level 0: BSSW WhatIs document
    Level 1: BSSW HowTo document (or equivalent level of detail)
    Level 2: More detailed content, beginner or intermediate levels
    Level 3: Advanced content

Prerequisites: Specify files for any assumed knowledge on the BSSW site (usually Level 0 and Level1 BSSW docs)

    prerequisites: filename1.md, filename2.md, etc.

Aggregate:

   Aggregate: base
   - The "base" designation indicates that content and metadata will be included from specified subresource files.  

  Aggregate: subresource
   - The "subresource" designation indicates that the item will not be displayed as a separate resource on the front-end BSSW site.  We expect this to be the most common usage.  However, omitting this subresource metadata will enable the item to be both (1) listed as a separate resource on the front-end site and (2) used as a subresource, as specified by an aggregate "base" resource.

--->
