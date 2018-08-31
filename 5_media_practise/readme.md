# Media screen practise

## Landscapes

```
1. Define variable that define different screen sizes, please you namings that correctly show what screens they are describing
  - large desktop: 1800px
  - medium desktop: 1200px
  - some tablets and desktop: 960px
  - Tabled Portrait: 768px
  - mobile: 320px
```
###  Take this html
```html
<main>
	<h2>1 block</h2>
	<div class="four block">
		<div class="plain colored">
			<div class="inside">
				<div class="text">1 part</div>
			</div>
		</div>
		<div class="plain colored">
			<div class="inside">
				<div class="text">2 part</div>
			</div>
		</div>
		<div class="plain colored">
			<div class="inside">
				<div class="text">3 part</div>
			</div>
		</div>
		<div class="plain colored">
			<div class="inside">
				<div class="text">4 part</div>
			</div>
		</div>
		<div class="clearfix"></div>
	</div>

	<h2>2 block</h2>
	<div class="two block">
		<div class="left colored">
			<div class="inside">
				<div class="text">Left part</div>
			</div>
		</div>
		<div class="right colored">
			<div class="inside">
				<div class="text">Right part</div>
			</div>
		</div>
		<div class="clearfix"></div>
	</div>

	<h2>3 block</h2>
	<div class="three block">
		<div class="right colored">
			<div class="inside">
				<div class="text">Right part</div>
			</div>
		</div>
		<div class="left colored">
			<div class="inside">
				<div class="text">Left part</div>
			</div>
		</div>
		<div class="center colored">
			<div class="inside">
				<div class="text">Centered part</div>
			</div>
		</div>
		<div class="clearfix"></div>
	</div>

	<h2>4 block</h2>
	<div class="three block">
		<div class="right colored">
			<div class="inside">
				<div class="text">Right part</div>
			</div>
		</div>
		<div class="left colored">
			<div class="inside">
				<div class="text">Left part</div>
			</div>
		</div>
		<div class="center colored">
			<div class="inside">
				<div class="text">Centered part</div>
			</div>
		</div>
		<div class="clearfix"></div>
	</div>

	<h2>5 block</h2>
	<div class="three block">
		<div class="right colored">
			<div class="inside">
				<div class="text">Right part</div>
			</div>
		</div>
		<div class="left colored">
			<div class="inside">
				<div class="text">Left part</div>
			</div>
		</div>
		<div class="center colored">
			<div class="inside">
				<div class="text">Center part</div>
			</div>
		</div>
		<div class="clearfix"></div>
	</div>
</main>
```

CSS for base styles:

```css
.block {
  margin-bottom: 10px;
}

.block > div:not(.clearfix) {
  background: #00BCD4;
  border: 1px solid #fff;
  height: 150px;
  color: #fff;
}

.clearfix {
  width: 100%;
  float: none;
  position: relative;
}

.clearfix:after {
  height: 1px;
  width: 100%;
  display: block;
  clear: both;
  content: "";
}

.left {
  float: left;
}

.right {
  float: right;
}

.inside {
  position: relative;
  height: 100%;
  overflow: hidden;
}

.text {
  position: absolute;
  
  transform: translate(-50% ,-50%);
  left: 50%;
  top: 50%;
  z-index: 1;
}
```

And create location for this blocks following instructions:

### Desktop
  1. 1 block -> 4 elements in a row, all equal width
  1. 2 block -> 2 elements in a row, all equal width
  1. 3 block -> 3 elements in a row, .right -> 50%, .left and .center -> 25%
  1. 4 block -> 3 elements in a row, .right -> 25%, .left -> 25% and .center ->50%
  


