vscode-glsl-literal
====================

Adds GLSL syntax highlighting for JavaScript template literals.

## Match on 

```js
glsl`` | glslify`` | frag`` | vert``
```

## Example

```js
const vert = glsl`
  attribute vec4 aVertexPosition;
  uniform mat4 uModelViewMatrix;
  uniform mat4 uProjectionMatrix;
  void main() {
    gl_Position = uProjectionMatrix * uModelViewMatrix * aVertexPosition;
  }
`;

```
