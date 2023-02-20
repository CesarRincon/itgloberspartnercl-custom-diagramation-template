📢 Use this project, [contribute](https://github.com/{OrganizationName}/{AppName}) to it or open issues to help evolve it using [Store Discussion](https://github.com/vtex-apps/store-discussion).

# Custom Diagramation

![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)

The custom-diagramation-template component allows you to give multiple options to the client to change the position of the elements on the screen.

Desktop
  Grid 1
<img width="1125" alt="image" src="https://user-images.githubusercontent.com/90701896/220188438-59a82ee5-aa50-47b1-88ee-56ff99cf91dd.png">

Desktop Grid 2
<img width="824" alt="image" src="https://user-images.githubusercontent.com/90701896/220188549-9b0281d8-8789-425a-b08c-3250529ef093.png">

Desktop Grid 3
<img width="828" alt="image" src="https://user-images.githubusercontent.com/90701896/220188623-d48504ee-8589-4f62-817c-ee0ac3429865.png">

Desktop Grid 4
<img width="843" alt="image" src="https://user-images.githubusercontent.com/90701896/220188705-ad3577a7-53e2-46a5-9577-11924cec1689.png">

Mobile grid <br>
<img width="295" alt="image" src="https://user-images.githubusercontent.com/90701896/220188982-06006758-48e3-4542-8f8d-5b33c6e0b415.png">

<img width="295" alt="image" src="https://user-images.githubusercontent.com/90701896/220189081-916abb29-5198-4eaa-abd1-b674b6cba52d.png">

## Configuration 

1. Import the special-diagramation app to your theme's dependencies in the manifest.json, for example:
```json
  dependencies: {
    "{vendor}.special-diagramation": "0.x"
  }
 ```
 
 2. Add the custom-grid block to the store-theme. For example:
```json
 "flex-layout.row#custom-grid-container": {
    "children": [
      "custom-grid"
    ]
  },
  "custom-grid": {
    "children": [
      "imagen#grilla1",
      "image#grilla2",
      "image#grilla3",
      "image#grilla4",
      "image#grilla5"
    ]
  }
   ```
|  Block name     | Description                                     |
| -------------- | ----------------------------------------------- |
| `custom-grid` | ![https://img.shields.io/badge/-Mandatory-red](https://img.shields.io/badge/-Mandatory-red)  Top level block that must be declared in the store theme block to render a default custom grid block.   |

## Customization

In order to apply CSS customizations in this and other blocks, follow the instructions given in the recipe on [Using CSS Handles for store customization](https://vtex.io/docs/recipes/style/using-css-handles-for-store-customization).

|CSS HANDLES |
| ----------- | 
|` grid__${gridType} `|
|` gridTypeClass `|
|` grid__itemBig `|
|` grid__itemSmall `|

## Contributors 

Thanks goes to these wonderful people:

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!

---- 

Check out some documentation models that are already live: 
- [Breadcrumb](https://github.com/vtex-apps/breadcrumb)
- [Image](https://vtex.io/docs/components/general/vtex.store-components/image)
- [Condition Layout](https://vtex.io/docs/components/all/vtex.condition-layout@1.1.6/)
- [Add To Cart Button](https://vtex.io/docs/components/content-blocks/vtex.add-to-cart-button@0.9.0/)
- [Store Form](https://vtex.io/docs/components/all/vtex.store-form@0.3.4/)