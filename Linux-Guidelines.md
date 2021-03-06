## File:
**Editor:** Adobe Illustrator or SVG editor

**Dimensions:** `48x48` pixels
* Please, no inches or non-square rectangles.

**Vector Save:** .AI or .SVG

**Export:** 48x48 SVG (double check SVGs created in Adobe Illustrator)

**Pixel Perfection:** Please never use "Align Objects to Pixel Grid". It ruins absolutely everything. You should instead manually check that all dimensions and positions are all whole numbers.

## Objects:
**Keyline Shapes:**
* Rectangles: `38x38` (Square), `44x32` (Landscape), `32x44` (Portrait)
  * `3px` Radius rounded corners
* Circle: `44x44`

**Maximum Area:** `44x44`

**Raised Objects:** *Need:* Long shadows, tints, shades, and drop shadows [*(See Raised Objects)*](#raised-objects)

**Finish:** *Need:* On very top layer, special radial gradient, fills the icon's silhouette [*(See Finish)*](#finish)

**Whole Icon:** *Need:* Tint, shade, drop shadow, raised object shadows clipped off if applicable [*(See Whole Icon)*](#whole-icon)

## Colors:
* Material Design Palette colors as much as possible. (some greens and special colors don't apply)
* Limit use of gradient spots or objects (excluding lighting effects, -45° only)
* Shade, drop Shadows, and long shadows have the appropriate shade color for the object it is on (not necessarily the object where lighting effect is from)

## Text:
* Use Roboto for generic text, logo font or path for specialized text. (logos for Pandora, Facebook, etc)
* `Create Outlines` before creating long shadows, drop shadows, tints, shades, or aligning.
* `Make Compound Path` before creating tints or shades

## Long Shadows:
**Gradient:** 
* Type: `Linear`
* Starting Node: `20% Opacity` *Color:* `Shade Color`
* Gradient Slider Midpoint: `Position 50%`
* End Node: `5% Opacity` *Color:* `Shade Color`
* Angle: `-45 degrees`

**Shape:** Created by using a `Blend` *from* a copy of the object at its original location *to* a copy of the object transformed -45 degrees with the outside anchors completely off the artboard (canvas)
* Blend: Use `Specified Steps` and pick a higher number for higher accuracy (for curvature)
  * More than 50 but less than 500 steps
  * `Pathfinder` > `Crop` using a copy of to the object(s) it's on
    * Remove the outline and leave the other objects(s)
  * Use the `Lasso Tool` in `Isolation Mode` to eliminate extra anchors that cause a staircase effect or awkward curvature

## Raised Objects:
**Tint and Shade:** Use the `Difference` (`Minus`) of two copies of the object separated vertically by a pixel
* Don't use duplicate objects and use them without making it the difference and realigned onto the object
* [Use these helpful `Actions` for creating and aligning tints and shades](https://goo.gl/pguAcr)

**Tint:**
* Use 20% opacity white for all colors but Gray 50 to Gray 300
* Use 40% opacity white for Gray 50 to Gray 300 (100% when tint looks better on Gray 50 only)

**Shade:** 
* Must have at least one shade, preferred to have both.

Type One:
* Shade on the object on the last pixel up against the edge.

Type Two:
* If doesn't touch the outside perimeter (or transparency in case of glass effect): 1px below the object that creates the light effect.

* Don't leave a gap between the shade and the object

**Crease:** Avoid folding or creasing the raised object if you do the object below without aligning them correctly

**Drop Shadow:**

Metrics:
* Mode: `Normal`

Type One (-45 Degree):
* `1px` offset for both X and Y (For the -45 degree lighting)

Type Two (Top Down):
* `0px` X and `1px` Y offset
* `1px` blur
* Colors: `Shade color`

* Clip off the shadows if they extend past the icon's perimeter
* Use long and drop shadow [*(See Long Shadow)*](#long-shadow)

## Finish: Radial gradient overlay on the top layer of the icon
**Gradient:**
** Mode: `Radial`
* Starting Node: `10% Opacity` *Color:* `White`
* Gradient Slider Midpoint: `Position 33%` (Spec Material) **or**
* Gradient Slider Midpoint: `Position 50%` (In Google's Icons)
* End Node: `0% Opacity` *Color:* `White`
* Angle: `-45 degrees`
* Shouldn't create white outside of the icon 
* Radial Circle: Covers the entire icon perimeter (not including drop shadows)
* Starting Point: Moved over at far as it can go towards the -45 indicator handle

## Whole Icon:
Shouldn't extend past the `2px margin` on all for side of the icon for a max area of `44x44` pixels

**Drop Shadow:** Add two fills to the appearance of the icon layer or group
* Stroke Color: No stroke
* Fill Color: `White`
* Mode: `Multiply`
* Top Shadow:
  * Mode: `Multiply`
  * `0px` offset for both X and Y
  * `.5px` blur
  * Color: `black` (#000000, not #202020)
* Bottom Shadow:
  * Mode: `Multiply`
  * `0px` offset for X and a `1px` for Y
  * `.5px` blur
  * Color: `black` (#000000, not #202020)

* Make sure the objects making the outside perimeter of the icon have a tint and shade that are on the object
* If there is a drop shadow for a glyph that extends off of the icon, clip it so it doesn't interact with the whole icon's drop shadow

## Icon Complexity:
* Don't over complicate the icons with excessive raised object
  * Think wisely about using more than two (including keyline or base shape)
* Don't and too many spot colors that won't scale well for lower densities.

## Read More:
* See Google's Product Icon Specification: [Here](https://www.google.com/design/spec/style/icons.html#icons-product-icons)
* Download our template: [Here](https://github.com/materialos/Icon-Submission/blob/master/Daniel%20Hickman/Template/product-icon-template.ai?raw=true)


***

#### Key:
`Values or Menu Items`

*Meta Text*

**Item:** Main text
* Child item
  * Grandchild item

[Link](#)