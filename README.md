This is a collection of pixel art fonts that I have made. They are entirely for fun, and therefore are available for free.

They are licensed under the [SIL OFL](OFL.txt), see the [OFL FAQ](OFL-FAQ.txt) for usage instructions.

The fonts under the *bg* folder have a black background, the *no-bg* folder have a transparent background.

The original Aseprite files are under the *ase* folder.

The names are all of the form name_*w*x*h*, where *w* and *h* refer to the number of pixels wide and high that each glyph is. All glyphs are packed with no padding--the padding is built-in to the characters. The range of all fonts is standard ASCII, 32-126, and you can actually get the offset into the png using this formula:

```python
char_w, char_h = 8, 8  # from the font name
c = 97  # any ASCII codepoint

char_x = char_w * (c % 16)
char_y = char_h * ((c // 16) - 2)

# Then the glyph is at (char_x, char_y) 
# with (char_w, char_h) as the subregion
```

### Credits

Phantasm is based heavily on the wonderful [Alagard](https://www.dafont.com/alagard.font) font. It's basically a rescale with some characters redone to fit inside the 10x10 bounding box. Check it out if you're looking for a non-monospaced version!
