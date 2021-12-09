# OGC API Building Blocks

Experimental repository for building blocks from the [OGC API standards](https://ogcapi.ogc.org).

* `geo` - geospatial building blocks
  * `common` - building blocks applicable to multiple geospatial resource types
    * `data types` - JSON representations of geospatial concepts
      * [OGC Collections](geo/common/json-collections.adoc)
      * [OGC Collection](geo/common/json-collection.adoc)
      * [Extent](geo/common/json-extent.adoc)
      * [Bounding Box](geo/common/json-bbox.adoc)
    * `parameters` - HTTP query parameters
      * [bbox-crs](geo/common/parameter-bbox-crs.adoc)
      * [bbox](geo/common/parameter-bbox.adoc)
      * [crs](geo/common/parameter-crs.adoc)
    * `headers` - HTTP headers
      * [Content-Crs](geo/common/header-content-crs.adoc)
  * `features`- building blocks applicable to feature resources
    * `resources` - API resources
      * [Features](geo/features/json-features.adoc)
      * [Feature](geo/features/json-feature.adoc)
* `ogc-utils` - Utility building blocks that are used in OGC API's but are not inherently geospatial. They were created to ensure 
consistency within OGC API's where there was not a clear mainstream standard.  They aim to be in line with best practices of the 
web and could be replaced, e.g. by building blocks specified in an IETF RFC or similar, if and when they are available. API's 
built with the geo building blocks do not need to use these, but they provide a nice default option that OGC-focused tools will 
understand.
  * `data types` - JSON representations of various utilities used in OGC API's
    * [OGC API Landing Page](ogc-utils/json-landing-page.adoc)
    * [OGC Conformance Declaration](ogc-utils/json-conformance-declaration.adoc)
    * [Instant](ogc-utils/json-instant.adoc)
    * [Interval](ogc-utils/json-interval.adoc)
    * [Link](ogc-utils/json-link.adoc)
  * `parameters` - HTTP query parameters
    * [datetime](ogc-utils/parameter-datetime.adoc)
    * [limit](ogc-utils/parameter-limit.adoc)
* `unstable` - These building blocks are not yet stable or mature. They may be extracted from core OGC API standards that have not 
yet been fully approved, or they may also be new ideas that are not yet in a standard.
  * `data types` - JSON representations of geospatial concepts or utilities that are not yet stable or mature.
    * [Dataset Collection](unstable/json-dataset-collection.adoc)

Currently only building blocks from [Part 1: Core](https://docs.ogc.org/DRAFTS/17-069r4.html) and [Part 2: Coordinate Reference Systems by Reference](https://docs.ogc.org/DRAFTS/18-058r1.html) of OGC API Features are included.

**Warning:** This is a work-in-progress.

## Building Block Maturity 

This repository is started with a set of completely mature building blocks that are extracted from the stable 
[OGC API - Features](https://ogcapi.ogc.org/features/) specification. But it includes a set of less stable building
blocks as well, to show what's coming next and to enable more participation in the shaping of the next blocks. All
building blocks in this repo must include a maturity classification, so that users can easily get a sense of how
much they can count on the extension. 


| Maturity Classification |  Min Impl # | Description | Stability |
| ----------------------- | ----------- | ----------- | --------- |
| Mature                  | 10           | Included in a standard that has been released for at least 1 year and has at least 10 diverse implementations. | Most stable, can rely on it completely. |
| Stable                  | 3           | Defined and used in one or more released standards.| Approaching stability - breaking changes are not anticipated but can easily come from additional feedback |
| Candidate               | 1           | Part of a standard that is close to approval, either as a section or a new 'part' | Mostly stable, breaking changes are unlikely, but possible. |
| Proposal                | 0          | A new idea. Ideally it should be linked at least a pull request against one of the OGC API repositories as a 'proposal' or new section | Not stable - breaking changes almost guaranteed as implementers try out the idea. |
| Deprecated              | N/A         | A previous extension that has likely been superseded by a newer one or did not work out for some reason. | DO NOT USE, is not supported |

Every building block in this repo will have a maturity field with one of the above classifications. If it is a stable or
mature block then it must include a reference field, with a link to the section of the released standard that specifies it. 
For less mature building blocks the reference can link to a standard in progress, a proposal on an existing standard, or 
a pull request. For the least mature levels a reference link is not required, but it is recommended to try to at least
get to a PR in the appropriate OGC API repository as soon as feasible.

Maturity mostly comes through the core building block definition going through the process of becoming a fully adopted
OGC standard, and should increase in diverse implementations during that process. But building block authors can also
choose to hold back the maturity advancement if they don't feel they anticipate that changes may be coming.

