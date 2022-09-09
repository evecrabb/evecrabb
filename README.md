![banner](images/eve.jpeg)

ALL OF THIS IS WIP AT THE MOMENT

[Breakpoints](#breakpoints)



# About me

Hi! I'm Eve, a Senior Developer at [giffgaff](https://www.giffgaff.com). 

# Utilities

These functions have been designed to be as similar as possible to the design system functions in the documentation.

Jump to:

- [Breakpoints](#breakpoints)
- [Layout tokens](#layout-tokens)
- [Colours](#colours)
- [Pastel Colours](#pastel-colours)
- [Icons](#icons)
- [Images](#images)
- [Spacers](#spacers)
- [Typography scale](#typography-scale)
- [Strikethrough](#strikethrough)
- [Gradients](#gradients)
- [Digital Noise](#digital-noise)
- [Borders](#borders)
- [Doodles](#doodles)
- [Sparkles](#sparkles)
- [Grid size](#grid-size)

## Breakpoints

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Tiny </td>
<td> 320px </td>
<td>

```tsx
@media (min-width: ${styles.breakpoint('tiny')}) {
  // your styles here
}
```

</td>
</tr>
<tr>
<td> Small </td>
<td> 360px </td>
<td>

```tsx
@media (min-width: ${styles.breakpoint('small')}) {
  // your styles here
}
```

</td>
</tr>
<tr>
<td> Medium </td>
<td> 768px </td>
<td>

```tsx
@media (min-width: ${styles.breakpoint('medium')}) {
  // your styles here
}
```

</td>
</tr>
<tr>
<td> Large </td>
<td> 992px </td>
<td>

```tsx
@media (min-width: ${styles.breakpoint('large')}) {
  // your styles here
}
```

</td>
</tr>
</table>

## Layout Tokens

```
${styles.layout('item')}
```

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Min width </td>
<td> 320px </td>
<td>

```tsx
${styles.layout('min-width')}
```

</td>
</tr>
</table>

**Options**:
'min-width', 'max-width', 'readable-width', 'header-height'

## Full Width Container

This gives you the same styling that the [full-width-container](https://www.giffgaff.design/design-fundamentals/breakpoints/) mixin in the design system does. There is no need to add any extra css into this - just the function.

```jsx
const Component = styled.htmlTag`
  ${styles.fullWidthContainer()};
`
```

Or, add 'readable-width' to create readable-width container styles.

```
${styles.fullWidthContainer('readable-width')};
```

## Colours

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Black </td>
<td> `#000000` </td>
<td>

```tsx
${styles.colour('black')};
```

</td>
</tr>
<tr>
<td> White </td>
<td> `#FFFFFF` </td>
<td>

```tsx
${styles.colour('white')};
```

</td>
</tr>
<tr>
<td> Light pink </td>
<td> `#EB5F8E` </td>
<td>

```tsx
${styles.colour('light-pink')};
```

</td>
</tr>
<tr>
<td> Light green </td>
<td> `#72B72A` </td>
<td>

```tsx
${styles.colour('light-green')};
```

</td>
</tr>
<tr>
<td> Light blue </td>
<td> `#35ADCE` </td>
<td>

```tsx
${styles.colour('light-blue')};
```

</td>
</tr>
<tr>
<td> Yellow </td>
<td> `#FCC31E` </td>
<td>

```tsx
${styles.colour('yellow')};
```

</td>
</tr>
<tr>
<td> Red </td>
<td> `#d60000` </td>
<td>

```tsx
${styles.colour('red')};
```

</td>
</tr>
<tr>
<td> Dark blue </td>
<td> `#00528A` </td>
<td>

```tsx
${styles.colour('dark-blue')};
```

</td>
</tr>
<tr>
<td> Olive </td>
<td> `#B9CC3F` </td>
<td>

```tsx
${styles.colour('olive')};
```

</td>
</tr>
<tr>
<td> Turquoise </td>
<td> `#00CEB3` </td>
<td>

```tsx
${styles.colour('turquoise')};
```

</td>
</tr>
<tr>
<td> Light orange </td>
<td> `#F39722` </td>
<td>

```tsx
${styles.colour('light-orange')};
```

</td>
</tr>
<tr>
<td> Lavender </td>
<td> `#C380BB` </td>
<td>

```tsx
${styles.colour('lavender')};
```

</td>
</tr>
<tr>
<td> Graphite </td>
<td> `#2F2E31` </td>
<td>

```tsx
${styles.colour('graphite')};
```

</td>
</tr>
<tr>
<td> Dove grey </td>
<td> `#666666` </td>
<td>

```tsx
${styles.colour('dove-grey')};
```

</td>
</tr>
<tr>
<td> Alto </td>
<td> `#D0D0D0` </td>
<td>

```tsx
${styles.colour('alto')};
```

</td>
</tr>
<tr>
<td> Wild sand </td>
<td> `#F5F5F5` </td>
<td>

```tsx
${styles.colour('wild-sand')};
```

</td>
</tr>
<tr>
<td> Gallery </td>
<td> `#ECECEC` </td>
<td>

```tsx
${styles.colour('gallery')};
```

</td>
</tr>
</table>

### Pastel Colours

Please ensure you adhere to the guidelines for using pastel colours.

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Yellow </td>
<td> `#FEF3D2` </td>
<td>

```tsx
${styles.pastelColour('yellow')};
```

</td>
</tr>
<tr>
<td> Green </td>
<td> `#E3F1D4` </td>
<td>

```tsx
${styles.pastelColour('green')};
```

</td>
</tr>
<tr>
<td> Red </td>
<td> `#FBE6E6` </td>
<td>

```tsx
${styles.pastelColour('red')};
```

</td>
</tr>
<tr>
<td> Blue </td>
<td> `#D7EFF5` </td>
<td>

```tsx
${styles.pastelColour('blue')};
```

</td>
</tr>
</table>

## Icons

### Icon Size

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Small </td>
<td> 16px </td>
<td>

```tsx
${styles.iconSize('small')};
```

</td>
</tr>
<tr>
<td> Medium </td>
<td> 24px </td>
<td>

```tsx
${styles.iconSize('medium')};
```

</td>
</tr>
<tr>
<td> Large </td>
<td> 48px </td>
<td>

```tsx
${styles.iconSize('large')};
```

</td>
</tr>
<tr>
<td> Huge </td>
<td> 72px </td>
<td>

```tsx
${styles.iconSize('huge')};
```

</td>
</tr>
<tr>
<td> Gargantuan </td>
<td> 120px </td>
<td>

```tsx
${styles.iconSize('gargantuan')};
```

</td>
</tr>
<tr>
<td> Colossal </td>
<td> 192px </td>
<td>

```tsx
${styles.iconSize('colossal')};
```

</td>
</tr>
</table>

### getIcon

Add the name of the file, without the .svg extension. Since all icons in the design system are svg files, this has been built into the function.

```jsx
background-image: url(${styles.icon('fileName')});
```

This will return the url of the icon from the Design System's icon library, which can be found [here](https://www.giffgaff.design/iconography/icons/)

## Images

### getImage

Note: there is no need to include the image extension in these functions.

```
${styles.jpeg('fileName')}

${styles.png('fileName')}

${styles.svg('fileName')}

${styles.gif('fileName')}
```

This will return the url of an image from the Design System's image library, which can be found [here](s3://static.test.gaff.systems/design-system/style-guide/latest/images/)

### getImageSize

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Tiny </td>
<td> 72px </td>
<td>

```tsx
${styles.imageSize('tiny')}
```

</td>
</tr>
<tr>
<td> Small </td>
<td> 120px </td>
<td>

```tsx
${styles.imageSize('small')}
```

</td>
</tr>
<tr>
<td> Medium </td>
<td> 192px </td>
<td>

```tsx
${styles.imageSize('medium')}
```

</td>
</tr>
<tr>
<td> Large </td>
<td> 312px </td>
<td>

```tsx
${styles.imageSize('large')}
```

</td>
</tr>
<tr>
<td> Huge </td>
<td> 504px </td>
<td>

```tsx
${styles.imageSize('huge')}
```

</td>
</tr>
</table>

## Spacers

<table>
<tr>
<th> Name </th> <th> Value </th> <th> Code </th>
</tr>
<tr>
<td> Fine </td>
<td> 4px </td>
<td>

```tsx
${styles.spacer('fine')}
```

</td>
</tr>
<tr>
<td> Tiny </td>
<td> 8px </td>
<td>

```tsx
${styles.spacer('tiny')}
```

</td>
</tr>
<tr>
<td> Small </td>
<td> 16px </td>
<td>

```tsx
${styles.spacer('small')}
```

</td>
</tr>
<tr>
<td> Medium </td>
<td> 24px </td>
<td>

```tsx
${styles.spacer('medium')}
```

</td>
</tr>
<tr>
<td> Large </td>
<td> 48px </td>
<td>

```tsx
${styles.spacer('large')}
```

</td>
</tr>
<tr>
<td> Huge </td>
<td> 72px </td>
<td>

```tsx
${styles.spacer('huge')}
```

</td>
</tr>
</table>

## Typography Scale

This, like the design system, will import all of the behaviours, including media queries, into your components. Lovely.

<table>
<tr>
<th> Name </th> <th> Code </th>
</tr>
<tr>
<td> Whisper </td>
<td>

```tsx
${styles.typographyScale('whisper')};
```

</td>
</tr>
<tr>
<td> Whisper Loud </td>
<td>

```tsx
${styles.typographyScale('whisper-loud')};
```

</td>
</tr>
<tr>
<td> Murmur </td>
<td>

```tsx
${styles.typographyScale('murmur')};
```

</td>
</tr>
<tr>
<td> Murmur bold </td>
<td>

```tsx
${styles.typographyScale('murmur-bold')};
```

</td>
</tr>
<tr>
<td> Speak </td>
<td>

```tsx
${styles.typographyScale('speak')};
```

</td>
</tr>
<tr>
<td> Speak up </td>
<td>

```tsx
${styles.typographyScale('speak-up')};
```

</td>
</tr>
<tr>
<td> Loud </td>
<td>

```tsx
${styles.typographyScale('loud')};
```

</td>
</tr>
<tr>
<td> Loud bold </td>
<td>

```tsx
${styles.typographyScale('loud-bold')};
```

</td>
</tr>
<tr>
<td> Louder </td>
<td>

```tsx
${styles.typographyScale('louder')};
```

</td>
</tr>
<tr>
<td> Shout </td>
<td>

```tsx
${styles.typographyScale('shout')};
```

</td>
</tr>
<tr>
<td> Megaphone </td>
<td>

```tsx
${styles.typographyScale('megaphone')};
```

</td>
</tr>
</table>

## Strikethrough

Adds strikethrough styling to the target element.

```jsx
const Component = styled.htmlTag`
  ${styles.strikethrough(textStyle, blackText)};
```

e.g.

```jsx
const Component = styled.htmlTag`
  ${styles.strikethrough('shout', true)};
```

## Gradients

This will import media query behaviours, just as the design system gradients do.

<table>
<tr>
<th> Name </th> <th> Code </th>
</tr>
<tr>
<td> Pink to blue </td>
<td>

```tsx
${styles.gradient('pink-to-blue')};
```

</td>
</tr>
<tr>
<td> Yellow to pink </td>
<td>

```tsx
${styles.gradient('yellow-to-pink')};
```

</td>
</tr>
<tr>
<td> Blue to yellow </td>
<td>

```tsx
${styles.gradient('blue-to-yellow')};
```

</td>
</tr>
<tr>
<td> Rainbow </td>
<td>

```tsx
${styles.gradient('rainbow')};
```

</td>
</tr>
</table>

## Digital Noise

This will allow the use of our digital noise as outlined [here](https://www.giffgaff.design/design-fundamentals/digital-noise/)

<table>
<tr>
<th> Name </th> <th> Code </th>
</tr>
<tr>
<td> Side </td>
<td>

```tsx
${styles.digitalNoise('side')};
```

</td>
</tr>
<tr>
<td> Bottom </td>
<td>

```tsx
${styles.digitalNoise('bottom')};
```

</td>
</tr>
<tr>
<td> Chunky </td>
<td>

```tsx
${styles.digitalNoise('chunky')};
```

</td>
</tr>
</table>

## Borders

This adds a giffgaff border to an element.

Please note that any colour can be used from the giffgaff colour palette (apart from pastels), but please try to stick to black as per design system guidelines.

```jsx
const Component = styled.htmlTag`
  border: ${styles.border('black')};
```

## Doodles

This adds a giffgaff 'doodle' to an element. Optional styling available for colours and different text styles of the element you are applying the doodle to.

```jsx
const Component = styled.htmlTag`
  ${styles.doodle(style, colour, textStyle)};
```

e.g.

```jsx
const Component = styled.htmlTag`
  ${styles.doodle('boing', 'light-pink', 'louder')};
```

## Sparkles

This adds a 'sparkle' to an element. Supports two types ('fine', 'chunky') and four sizes ('small', 'medium', 'large', 'huge').

```jsx
const Component = styled.htmlTag`
  ${styles.sparkle(type, size)};
```

e.g.

```jsx
const Component = styled.htmlTag`
  ${styles.sparkle('chunky', 'medium')};
```

## Grid Size

This gives access to the grid units from the design tokens. Simply pass in a multiplier to get the correct 'px' value.

```jsx
const Component = styled.htmlTag`
  width: ${styles.gridSize(3)};
```



## Stack 

- ### **My Stack**

<img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-plain-wordmark.svg" alt="HTML logo" width="50px" height="50px" />  <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg" alt="CSS logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/sass/sass-original.svg" alt="SASS logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/less/less-plain-wordmark.svg" alt="LESS logo" width="50px" height="50px" />  <img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" alt="JavaScript logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/nextjs/nextjs-original-wordmark.svg" alt="NextJS logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/eleventy/eleventy-original.svg" alt="Eleventy logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/php/php-original.svg" alt="PHP logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/jenkins/jenkins-original.svg" alt="Jenkins logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original-wordmark.svg" alt="NodeJS logo" width="50px" height="50px" />  <img src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-original-wordmark.svg" alt="Docker logo" height="50px" width="50px" />   <img src="https://github.com/devicons/devicon/blob/master/icons/git/git-plain-wordmark.svg" alt="Git logo" width="50px" height="50px" /> <img src="https://github.com/devicons/devicon/blob/master/icons/visualstudio/visualstudio-plain.svg" alt="VS Code logo" height="50px" width="50px" />

## GitHub statistics

![My's GitHub stats](https://github-readme-stats.vercel.app/api?username=evecrabb&show_icons=true&theme=prussian)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=evecrabb&hide=html&theme=prussian)](https://github.com/anuraghazra/github-readme-stats)


## Credits

* [devicon](https://github.com/devicons) and [Terence Eden & co](https://github.com/edent/SuperTinyIcons) for the icons.
* [Anurag Hazra](https://github.com/anuraghazra/github-readme-stats) for the GitHub stats.
* [Claire Lemonnier](https://github.com/lemocla) for the inspiration.
