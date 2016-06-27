# 3D-Visualization-Demos

Learn how to visualize data in 3D with the ArcGIS 4.0 API for JavaScript. In this session we’ll overview various points to consider when thinking about 3D visualization, including when it is appropriate to use 3D symbols and 2D symbols. Create single variable and multivariate visualizations in just a few lines of code. Understand the variety of visualization opportunities in 3D, while acknowledging some of the pitfalls. Become familiar with some of the up and coming features related to 3D visualization.

## Topics to cover/Outline

* Visualization intro  
  * 2D viz and 3D viz are similar in many respects
    * Handled with the same renderers
    * principles of color, generalization,
  * 3D differences/considerations
    * Icon placement
      * Draped vs billboarded
      * Quick sample showing both
    * Size can be rendered in flat (2D space) or take advantage of the z-axis as a volume/extrusion
      * Images (from SDK)
    * Colors are shaded differently depending on
      * camera angle
      * environment settings
      * Images (from SDK)
    * Opacity doesn't work well (yet)
      * Not able to see through transparent objects from certain angles
      * Images (modified sample from SDK)
    * Rotation - not supported (yet)
      * Hard to determine in screen space where north is in a 3D view
      * Image (from SDK)
  * Use cases
    * Location
      * Sample: Mt Baldy POI
      * Sample: NYC SceneLayer
    * Types
      * Visualization depends on unique (usually string) values
        * high, medium, low
        * residential, commercial, mixed
        * freeway, highway, arterial, residential street
      * Sample: building types
      * Sample: road/highway types
      * Sample: tree species
    * Thematic counts and amounts
      * Visualization depends on numeric values
      * Data driven color
        * Sample: poverty
      * Data driven size
        * Sample: poverty (flat)
        * Sample: poverty (extrusion)
          * Using color for same field is a good idea
      * Data driven opacity
      * Muliple variables
        * Can create cool visualizations
        * Sample: marriage stats/census data
        * Use caution
        * Sample: politics/poverty
    * Real world sizes
      * Create an object similar to
      * Sample: trees/carbon storage
      * Sample: buildings
  * Renderers
    * Define which symbols apply to which features
    * SimpleRenderer
    * UniqueValueRenderer
    * ClassBreaksRenderer
    * Visual variables
      * Defines color, size, and opacity values based on data
  * Symbols
    * Most symbol types are supported in 3D
    * 2D symbols (images + code)
      * Points
        * SimpleMarkerSymbol
        * PictureMarkerSymbol
      * Lines
        * SimpleLineSymbol
      * Polygons
        * SimpleFillSymbol
        * ~~PictureFillSymbol~~
    * 3D symbols (recommended) (images + code)
      * flat vs. volumetric
      * 5 types
        * PointSymbol3D
        * LineSymbol3D
        * PolygonSymbol3D
        * MeshSymbol3D
        * LabelSymbol3D
      * Symbol layers
      * 2D vs 3D comparison
  * Visualization wrap up
    * This requires that you know your data
    * Future Smart Mapping support in 3D
      * Show slider sample?
* Conclusion
  * Where to go for advanced WebGL cases
  * Helpful resources
    * Quick overview of documentation
    * Samples/tutorials in SDK
    * 3D blog series
    * Other repos

## Resources

* [Community](https://developers.arcgis.com/en/javascript/jshelp/community.html)
* [ArcGIS for JavaScript API Resource Center](http://help.arcgis.com/en/webapi/javascript/arcgis/index.html)
* [ArcGIS Blog](http://blogs.esri.com/esri/arcgis/)
* [twitter@esri](http://twitter.com/esri)

## Issues

Find a bug or want to request a new feature?  Please let us know by submitting an issue.

## Contributing

Esri welcomes contributions from anyone and everyone. Please see our [guidelines for contributing](https://github.com/esri/contributing).

## Licensing
Copyright 2016 Esri

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

A copy of the license is available in the repository's [license.txt](https://github.com/ArcGIS/3D-Visualization-Demos/blob/master/license.txt) file.

[](Esri Tags: Esri 3D Visualization Esri JavaScript 4.0)
[](Esri Language: JavaScript)
