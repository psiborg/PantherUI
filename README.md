PantherUI
=========

Carousel
--------

The Carousel module lets you easily create multi-sided 3D carousels that you can rotate horizontally or vertically.

**Demo:**

http://dl.dropboxusercontent.com/u/5670642/blackberry/webworks/bb10/psiborg/PantherUI/app.html

**Usage:** (see basic1a.html)

1. Include the PantherUI.min.css file, and add your own CSS for size and position.

``` css
<link rel="stylesheet" href="lib/PantherUI.min.css">

<style>
#container1 {
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}
</style>
```

2. Add HTML markup. To create a 4-sided carousel, just add 4 figure elements.

``` html
<section class="panther-Carousels">
    <section id="container1" class="panther-Carousel-container">
        <div id="carousel1" class="panther-Carousel-carousel">
            <figure>
                <div class="panther-Carousel-panelTitleBar"><span class="panther-Carousel-panelTitle">&lt; Carousel 1 &gt;</span></div>
                <div class="panther-Carousel-panelContent">
                    <!-- Panel 1: Add your content here -->
                </div>
            </figure>
            <figure>
                <div class="panther-Carousel-panelTitleBar"><span class="panther-Carousel-panelTitle">&lt; 2 &gt;</span></div>
                <div class="panther-Carousel-panelContent">
                    <!-- Panel 2: Add your content here -->
                </div>
            </figure>
            <figure>
                <div class="panther-Carousel-panelTitleBar"><span class="panther-Carousel-panelTitle">&lt; 3 &gt;</span></div>
                <div class="panther-Carousel-panelContent">
                    <!-- Panel 3: Add your content here -->
                </div>
            </figure>
            <figure>
                <div class="panther-Carousel-panelTitleBar"><span class="panther-Carousel-panelTitle">&lt; 4 &gt;</span></div>
                <div class="panther-Carousel-panelContent">
                    <!-- Panel 4: Add your content here -->
                </div>
            </figure>
        </div>
    </section>
</section>
```

3. Include the PantherUI.min.js file, and add your JavaScript to configure and initialize the carousel(s) by element ID:

``` js
<script src="lib/PantherUI.min.js"></script>

<script>
// Initialize carousel
Panther.Carousel.init({
    id: 'carousel1'
});
</script>
```