---
id: 482
title: Data inputs and editing
date: 2016-01-26T12:05:41+00:00
author: lassegs
layout: post
guid: http://skole.lassegs.org/?p=482
permalink: /2016/01/26/data-inputs-and-editing/
categories:
  - SGO4940
---
<div>
  <em>Andreas Forø Tollefsen,</em>
</div>

<div>
</div>

<div>
  <strong>Slides from last lecture:</strong>
</div>

<div>
</div>

<div>
  Represent elevation: Elevation as contour lines. ISOlines, equidistance is the distance from one line to next.
</div>

<div>
                                         Elevation as polygons. Also generalizing, classifying heights into groups.
</div>

<div>
                                         Elevation as raster. Continous data scale. Gives better approximation of the heights between classes.
</div>

<div>
                                         Elevation as TIN: Triangulated Irregular Netwrk. Direction and ascpect is non varying within triangles.
</div>

<div>
</div>

<div>
  Raster &#8211; 3D models- Continious data. Representing frequency as elevation. Useful for some purposes.
</div>

<div>
</div>

### Generalization of reality

<div>
  We always have generalizations of the real world. We cannot make perfect models of something as complex. So we make generalizations, we ignore differences and set borders
</div>

<div>
</div>

### Think about similarities

<div>
  Similarities in locations and similarities in attributes. Spatial autocorrelation is more complex than
</div>

<div>
  Positive Serial Correlation. Similarities in time, all the data points are dependent on the previous point in time. The values and the timing of the point follows each other. This is prevalent.
</div>

<div>
  Negative Serial Correlation is not very common.
</div>

<div>
</div>

<div>
  Spatial autocorrelation is similarities across space. Many directions simultaneously. Recap Tobler&#8217;s first law of geography!
</div>

<div>
  <em>&laquo;Everything is related to everything else, but near things are more related than distant things.&raquo; </em>Tobler.
</div>

<div>
</div>

<div>
  Spatial heterogeneity: Locations are different
</div>

<div>
  Spatial homogeneity: Locations are similar
</div>

<div>
  Similarity where? DIstance and scope affects similarity.
</div>

<div>
</div>

### Smoothness / irregularity

### Spatial autocorrelation

<div>
  Similar to Toblers first law: Positive spatial autocorrelation: Similitarity in both position and attributes.
</div>

<div>
  Opposite to Tobler&#8217;s first law: Negative spatial autocorrelation. Similarity in position, but not in attributes.
</div>

<div>
  Zero autocorrelation when position and attributes are completely independent. No pattern, random.
</div>

<div>
</div>

<div>
  The most used way to measure this is Morans I. A measure of the spatial autocorrelation from -1 to +1. 0 is random, no pattern.
</div>

<div>
  -1 is perfect negative spatial autocorrelation. We cannot reach perfect positive autocorrelation.
</div>

### Morans I

<div>
  Both vector and raster data. The most used indicator for spatial autocorrelation.
</div>

<div>
</div>

### Dissimilarity

<div>
  Is likely to occur when competition between regions or actors outweigh cooperative factors.
</div>

### Sampling methods

<div>
  Random selection &#8211; most used. Throw out points in an area.
</div>

<div>
  Stratified selection &#8211; make a grid, do selections in the intersections
</div>

<div>
  Stratified random selection &#8211;
</div>

<div>
  Stratified selection with random grid variations &#8211; random grid size, measuer in intersections
</div>

<div>
  Cluster selections &#8211;
</div>

<div>
  Cross sectional selection
</div>

<div>
  Contour line selection
</div>

<div>
</div>

### Spatial data input and editing

<div>
  Geo-referencing. What should we attach data to? Coordinate systems. Lengths and latitude. Datum. Projections. Primary and secondary data sources.
</div>

<div>
</div>

<div>
  Goodchild 2011 three meanings of scale. Representative fraction. Exxtent in space. Resolution.
</div>

<div>
  Bott and Young. The role of crowd-sourcing. Open-source data and information. Increase collective knowledge, community building, collective creativity and innovation, crowdfunding, civic engagement. Crowdsourcing GIS and community knowledge important, like environmental management, crisis management, post-conflict. More on this in the Qualitative GIS lecture.
</div>

<div>
</div>

### Geo-referencing

<div>
  Several terms are used interchangeably: mapping, tagging, geo-coding. Geo-referncing in this regard: link an object or attribute to a location (possibly also to some point), placing the object or attribute geographically.
</div>

### What should we attach data to?

<div>
  The main requirement for localization is that the geographical reference is
</div>

  *     &#8211; Unique, so taht there is only one location which corresponds to the reference.
  * The existence of a common understanding to contents of the refrence ssytem that is shared.
  * A stable reference system.

<div>
  In our use of GIS we link data either <strong>explicitly</strong> to the coordinates (latitude and longitude, X and Y) or <strong> implisityly </strong>assumed for the references we use, such as place, administrative zones, regions, addresses.
</div>

<div>
</div>

<div>
  Take into account double phenomena (cities called Springfield), addresses and change of names.
</div>

<div>
  Residential adresses is a good way to locate housing and economic activity in cities and towns, but does not work so well in rural areas.
</div>

<div>
</div>

### Geographic coordinate systems

<div>
  The safest way to localize. Only one unique coordinate for each location. Persistent through time. Common understanding fo the system.
</div>

