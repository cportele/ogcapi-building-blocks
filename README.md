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
* `ogc-utilities` - building blocks that are used in OGC API's but are not inherently geospatial. They were created to ensure consistency within OGC API's where there was not a clear mainstream standard.  They aim to be in line with best practices of the web and could be replaced, e.g. by building blocks specified in an IETF RFC or similar, if and when they are available. API's built with the geo building blocks do not need to use these, but they provide a nice default option that OGC-focused tools will understand.
  * `data types` - JSON representations of various utilities used in OGC API's
    * [OGC API Landing Page](ogc-utilities/json-landing-page.adoc)
    * [OGC Conformance Declaration](ogc-utilities/json-conformance-declaration.adoc)
    * [Instant](ogc-utilities/json-instant.adoc)
    * [Interval](ogc-utilities/json-interval.adoc)
    * [Link](ogc-utilities/json-link.adoc)
  * `parameters` - HTTP query parameters
    * [datetime](ogc-utilities/parameters/datetime.adoc)
    * [limit](ogc-utilities/parameters/limit.adoc)

Currently only building blocks from [Part 1: Core](http://docs.ogc.org/DRAFTS/17-069r4.html) and [Part 2: Coordinate Reference Systems by Reference](https://docs.ogc.org/DRAFTS/18-058r1.html) of OGC API Features are included.

This is a work-in-progress.
