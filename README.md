# uc-2016-4x-3D-Visualization

Learn how to visualize data in 3D with the ArcGIS 4.0 API for JavaScript. In this session we’ll overview various points to consider when thinking about 3D visualization, including when it is appropriate to use 3D symbols and 2D symbols. Create single variable and multivariate visualizations in just a few lines of code. Understand the variety of visualization opportunities in 3D, while acknowledging some of the pitfalls. Become familiar with some of the up and coming features related to 3D visualization.

## Topics to cover/Outline

* Intro (10 min) (Kelly)
  * Demo 3d app (something cool)
  * Browser support
  * Quickly build demo app
    * Create map, view
    * Add layer to map (also maybe demo web scene)
    * Local vs global (default is global)
    * Explain camera
    * Ground elevation
* Visualization intro  (Kristian)
  * 2D viz and 3D viz are similar in many respects
  * 3D considerations
    * Icon placement
      * Draped vs billboarded
    * Size can be rendered in flat (2D space) or take advantage of the z-axis as a volume/extrusion
    * Colors are shaded differently depending on
      * camera angle
      * environment settings
    * Opacity doesn't work well (yet)
      * Not able to see through transparent objects from certain angles
    * Rotation - not supported (yet)
      * Hard to determine in screen space where north is in a 3D view
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
    * All symbol types are supported in 3D
    * 2D symbols
      * Points
        * SimpleMarkerSymbol
        * PictureMarkerSymbol
      * Lines
        * SimpleLineSymbol
      * Polygons
        * SimpleFillSymbol
        * PictureFillSymbol
    * 3D symbols (recommended)
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
* Web Scenes  (Kelly)
  * Less code (offload dev tasks)
  * Use id in your app
  * Limitations (currently)
* Conclusion
  * Where to go for advanced WebGL cases
  * Helpful resources
    * Quick overview of documentation
    * Samples/tutorials in SDK
    * 3D blog series
    * Other repos


