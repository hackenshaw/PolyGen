# PolyGen
A demo application for procedural generation of 2D polygons

You can get the source code here: https://store.hackenshaw.com/b/jBhuX

## Video
[![Watch the video](https://img.youtube.com/vi/APvosl3d1uc/maxresdefault.jpg)](https://youtu.be/APvosl3d1uc)


## Description
Polygon Generation Script

I needed some polygons for a game I’m working on so I spent a week developing a procedural polygon generator script that can generate polygons based on a few parameters that I can control in real-time.

### Iteration 1: Randomness

Randomly create a few points in 2d space and connect them to each other. 

This creates a polygon, but it does not always work. This is because with this approach, some lines can intersect, and then it's no longer a simple polygon.


### Iteration 2: Simple Polygons

Make sure that no lines are intersecting. Generate some random points, but instead of connecting them right away, first sort them based on angle and THEN connect them.

This works much better but it looks too random and there is no control over what shape you get (except for how many sides it has). 


### Iteration 3: Regular Polygons

To generate a square, or a hexagon, or any other regular polygon, we need a polygon where all sides are equal in length. 

We have the angle and the radius and we can use that calculate the corresponding x,y vectors


### Iteration 4: Irregular Polygons

If we make the angles between the points random we bring back some randomness to our regular polygons, 


### Iteration 5: Concave Polygons

So far, we can generate convex polygons which means that all of its points are pointing outwards. A concave polygon has at least one point pointing inward. So I take a few points and move them in or out by adding a random value to the radius. 


### Iteration 6: Greyscale Mode

A “greyscale mode”



## Download

[Version 1.0.0](https://github.com/hackenshaw/PolyGen/releases/tag/v1.0.0)
