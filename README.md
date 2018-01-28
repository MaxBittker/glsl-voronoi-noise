# glsl-voronoi-noise

Voronoi noise, packed for glslify

![example output]()

usage: 
```glsl
precision mediump float;
#pragma glslify: fbm3d = require('glsl-voronoi-noise/3d')

varying vec2 uv;
uniform float t;

void main() {
    gl_FragColor.rgb = voronoi3d(vec3(uv, t);  
    gl_FragColor.a   = 1.0;
}
```

Implementations from Shawn Lawson:
https://github.com/shawnlawson/The_Force/blob/b28befa00fc8c2c128945ee36c55df4e1bb8416d/shaders/header.frag#L186-L226
