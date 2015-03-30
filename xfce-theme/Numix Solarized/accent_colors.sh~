#!/bin/bash
# Sets the selected_bg_color to one of the Solarized accent colors

# Color prompt
read -p "Please chose an accent color. (yellow, orange, red, magenta, violet, blue, cyan, green or custom) : " color

if [ $color = yellow ]
	then
               hexcolor=b58900
elif [ $color = orange ]
	then
               hexcolor=cb4b16
elif [ $color = red ]
	then
               hexcolor=dc322ff
elif [ $color = magenta ]
	then
               hexcolor=d33682
elif [ $color = violet ]
	then
               hexcolor=6c71c4
elif [ $color = blue ]
	then
               hexcolor=268bd2
elif [ $color = cyan ]
	then
               hexcolor=2aa198
elif [ $color = green ]
	then
		hexcolor=859900
elif [ $color = custom ]
	then
               read -p "Please chose an hex code for the color (without the #): " hexcolor
fi

# Sed operations

sed -i 's/selected_bg_color #.*;/selected_bg_color #$hexcolor;/g' gtk-3.0/gtk.css
sed -i 's/selected_bg_color #.*;/selected_bg_color #$hexcolor;/g' gtk-3.0/gtk-dark.css
sed -i 's/nselected_bg_color:#.*\\ntext/nselected_bg_color:#$hexcolor\\ntext/g' gtk-2.0/gtkrc

# Feedback

echo "Accent color set to $color (#$hexcolor)"
