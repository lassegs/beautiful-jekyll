---
id: 478
title: GIS Revisited
date: 2016-01-19T13:07:38+00:00
author: lassegs
layout: post
guid: http://skole.lassegs.org/?p=478
permalink: /2016/01/19/gis-revisited/
categories:
  - SGO4940
---
<div>
  <em>Andreas Forø Tollefsen</em>
</div>

<div>
  <em> </em>
</div>

<div>
  Summary: Builds on the 1910 course. GIS as a tool to study social phenomena (and beyond). Focus more on data management. Spatial databases. More analysis and modeling. Statistics and space-time problems in GIS. More advanced hands-on tutorials. Some repetition from SGO1910 unavoidable.
</div>

<div>
</div>

### Format of the course

<div>
  Lectures, Tuesday 10.15 &#8211; 12.00. Seminars, Mondays 14.15 &#8211; 16.00. Two weeks to complete seminar, submit before the seminar after next seminar. Individual project work (due May 2, 14.00). Oral exam about the project report (date, TBD, week 20?)
</div>

<div>
</div>

### Individual project (due may 2, 14.00)

<div>
  The aim is to integrate what you have learned in GIS lectures and labs through practical experience. Working individually, you wil address a &laquo;spatial problem&raquo; relevant to your MA. thesis through the collection, mapping and analysis of data, which will then be presented in a concise professional report.
</div>

<div>
  Use what you learn in lectures and seminars. Maybe relevant for MA thesis?
</div>

<div>
  Politics, development, climate, social, spatial, urban change,
</div>

<div>
  Not just mapping, but analyzing, integrating a wide range of knowledge obtained form the course.
</div>

<div style="padding-left: 30px;">
  &#8211; To succeed, include data collection, georeferencing, analysis, cartography + + +
</div>

<div style="padding-left: 30px;">
  &#8211; Theoretical justifications for choosing your approach, data and method.
</div>

<div>
  Start thinking about an idea already now.
</div>

<div>
</div>

<div>
  This course is part of a trial project called &laquo;Digital exam&raquo;.
</div>

<div>
</div>

<div>
  One page project description due soon
</div>

### GIS revisited

<div>
  Almost everything that happens, happens somewhere. Events, cultural differences, forests, vegetation,
</div>

<div>
  Knowing where can be critically important
</div>

<div style="padding-left: 30px;">
  Knowing where adds a lot of information (i. e. proximity of observations). Emergency services, search and rescue, military, transport sector, planning, knowing where conflict takes place. Knowing where gives us a wholly different way, compared to having no position data. Knowing location, also gives us proximity of observations. The relationships between the observations.
</div>

<div>
  Scale, or level of detail
</div>

<div style="padding-left: 30px;">
  Our geographic scale depends on what we want to &laquo;see&raquo;. Magnifying glass or countries?
</div>

<div>
  Purpose
</div>

<div style="padding-left: 30px;">
  Scientific or practical (pragmatic GIS)? Help us out, help society out with communication and planning. On the other side we have the scientific part, where we use spatial information to derive new knowledge. Find clusters of phenomena, etc.
</div>

<div>
  Timescale
</div>

<div style="padding-left: 30px;">
  A fundamental problem. GIS is good at showing a space in a particular time, but not over time. Mapping crime for example, you would have to choose a time interval, which will affect the results. Short to long term. Animations? Space/time figures?
</div>

<div style="padding-left: 30px;">
</div>

### Spatial is special

<div>
  Almost all human activities and decisions involve a geographic component.
</div>

<div>
  Geographic component adds important information.
</div>

<div>
  Spatial data is different from data
</div>

<div>
  All spatial data has X and Y coordinates, at least a geographic reference
</div>

<div>
  Large in data size terms &#8211; especially complex polygons
</div>

<div>
  Scale &#8211; in spatial data scale is of high importance. What is included
</div>

<div>
  Special analytical and statistical methods. In general it has to do with the geographic component. In regular statistics we have dependent and independent variables. In statistics one assumes that observations are independent, but in spatial data one can actually check the dependence.
</div>

<div>
  Visualizations are much cooler with spatial data
</div>

<div>
</div>

### Point in polygon

