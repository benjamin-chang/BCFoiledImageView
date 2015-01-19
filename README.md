# Foiled
A shinny UIImageView and CALayer.

## Install
You can install in one of two ways:

1. Copy the source files into your project.
2. Wait for me to write a podspec and install with [Cocoapods](http://cocoapods.org).

## Usage
Create either a `BCFoiledImageView` and set its `foiled` property to `YES`.

```objective-c
BCFoiledImageView *imageView = [[BCFoiledImageView alloc] initWithFrame:self.view.bounds];

//set your image
//imageView.image = [UIImage imageNamed:@"foo"];

imageView.contentMode = UIViewContentModeScaleAspectFit;
imageView.clipsToBounds = YES;
imageView.foiled = YES; //make it shinny!

[self.view addSubview:imageView];
```

Create a `BCFoiledLayer` and add it to a `CALayer`.
```objective-c
BCFoiledLayer *foiledLayer = [MEFoiledLayer layer];
foiledLayer.frame = self.bounds;
[self.layer addSublayer:foiledLayer];

```
