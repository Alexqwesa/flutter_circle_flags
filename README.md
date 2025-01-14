# circle_flags

A collection of circular country flags. 

## Demo

to view all flags https://hatscripts.github.io/circle-flags/gallery

<img src="https://hatscripts.github.io/circle-flags/flags/br.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/cn.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/gb.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/id.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/in.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/ng.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/ru.svg" width="48">
<img src="https://hatscripts.github.io/circle-flags/flags/us.svg" width="48">

## Usage

```dart

// use a valid country code
CircleFlag('us');
CircleFlag('fr');
CircleFlag('es');

```

# Preloading

You might want to preload images for a smoother list scrolling experience:

```dart
// see full example in example
// create preloaded flag loaders bytes
final cache = FlagCache();
completer = cache.preload(['fr', 'us']);
// once the completer completes you can use

CircleFlag(
  'fr',
  cache: cache,
),

```

# Issues & Contributing

This package uses flags from https://github.com/HatScripts/circle-flags

If a change is required to one of the flag the issue should be opened in that repository.

