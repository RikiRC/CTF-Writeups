# emote
# Description:
recently i've been converting strings into images for funsies and staring at them. anytime time to go share those images with my friends in discord! warning: staring at noise in visual form may or may not introduce you to the abyss

# Solution:
- Go to the discord of UIUCTF and check profile of ian5v (creator of this flag)
- You will find that ian5v has posted some weird looking emote - https://cdn.discordapp.com/emojis/870834335257882624.png?v=1
- Download the emote and check it with zsteg:
  - zsteg -a emote.png
- At payload "b1,r,lsb,xy" you will see the flag

# Flag:
uiuctf{staring_at_pixels_is_fun}
