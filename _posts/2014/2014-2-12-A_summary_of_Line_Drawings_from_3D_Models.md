---
layout: post
title: A summary of Line Drawings from 3D Models 
categories:
- Summary
tags:
- Line drawing， classify
---
##Why begin reading this paper?
Recently, I had spent two days for reading a __Siggraph course__ about Line Drawing---[_Line Drawings from 3D Models_](http://dl.acm.org/citation.cfm?id=1401188), they give me a detail demonstration about what Line drawing is? How people perceive line drawings? They introduce a set of spare line drawings (silhouettes, contours, creases, suggestive contours and highlights, and apparent ridges and valleys) with mathematical definition.  They also describe related algorithms for finding and drawing those lines. Although I have read some related papers about outline before, I am still confused among some of them. I read some of hatching papers(hatching are patterns of lines which use closely spaced parallel lines to convey shading through their local density and convey geometry through their direction), and some line drawing papers. A paper about [Apparent ridges for line drawing](http://dl.acm.org/citation.cfm?id=1276401), they wrote had referred about those line drawings. And here I made a summary just about the different types of line drawings part(Some of them are not related).
    
##Two Picture of summary 
   
![Perception Pipeline](http://zhuyongnan.cn/picture/2014/2/LinesSummary.jpg)       
![Information In Line Drawing](http://zhuyongnan.cn/picture/2014/2/InformationInLineDrawing.jpg)      

They begin with three class of mathematical line definitions:    

* image-space    
* view-independent object-space (It yields lines directly to convey shape)  
* view-dependent object-space (It yields line on the surface to convey shape)

###Line mark fixed location on the shape [_view-independent object-space_]

####1.Creases    

>Creases mark discontinuities in surface orientation (__lines of normal discontinuity__).   
>Crease separates front-and back-faces(silhouette)
>Geometric ridges and valleys are essentially smoothed creases


####2.Ridges and valleys   

>Ridges and valleys mark locally maxima changes in surface orientation.
>Ridges and valleys are __local maxima of principal curvature__, in the corresponding principal direction

####3.Surface markings   

>_Markings on a surface_ can appear as arbitrary lines inside the shape, also could be texture patterns and sets of parallel geodesics

####4.Hatching lines 

>Hatching use repeating __patterns of lines__ to form the basis of hatching. These lines convey shape to produce a gradation of tone with the control of _density_, and also line placement direction(or _orientation_) to convey principal directions of the surface with its curvature.

###Line can mark view-dependent location on the shape [_view-dependent object-space_] 

####1.Contours   

>(1).Contours are those surface Locations at which, from the current viewpoint, there is a __depth discontinuity__.    
>(2).Contours are those surface locations where the surface normal n is perpendicular to the viewing direction v (__n dot v=0__).

####2.Suggestive contours   

>Suggestive contours as local __minima of n dot v__, in the projected view direction w and its perpendicular.    
>Suggestive contours are extensions of occluding contours.(They are curves along which the _radial curvature is zero_)

####3.Apparent ridges

>Apparent ridges are surface locations where the normal vector is changing maximally(maximal view-dependent curvature).
>Apparent ridges as local __maxima of n dot v__, in the projected view direction w and its perpendicular.    


###Lines can mark lighting-dependent location on the shape [_image-space_]

####Isophotes(boundaries of attached shadows or in cartoon shading) 

>Isophotes are curves of __constant illumination__, which also correspond to toon shading boundaries.

####Image space “ridges” and “valleys”.

> Image-space lines are the image intensity “ridges” and “valleys”, These are curves on the surface of locally __maximal/minimal intensity__.

####Edges

>__Local maxima of gradient magnitude__ in gradient direction

####Silhouette

Silhouette could __separate front-facing from back-facing regions__ of the surface, it could be the boundary between the object and the background, it also occluding contours (or sometimes “interior silhouettes”), which marks any depth discontinuities.

Here are some picture:    

Outlines(silhouette, crease, suggestive contours):    

![Outline](http://zhuyongnan.cn/picture/2014/2/Outline.jpg)  

Contours, Ridges and Valleys:    

![Contours, Ridges and Valleys](http://zhuyongnan.cn/picture/2014/2/ContoursAndRidgesValleys.jpg)    

Apparent Ridges:    

![Apparent Ridges](http://zhuyongnan.cn/picture/2014/2/ApparentRidges.jpg)    
