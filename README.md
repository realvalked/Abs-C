# Abs-C

## Setup and compilation
```
sudo apt install libx11-dev
cd (Wherever you saved Abs-C to)
make
```
Or simply run the binary!

## Configuration

Add your user to the input group
```
sudo gpasswd -a user input
```

Place abs-c.ini into ~/.config/

### Config options

#### Custom Area
These values are relative to the center of the touchpad/screen and are measured in percent:

`x_scale_pct_min`: Left edge

`x_scale_pct_max`: Right Edge

`y_scale_pct_min`: Top edge

`y_scale_pct_max`: Bottom edge


#### Other options
`keep_ratio`: Enable/Disable Ratio Compensation (Similar to "Keep aspect ratio" on monitors)

`use_pen`: Use an active stylus on a compatible touchscreen tablet, instead of the touchpad

## Usage

If playing on osu!Lazer, disable High Precision Mouse (and Fullscreen, if on Wayland) within Lazer's settings.

Add your user to the input group:

`sudo usermod –a –G input $USER`

Run with:
```
./abs-c
```
