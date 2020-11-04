---
layout: default
title: Optix Pathtracer
permalink: /pathtracer
---

# Optix Ray Tracer & Path Tracer
![Path traced spheres](./assets/images/three-spheres-mis.png "Path traced spheres")

For this project I wrote a general purpose path tracer in C++ using the [NVIDA OptiX 7.1](https://developer.nvidia.com/optix) ray tracing engine.  The program demonstrates a variety of different rendering techniques from simple Lambertian shading to complex physically based rendering with multiple importance sampling.  

The application parses a scene file to build a graph containing vertices, triangles, spheres, material data and lighting data; it then builds the Optix pipeline containing the ray tracing programs, global acceleration structure containing the scene graph and shader binding table containing the material and lighting data.  The pipeline and data is then sent to the GPU and the ray generation program is launched.  

- Source code can be shared upon request.   [Contact me](./contact/)

### Program Capabilities  
- Ray generation program can generate multiple samples per pixel with sub-pixel jitter. 
- Intersection program supports triangle and sphere primitives with arbitrary matrix transformations. 
- Ray traced lighting program with support for point and direct lights using Blinn-Phong shading. 
- Direct lighting path tracer capable of illuminating scenes containing area lights with Monte Carlo estimation.   
- Indirect light path tracer with cosine and BRDF importance sampling with implementations of modified Phong and GGX BRDFs. 
- Can optionally use Russian roulette path termination. 
- Multiple importance sampling employs both direct lighting and BRDF importance sampling using power heuristic weighting. 

### Technologies Used
- C++
- [NVIDIA OptiX 7.1](https://developer.nvidia.com/optix)
- NVIDIA[CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) version 10.1
- Win32 


### Screen shots
Cornell box with Multiple Importance Sampling
![Multiple Importance Sampling](./assets/images/cornell-mis.jpg "Cornell Box with Multiple Importance Sampling")
- 128 samples per pixel
- Modified Phong and GGX BRDFs 
- Single area light
<hr/>

Six spheres rendered with direct Ray Tracing
![Ray Traced Spheres](./assets/images/six-spheres-ray.png "Ray Traced Spheres")
- 4 samples per pixel
- Three overhead point light sources 
- Maximum render depth of 5
- Blinn-Phong BRDF 
<hr/>

Six spheres rendered with Multiple Importance Sampling
![Path Traced Spheres with MIS](./assets/images/six-spheres-mis.png "Path Traced Spheres with MIS")
- 256 samples per pixel
- Modified Phong and GGX BRDFs 
- Three overhead area light sources
<hr/>

Six spheres rendered with direct Ray Tracing
![Ray Traced Spheres](./assets/images/three-spheres-ray.png "Ray Traced Spheres")
- 4 samples per pixel
- Three overhead point light sources 
- Maximum render depth of 5
- Blinn-Phong BRDF 
<hr/>

Three spheres rendered with Multiple Importance Sampling
![Path Traced Spheres](./assets/images/three-spheres-mis.png "Path Traced Spheres")
- 256 samples per pixel
- Modified Phong and GGX BRDFs 
- Three overhead area light sources


