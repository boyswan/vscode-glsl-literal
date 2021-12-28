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

## Caveat

If you're not using glslify or another glsl processing library, you will need an identity function named as above to match the syntax.

```js
const glsl = x => x;
```

Alternatively now you can instead use a block comment before the literals to achieve the same thing.

```js
/*glsl*/``
```