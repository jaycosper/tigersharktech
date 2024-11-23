# Linux Notes

## Random

### Rescale Photo
```
Script klov_pic.sh
ffmpeg -i $1.jpg -vf scale=720:-2 $1_scaled.jpg
# ffmpeg -i $1.mp4 -vf scale=480:-2 $1_scaled.gif
```

### QR Code
```
xclip -o -s c | qrencode -o - | feh --force-aliasing -ZF -
```

- xclip
    - pastes clipboard command
- qrencode
    - generates QR Code as PNG
- feh
    - display full screen

```
Script
xclip -o -s c | qrencode -o $1.png
```