<div>
  Latitude (paralell with equator] Based on the equator ( a sectional earth perpendicular to the rotation axis and the mass mean point. Ranges from 90 degress south to 90 degrees north.
</div>

<div>
  Longitude. Based on the 0 meridian through Greenwich observatory. Ranges from 0 &#8211; 180 east and 0 &#8211; 180 west.
</div>

<div>
</div>

<div>
  We typically convert coordinates to desmal degrees. Decimal degrees = (degrees + Minutes / 60) + (Seconds / 3600).
</div>

<div>
</div>

<div>
  Earth is not a perfect sphere.
</div>

<div>
  Global Datum WGS84 is the best fit globally.
</div>

<div>
  Local Datum (best fit for local area of interest).
</div>

<div>
</div>

<div>
  We need datum to establish reference systems on the earths surface. Euref89 is Norwegian.
</div>

<div>
  We are projecting coordinates of the ellipsoid on to flat maps. Different projections take different characteristics.
</div>

<div>
  Equal area: Area correct
</div>

<div>
  Conform: The shape of areas corret
</div>

<div>
  Equidistant: Measurd distance correct.
</div>

<div>
  Retroazimuthal: Measured directions are correct.
</div>

<div>
  Compromise: No specific properties are correct. Minimize all errors.
</div>

<div>
</div>

### Common projections

<div>
  Planar: We imagine taht we put a flat sheet to the world. The representation is appropriate touch point. This is often used on the map of the polar regions.
</div>

<div>
  Cylinder projection: Stretch a sheet around the globe. the representation is correct along the touch line.
</div>

<div>
  Conic projection: Will most correct along a latitude between the equator and the pole, depending on the cone shape.
</div>

<div>
  Projections may be either tangent (the sheet touches the globe) or Secant (the sheet cuts through the globe, so we get two touch lines).
</div>

<div>
</div>

### Plate Caree (cylindrical equidistant projection):

<div>
  The simplest form of projection: latitude as the x-coordinates and longitude as y-coordinates. Distances are right on the equator and along the meridians, but not otherwise.
</div>

<div>
  The cartesian coordinate system.
</div>

<div>
  Universal Transverse Mercator (UTM) projection, map wrappped around the globe, but over the transverse. UTM parts globe in 60 different zones, each 6 degrees wide.
</div>

<div>
  Norway is covered byt the UTM zone 31N &#8211; 36N, but it is common to use zone 33N throughout Norway. UTM is all in meters, good for measuring distances.
</div>

### Why is this important?

<div>
  Because if we read into different layers with different datum, geographic coordinate systems and projections, we cannot match the layers to each other and we will not be able to analyze various data layers against each other.
</div>

<div>
</div>

<div>
  We can show degrees of error in maps with Tissot matrix.
</div>

<div>
</div>

### Data models in GIS

<div>
  Representation and data model are overlapping concepts.
</div>

  * Representation is more conceptual and scientific
  * Data models used moer in practice and in database and project design

<div>
  How the geographical reality is modeled in a GIS?
</div>

<div>
</div>

<div>
  A data model is a set of constructs for describing and representing part of the real world in a computer.
</div>

<div>
</div>

<div>
  A data model defines the data structure and determines how data is stored and therefore consequently affect the types of analysis taht can be performed. It is a simplified description of reality.
</div>

<div>
</div>

<div>
  We go from the real world. We make the data model, describe and represent. Operational analysis and presentation. People .
</div>

### Levels of generalization or simplification.

<div>
  Conceptual model: reality -> Conceptual -> logical model &#8211; physical model.
</div>

<div>
  Reality includes everything. Comprised of real phenomena. Buildings, roads, wells, lakes, people, etc. Need to simplify. We have to generalize reality into a manageable form.
</div>

<div>
  Abstraction level &#8211; conceptual. Human oriented. Partly structured model with selected objects and processes. Which objets and processes are relevant for our purpose+
</div>

<div>
  Logical model  implementation oriented.
</div>

<div>
  Physical model. The actual implementation in GIS. Tables stored as files or databases. Digital terms.
</div>

<div>
</div>

<div>
  Computer models as common framework. Important that everyone has a common understanding of the project.
</div>

<div>
  From system design to system. Describes project in-depth. Document how you gather data, from systems design to the system itself.
</div>

<div>
</div>

<div>
  In ArcGIS we have the model builder. It takes input, shows tools we need to get a certain output.
</div>

<div>
  GIS data model types are based on continuous fields and discrete objects. GIS data models are based on layers.
</div>

<div>
</div>

<div>
  Raster data model consists of strict matrix of cells or pixels to represent real objects. One value per pixel. Can be compressed. Satellite Images can have multiple raster bands. hus one color value per band can be assigned.  For example, saturation values of respectively red, green and blue can be combined to visualize teh sattelite data. We cannot add variables to the pixels.
</div>

<div>
  A raster often contain header / metadata.
</div>

<div>
  The coordinates of starting corner.
</div>

<div>
  Pixel size (cell size)
</div>

<div>
  Number of rows and columsn.
</div>

<div>
  The projection.
</div>

<div>
  No-data value.
</div>

<div>
</div>

### Vector model

<div>
  Simple features. point line or polygon
</div>

<div>
  Topological features. The science and mathematics in vector data. This information can be used for network analysis to test the validity of a polygon adjacency or other topological errors. Network connectivity.
</div>

<div>
</div>

<div>
  Data collection:
</div>

<div>
  Planning &#8211; preperation &#8211; digitizing, transfering &#8211; editing, improving &#8211; evaluation. And go again.
</div>

<div>
</div>

### Collecting data

<div>
  Primary data sources: Collected in digital format for a particular GIS project.
</div>

<div>
  Two broad categories of data sources:
</div>

  * Data collection (direct collection): Primary sources. Secondary sources.
  * Data transfer (exchange of collected data)

<div>
  Data collection is often time consuming and expensive
</div>

<div>
</div>