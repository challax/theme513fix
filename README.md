## What?


Adds a min-height: rule to .Content .ProductList .ProductImage refrence in Styles.css.

## Why?


The current refrence is missing a height attribute and IE doesnt respect max-height property. Setting a min-height causes all of the images to be the same height regardless of the resolution of the image. 

https://jira.bigcommerce.com/browse/THEME-513


## Testing /Proof


Before :
.Content .ProductList .ProductImage img {
	vertical-align: middle;
}


After:
.Content .ProductList .ProductImage img {
	vertical-align: middle;
  min-height:275px !important;
  }
