# Foiled
A shinny UIImageView and CALayer

## Usage
Create either a `BCFoiledImageView` or `BCFoiledLayer` and set its `foiled` property to `YES`.

```objective-c
BCFoiledImageView *imageView = [[BCFoiledImageView alloc] initWithFrame: self.view.bounds];

//set your image
//imageView.image = [UIImage imageNamed:@"foo"];

imageView.contentMode = UIViewContentModeScaleAspectFit;
imageView.clipsToBounds = YES;
imageView.foiled = YES; //make it shinny!

[self.view addSubview:imageView];
```
