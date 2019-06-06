# Magento2 js init modifier

## See example of using the modifier:

```
<script>
    (function () {
        var galleryOptions = {
            '[data-gallery-role=gallery-placeholder]': {
                'mage/gallery/gallery': {
                    'options': {
                        'thumbmargin': 15,
                        'thumbborderwidth': 1
                    }
                }
            }
        };

        jsInitModifier.setJsInitBlockOptions('mage/gallery/gallery', galleryOptions);

        var minicartOptions = {
            'dropdownDialog': {
                'triggerEvent': 'hover',
                'closeOnMouseLeave': true,
                'timeout': 0
            }
        };

        jsInitModifier.setJsInitBlockOptions('.block-minicart', minicartOptions);
    })();
</script>
```
