# Just some random OpenGL playground

Run it with `cargo run`.

## Scenes

### `F1` Round Quads

Tons of randomly styled rounded rectangles, spinning faster the closer they are to the mouse.

### `F2` Blurring

An image of Gawr Gura being blurred.
The blur technique used is Kawase blur (two-pass diagonal gaussian blur) with color dithering.

Relevant articles:
- [Scale space implementation > The sampled Gaussian kernel](<https://en.wikipedia.org/wiki/Scale_space_implementation#The_sampled_Gaussian_kernel>)
- [Removing Banding In Linelight](<https://pixelmager.github.io/linelight/banding.html>)
- [Bandwidth-Efficient Rendering (Kawase blur)](<https://community.arm.com/cfs-file/__key/communityserver-blogs-components-weblogfiles/00-00-00-20-66/siggraph2015_2D00_mmg_2D00_marius_2D00_notes.pdf>)
  > I realized my diagonal sampling wasn't a kawase blur to begin with. I'll probably change that later.

Keybinds:
- `K` - Toggle diagonally sampled blur (mistakenly named "kawase", will probably change that later)
- `↑` - Increment blur kernel size
- `↓` - Decrement blur kernel size
- `→` - Increase blur radius
- `←` - Decrease blur radius
