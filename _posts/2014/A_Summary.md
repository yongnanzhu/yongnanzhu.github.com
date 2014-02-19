---
layout: post
title: A summary  
categories:
- Summary
tags:
- space perception
---

##Questions

* How different hatching ways influence perception of DTI fibers?    
* Where and how to hatch for better perception information (from the literature guideline and Artist drawing suggestion, and their comparison for perception)?

##Summary of the hatching technique

###Hatching Level (Generally convey)

1. no hatching(highlight)    
2. single hatching
3. cross-hatching (could be shadow place)

###Hatching stroke properties

1. stroke orientation: orientation/curvature __===>__ shape cue
2. stroke spacing
3. stroke density(tone, darkness): darkness/tone value/different hatching level __===>__ light intensity(shading cue)
4. stroke length
5. stroke width(thickness): vary with stroke spacing __===>__ depth encoding or other information(TL(total length of streamtube), FA)  
6. one __additional property__ is always used: Number of strokes.

####With the dense streamtube, how to place the hatching stroke direction?
1. place along the streamtube orientation (first principle curvature(maximal principle curvature))?
2. place perpendicular to the streamtube orientation (second principle curvature(minimal principle curvature))?
3. place arbitrary orientation?

Similar paper about Texture pattern orientation: [Visualizing Spatial Relations Between 3D-DTI Integral Curves Using Texture Patterns](http://cs.brown.edu/~wzhou/research/vis2007_stripes_abstract.pdf).

Actually, most people like place the stroke perpendicular to the streamtube orientation, because it is easy for perception.(I think, but there is no people to verify it, it is just a common way.)    

Some papers refer how to draw Cylindric surfaces:    
1. [Line-Art Rendering of 3D-Models](http://pdf.aminer.org/000/540/086/line_art_rendering_of_d_models.pdf)   
2. [Illustrating smooth surfaces](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.37.5140&rep=rep1&type=pdf):  Psychophysical studies confirm that even a few parallel curves can create a strong impression of a cylindrical surface with curves interpreted as principal curvature lines   
...

####Relationship of the four properties which is always used
>Number of stroke, Stroke spacing, Stroke density, Stroke width
#####Single hatching orientation
1. Number of stroke(constant), Stroke spacing(constant), Stroke width(vary) __==>__ Stroke density(vary) 
2. Number of stroke(constant), Stroke density(constant), Stroke width(vary) __==>__  Stroke spacing(vary)  _wide space with narrow stroke width_
3. Stroke spacing(constant), Stroke width(constant), Number of stroke(constant) as place different layers of strokes on same area __==>__ stroke density(tone vary)   

###Conclusion of Hatching variable

So, here, we have hatching related variables:
1. stroke orientation
2. stroke spacing
3. stroke density(tone, darkness)  =>hatching level we will perceive
4. stroke width(thickness)
5. Number of strokes.

Because stroke length is not always used to encoding information, and it usually is used as random length of stroke.  

##Task Design
###Seven task types to answer questions in 3D visualizations of fiber tractography design 

>from [Effects of Stereo and Screen Size on the Legibility of Three-Dimensional Streamtube Visualization](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6327218&tag=1)  

1. Certain numerical measurement metrics (9 metrix from [Quantitative Tractography Metrics of White Matter Integrity in Diffusion-Tensor](http://www.sciencedirect.com/science/article/pii/S1053811908006435) )
2. Spatial relationships of fiber bundles (e.g., for resolving brain connectivity)
3. pathological condition search and manipulation (e.g., is there a lesion? How can fibers be cut to remove a tumor?)
4. Comparisons (e.g., how different are two bundle volumes in two hemispheres? Are two brain tractographies the same? Are they normal?)
5. Categorical (e.g., to which anatomical structure does a bundle belong?)
6. Tube tracing (e.g., where does a tube bundle go?) 
7. Understanding of functional or structural images.

###Pick up task
Actually, we just draw static picture on the paper, so we could not do the interactive task, however, we could make comparison.
###Type 1: Certain numerical measurement metrics

>9 metrix from [Quantitative Tractography Metrics of White Matter Integrity in Diffusion-Tensor](http://www.sciencedirect.com/science/article/pii/S1053811908006435):

>1) total length(TL)  
>2) total weighted length (weighted for linear anisotropy) (TWLCL)   
>3) total weighted length (weighted for FA) (TWLFA)  
>4) number of streamtubes (NS)  
>5) normalized total length(NTL)  
>6) normalized total weighted length – linear anisotropy (NTWLCL)  
>7) normalized total weighted length – FA (NTWLFA)  
>8) normalized number of streamtubes (NNS)  
>9) average length (AL)  

Those matrix varies from length, anisotropy, FA, number of streamtube in the TOI, to their total or normalized.
And I picked up the most common two: __total length(TL)__, FA.
Detailed description are in the picture below:
![ Certain numerical measurement metrics](http://zhuyongnan.cn/picture/2014/2/Certain_numerical_measurement_metrics.JPG) 

###Type 2:Spatial relationships of fiber bundles 
>idea resembles to [Real-Time Illustration of Vascular Structures](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=4015442)  
####fibers occluded with other
Detailed description on the follow picture:
![ fibers occluded with other](http://zhuyongnan.cn/picture/2014/2/fibers_occluded_with_other.JPG) 
####fibers with different distance from the viewport
Detailed description on the follow picture:
![ fibers with different distance from the viewport](http://zhuyongnan.cn/picture/2014/2/fibers_with_different_distance_from_the_viewport.JPG) 

