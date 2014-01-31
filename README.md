jquery.dark-overlay
===================

A small jQuery plugin for adding a dark, semi-transparent overlay over a set of matched elements.

This currently only works on static elements (i.e. if you change the size or position of an element after adding an overlay, the overlay will not follow).

This hasn't yet been tested throughly on all browsers. In particular, I doubt that the "allowClickThrough" option works on older IE browsers (I don't have any older IE browsers handy to test with).

Example usage:
    $('SELECTOR').darken();

    which is equivalent to...
    $('SELECTOR').darken(0.5);

    which is equivalent to...
    $('SELECTOR').darken({
        'opacity': 0.5,
        'allowClickThrough': true
    });

    $('SELECTOR').undarken();

    $('SELECTOR').toggleOverlay();