<div>
  Common spatial relationship between datasets.
</div>

<div>
</div>

### GI-systems/science

<div>
  Systems usually refers to the tools we use. Science refers to the study of spatial data and methods used to manage and analyze spatial data.
</div>

<div>
  Knowledge about how the world works is more valuable than knowledge about how it looks bevause it can be used to predict and understand.
</div>

<div>
</div>

### From data to knowledge

<div>
  Six parts of GIS: Software, people, data, procedures, hardware, network. Machine learning is automatic analysis of data, and takes away the people part.
</div>

<div>
</div>

### Representation

<div>
  How do we construct a digital model (GIS) representing aspects of the surface of the Earth?
</div>

<div>
  Our representation in a data model depends fully on our ontology.
</div>

<div>
  Can we represent all heterogeneity? Variation and minority class/objects/groups/&#8230; We cannot show everything, so we must choose.
</div>

<div>
  What is non-representable?
</div>

<div>
  GIS is subject to critique in Geography:
</div>

<div style="padding-left: 30px;">
  Homogeneity, Majorities, Ethical (surveillance), technologicaly driven, for the privileged, critical research.
</div>

<div style="padding-left: 30px;">
  Increasing acceptance across the sub-disciplines
</div>

<div>
</div>

### Records and attributes

<div>
  Records &#8211; observations/cases/<strong>features</strong> &#8211; rows. One row for each observation
</div>

<div>
  Attributes &#8211; Variables &#8211; Columns
</div>

<div>
</div>

### How do we register attributes? Scales of measurement 1

<div>
  Nominal sacle: Classification based on names or in distinct categories without order: Colors (red, green, blue). Land types (forest, grass, gravel). Municipality number (219, 123, 423).
</div>

<div>
  Using names can create duplicates. Many places named Springfield in the US (38).
</div>

<div>
</div>

<div>
  Ordinal values: Classification of distinct categories with a rank order, meaning some things are more or less than others.
</div>

<div style="padding-left: 30px;">
  Dichotomous: Sick vs healthy, peace vs war
</div>

<div style="padding-left: 30px;">
  non-dichotomous: Small, medium, large ball.
</div>

<div style="padding-left: 30px;">
</div>

<div>
  Interval values: Constant intervals between values, but not the ratio between. Cannot say taht 20 C is twice as hot as 10 C. The zero is abitrarily chosen
</div>

<div>
</div>

<div>
  Ratio scale: Contant intervals between the values and an absolute zero. Weight, volume, distance, height.
</div>

<div>
</div>

<div>
  Cyclic values: Compass direction, months of the year.
</div>

<div>
</div>

### What about objects?

<div>
  Two fundamentally different ways to represent geography: Discrete objects and continious fields.
</div>

<div>
</div>

<div>
  Vector: Discrete objects with well defined boundaries. Points, lines and polygons. Can all have attributes with information.
</div>

<div>
  Raster: Continuous fields. Pixel values represents information. One value per pixel.
</div>

<div>
</div>

<div>
  Raster is faster, but vector is corrector.
</div>

<div>
</div>

<div>
  Generalization of polygons. A real feature is digitized, and we exclude small variations. We can not make perfect representations of everything. We must accept some level of generalization, some level of reduction of quality and exacteness.
</div>

<div>
</div>

<div>
  Continious fields: Non-discrete objects, not fixed in space, but varies continiously across space. Altitude is a good example: Any X, Y point on earth has elevation (z). Also population density. Air temperature. Vegetation, land types.
</div>

<div>
  Rasters consists of grid cells, rectangular, usually squared cells, where geographic variation is represented by pixels as values. We always lose details in the representation.
</div>

<div>
</div>

<div>
  Common for both discrete objects and continious fields is that internal variation within the object is masked / ignored.
</div>

<div>
  We either have to accept the homogeneous nature of geographic representation, or make choices of what to represent: The average within the polygon? Majority land class? What exists in the center?
</div>

<div>
  If this is unacceptable, increase raster resolution, or increase the number of objects.
</div>

<div>
</div>

<div>
</div>

<div style="padding-left: 30px;">
</div>

<div style="padding-left: 30px;">
</div>

&nbsp;