# openmaptiles-fonts

Hosted fontstacks to serve with openmaptiles.

These fonts come from the
[openmaptiles/fonts](https://github.com/openmaptiles/fonts) repository. That
repository contains the code to generate these fontstacks, but the actual fonts
themselves are in the _releases_, and thus you can't point a style directly at
that repository.

This repository hosts the individual fontstack files, so you can just add
```
"glyphs": "https://raw.githubusercontent.com/kylebarron/openmaptiles-fonts/master/fonts/Metropolis/{fontstack}/{range}.pbf"
```
to your style.

## Using

In order to load fonts in a Mapbox GL style, you need to have a key in your Style JSON with a `glyphs` key. For Mapbox-hosted styles and styles that point to Mapbox, [this is usually](https://docs.mapbox.com/mapbox-gl-js/style-spec/glyphs/).

```
"glyphs": "mapbox://fonts/mapbox/{fontstack}/{range}.pbf"
```

In order to serve these fontstacks from this repository, just change that to:

```
"glyphs": "https://raw.githubusercontent.com/kylebarron/openmaptiles-fonts/master/fonts/Metropolis/{fontstack}/{range}.pbf"
```

You can also fork this repository, to make sure that you can easily host the
fonts for as long as Github is running. If you do so, just change `kylebarron`
with your Github username.

## License

Please mind the license of the original fonts. All fonts are either licensed under OFL or Apache.
