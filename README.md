# Polybar Redshift

Simple redshift toggle switch. Displays current redshift display temperature target.

<img src="https://imgur.com/F8n0WOz"/>

## Dependencies

- redshift
- polybar

## Usage

- Left click to toggle on/off

# Configuration

- Move `redshift.sh` to ~/.config/polybar/scripts/redshift.sh
- Make `redshift.sh` executable
- Load `redshift.sh` from polybar config 

```INI
[module/redshift]
type = custom/script
format-prefix = " "  
exec = ~/.config/polybar/scripts/redshift.sh temperature 
click-left = ~/.config/polybar/scripts/redshift.sh toggle 
interval=1.0
```