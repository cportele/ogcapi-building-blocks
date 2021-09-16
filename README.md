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
* `other` - building blocks that are not inherently geospatial and could be replaced, e.g. by building blocks specified in an IETF RFC or similar, once available
  * `common` - building blocks applicable to multiple geospatial resource types
    * `resources` - API resources
      * [OGC API Landing Page](other/common/resources/landing-page.adoc)
      * [OGC Conformance Declaration](other/common/resources/conformance-declaration.adoc)
    * `parameters` - HTTP query parameters
      * [datetime](other/common/parameters/datetime.adoc)
      * [limit](other/common/parameters/limit.adoc)
    * `schemas` - Reusable data types
      * [Instant](other/common/schemas/instant.adoc)
      * [Interval](other/common/schemas/interval.adoc)
      * [Link](other/common/schemas/link.adoc)

Currently only building blocks from [Part 1: Core](http://docs.ogc.org/DRAFTS/17-069r4.html) and [Part 2: Coordinate Reference Systems by Reference](https://docs.ogc.org/DRAFTS/18-058r1.html) of OGC API Features are included.

This is a work-in-progress.
