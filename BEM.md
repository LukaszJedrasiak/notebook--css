>There are only two hard problems in Computer Science: cache invalidation and naming things — Phil Karlton

BEM is a method of naming CSS objects in order to:
- reduce a time of writing the code,
- reduce the amount of necessary code (and time to load it by browser)
- make the maintaining easier.

## benefits
### modularity
Objects styles in BEM are independent from other elements on page, so it is easy to transfer them from one project to another.

### reusability
Each object styles are independent so you can reuse them in various parts of website without the fear of conflicts with previous rules. Following the CSS recommendations enables to put a block into any place on a page and be sure that it won’t be affected by its surroundings.

### structure
CSS code written by BEM is simply and easy to understand.

## objects in BEM methodology
### blocks
The basic term in BEM methodology is `block`. Block is a standalone entity that is meaningful on its own. Examples:
- header,
- container,
- menu,
- checkbox,
- input.

### elements
`Element` is a part of block that has no standalone meaning and is semantically tied to its block. Examples:
- menu item,
- list item,
- checkbox caption,
- header title.

### modifier
`Modifier` is a flag on a block or element. Use it to change appearance or behavior. Examples:
- disabled,
- highlighted.
- checked,
- fixed,
- size big,
- collor yellow.

## rules
1. Use class names only:
	- Leave tag names for semantical meaning in HTML structure
	- Leave ids for JS scripts.
2. In `block` name you can add a prefix describing the object, i.e. `.block-menu`.
3. An `element` name contains of:
	- parent block name,
	- two underscores,
	- element name.
	Example: `block-menu__menu-item`
4. `Modifier` name contains of:
	- block or element name
	- two dashes
	- modifier name. Spaces in complex modifiers are replaced by single dash.
	Example: `block-menu--background-dark` or `block-menu__menu-item--disabled`.