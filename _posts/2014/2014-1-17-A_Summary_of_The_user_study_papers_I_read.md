---
layout: post
title: A Summary of The user study papers I read
categories:
- summary
tags:
- paper review
---

In order to have a clear concept about how to do a user study-related research, those days I read some user study-related papers.
Here are the papers:    
1. `TVCG` : ` <<Conveying Shape with Texture: Experimental Investigation of Texture's Effect on Shape Categorization Judgement>>`   
2. `ACM Transaction on Graphics`: `<<Gloss Perception in Painterly and Cartoon Rendering>>`   
3. `ACM Transaction on Graphics`: `<<Where do people draw Lines?>>`   
4. `ACM Transaction on Graphics`: `<<How well Do line Drawings Depict Shape?>>`  
5. Related-papers(Not user study) Dr Chen told me: `TVCG` : ` <<Real-Time illustration of Vascular Structures>>`   

------    
     Just as Dr Chen told me:
     we must know the Focus about the research, what we are doing.
     Usually the process as follows:
     * Survey: build a design space to find your focus.
     * Get the implement about things in design space.(A program or some other ways)
     * Design a User study.
     * Analysis the result.    
------   
So I think It's Time to have a summary.     

about 1. This is a long paper from 2004.    

(1)  There __goal__ is to find the question about `What rendering characteristics should we choose to most effectively convey surface? Which ideal texture pattern to apply?`     
So their __focus__ is texture pattern for shape perception.    

(2)  They did the __survey__ work, and find there are lack of standard reliable ,universally accepted metrics for shape perception. 

(3)  Their __design space__ of texture for shape perception.
> a. Shape categories: ellipsoid, elliptical, clylinder saddle and flat.   
=> This could be used to survive the task for ifentify intrinsic shape of surface.    
> b. Eight different texture pattern.    
> c. Two different viewing conditions.    
> d. Two different projection conditions.     
=> This could be used to survive the task for find the orientation of surface (convex or concave).     

(4) they did a user study.    
(5）they analysis the result with statistics methods.   

Actually, They did another experiment, but the process is likely the same. And here I foucs on how they do their research, not focus on what they do.    

about 2. This is a good paper, I think what I will do could learn some from them.    

(1)  There __goal__ is to find the question about `How well stylized images depict scene properties(shape, material, lighting)?`     
So their __focus__ is material perception of gloss, perception of shiness. What makes gloss? How?    

(2)  They did the __survey__ work, and find there is unclear about that question.    

(3)  Their __design space__ about the parameters do influence the gloss perception(contrast, sharpness)[diffuse, specular]    
parameters:    
>(a). painterly:    
>>brush size,   
brush opacity,   
brush oapcity     

>(b). cartoon style:          
>>a soft qunatization for cartoon.    
a hard qunatization for cartoon.    

>(c). blur(Gaussian blur): remove details in the image

(4) they did a user study.     
>a. Amazon mechanical Turk study.   
>b. Lab study.

>>>Hypotheses
>>>Experimental design: Task and result(analysis)  

about 3. This is a paper with artist.    

(1)  There __goal__ is to find the question about `how well the locations of the artists’ lines correlate with other artists’, with current computer graphics line definitions, and with the underlying differential properties of the 3D surface?`     
So their __focus__ is characterize the _mathematical properties_ of line drawings made by human artists.    
The statictical analysis about describe the lines mathematically part I think is very helpful.    

(2)  They did the __survey__ work, and find 
>a. Artist pays more attentation on the principles of how to make drawings, while little about where on a figure to place lines in oreder to best draw lines.    
>b. There are many ways to convey shape.focus on feature lines, neglect diffuse shading effect, hatching...)   
>c. Su much line drawing options, but don't know which are appropriate for drawing and human perception? and there are lack of a evaluate work for making a comparision.    

(3)  Their __design space__ is about  to capture the relationships between the locations _where human artists draw lines_ and the _mathematical properties_ of the of the model’s surface and appearance at those locations. 
So, I think how to control the artist and how to analyze the result is much important.
>a. what _drawing style_ to consider   
>b. what _models, views, and lighting conditions_ to use as prompts     
>c. how to present these prompts to the artists
>d. what instructions to give the
artists   
>e. __how to scan and process the drawings__  


(4) they did a user study with the artist draw the certain picture and they process drawings to extract the different lines. and after that they did a statistic analysis.    

about 4. This is a good paper, This is the work after 3.    

(1)  There __goal__ find is to how people interpret the line drawings(both hand-draw, and computer-generated)?` and give a quantify analysis about the line drawing to convey the shape.    

(2)  They did the __survey__ work, and there many types of line drawings, but which is good to help shape perception.  
(_This paper give us qualitative and quantitive comparisonabout the effect of different line drawings_)    
(3)  Their __design space__ focus on line drawing, exclude __hatching__ and texture line. 
So,    
>a. what images and drawings to show    
>b. how to sample each image with gauges  
>c. how to structure the presentation to each participate.      
(Gauge is used for the participate to place, to test the effect of different line drawings)     

(4) they did a user study with the task for placing the gauges.


about 5. `TVCG` : ` <<Real-Time illustration of Vascular Structures>>`    

They want to accentuate spatial depth, separation perception [shape and depth].
Three contribution for perception:    
>a. distance-encode shadow [different shadow size], we can perception depth between vacsulars.    
>b. observer-relative depth distance(distance-encode surface) [varying different width of strokes], on the unoccluded surface, we perception the different width of strokes.    
>c. distance between vascular structures and a lesion [different colors, or size of glyphs], we colud perceive different size of glyph texture with the different distance.
