# Lab 03 - CSS

Write the CSS selectors for the following:

1. All `p` elements within an element with id of `blog-post`.

    Answer: `#blog-post p`. :link: [more](https://github.com/comp-2511/css-intro#descendant-selector)

1. All elements with class of `mru` within an element with id of `university`.

    Answer: `#university .mru` :link: [more](https://github.com/comp-2511/css-intro#descendant-selector)

1. All `a` elements that redirect the page to the MRU website (`https://www.mtroyal.ca` or `mtroyal.ca` or `www.mtroyal.ca` or `mru.ca`).

    Answer: `a[href*="mtroyal.ca"], a[href*="mru.ca"]` :link: [more](https://github.com/comp-2511/css-intro#partial-match-attribute-value-selector)

1. All images that have the `alt` attribute.

    Answer: `img[alt]` :link: [more](https://github.com/comp-2511/css-intro#simple-attribute-selector)

1. All `section` elements that come right after a `header` element.

    Answer: `header ~ section` :link: [more](https://github.com/comp-2511/css-intro#sibling-selector)

1. All `aside` elements that are direct children of a `main` element and come after a `section` and an `article` elements.
    ```html
    <main> 
        <section></section>
        <article></article>
        <aside></aside>
        <aside></aside>
    </main>
    ```
    Answer: `main > section + article ~ aside` :link: [more](https://github.com/comp-2511/css-intro#adjacent-sibling-selector)

1. All `strong` elements that are direct children of `a` elements within a `nav` element with `id` of `navigation`.

    ```html
    <nav id="navigation"> 
        <a>
            <strong></strong>
        </a>
        <a>
            <strong></strong>
        </a>
    </nav>
    ```

    Answer: `nav#navigation a > strong` :link: [more](https://github.com/comp-2511/css-intro#children-selector)

1. All `a` elements that use the secure HTTP protocol (HTTPS) in their `href` attribute.

    ```html
    <a href="https://..."></a>
    <a href="https://..."></a>
    <a href="https://..."></a>
    ```

    Answer: `a[href^="https"]` :link: [more](https://github.com/comp-2511/css-intro#partial-match-attribute-value-selector)

1. All `div` elements with the class `warning` and `notification`.

    ```html
    <div class="warning notification"></div>
    <div class="notification warning"></div>
    ```

    Answer: `div.warning.notification` :link: [more](https://github.com/comp-2511/css-intro#multiple-classes)


1. All `table` elements that have the attribute `border` set to `1`.

    Answer: `table[border="1"]` :link: [more](https://github.com/comp-2511/css-intro#exact-attribute-value-selector)
