# Games101 Experiment 5

## Experiment Content

- Implement Whitted-style ray tracing.
- The two key functions in this experiment are `Render` and `rayTriangleIntersect`.
- The `Render` function is mainly responsible for computing the direction of rays cast from the camera to each pixel. The basic idea is to first convert screen coordinates to coordinates on the near plane in clip space. The ray direction vector is then obtained by subtracting the camera origin from these coordinates.
- The `rayTriangleIntersect` function is used to determine whether a ray intersects a triangle. If an intersection occurs, it also returns the barycentric coordinates of the intersection point and the value of `tNear`. The intersection test is implemented using the Möller–Trumbore algorithm.

## Experiment Result

- <img src="https://github.com/corgiInequation/Games101_WhittedStyleRayTracing/blob/main/image.png" alt="ray-tracing-result" width="67%" />
- As shown, Whitted-style ray tracing effectively handles both reflection and refraction effects.
