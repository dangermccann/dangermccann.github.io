---
layout: page
title: NVIDIA Optix Path Tracer
permalink: /raytracer
hero_image: six-spheres-mis.png
description: For this project I wrote a general purpose path tracer in C++ using the NVIDA OptiX 7.1 ray tracing engine.  
lead: For this project I wrote a general purpose path tracer in C++ using the [NVIDA OptiX 7.1](https://developer.nvidia.com/optix) ray tracing engine.  

sublead: |
  
  <p class="mb-3">
  Source code can be shared upon request. 
  </p>
  <p>
  <a href="/#section-contact" class="btn btn-secondary px-4 py-2 btn-sm">Contact me</a>
  </p>

screenshots:
  - image_url: cornell-mis.jpg
    caption: Cornell box with Multiple Importance Sampling
  - image_url: three-spheres-mis.png
    caption: Three spheres rendered with Multiple Importance Sampling
  - image_url: three-spheres-ray.png
    caption: Three spheres rendered with direct Ray Tracing
  - image_url: six-spheres-ray.png
    caption: Six spheres rendered with direct Ray Tracing
  - image_url: six-spheres-mis.png
    caption: Six spheres rendered with Multiple Importance Sampling

---
The program demonstrates a variety of different rendering techniques from simple Lambertian shading to complex physically based rendering with multiple importance sampling.  

The application parses a scene file to build a graph containing vertices, triangles, spheres, material data and lighting data; it then builds the Optix pipeline containing the ray tracing programs, global acceleration structure containing the scene graph and shader binding table containing the material and lighting data.  The pipeline and data is then sent to the GPU and the ray generation program is launched.  

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
- NVIDIA [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) version 10.1
- Win32 

