Duke Nukem 3D Extended Color Look-up Table Pack
By Lezing Entertainment, 2010

  FINAL VERSION CHANGELOG

- 3DRealms logo palette fixed to avoid using the reserved colors (tiles009.art included).
- The reserved colors were removed from the logo animation palette (logo.anm included).
- Pal #121 now gives negated logarithm instead of converting the self-luminous colors; this pal was used in the test map to show textures correctly in white fog.

  SHADES

The conventional 32-shade table is preserved with duplicate colors isolated (they are made non-shadable except the color #160).

  PALETTES

26 original pals (##0-25) are preserved with duplicate colors removed; 102 custom pals (##26-127) are introduced. Pals ##129-132 are used for EDuke32 color fog. Pal #128 is the same as pal #0. Some pals may considerably distort image, so try tweaking your scene to improve the look. See EXTCLUTS.MAP for some examples.
  Colorizers
    Pal # 26: Everything is pale brown
    Pal # 27: Everything is gray
    Pal # 28: Everything is brown
    Pal # 29: Everything is orange
    Pal # 30: Everything is violet
    Pal # 31: Everything is spectral
    Pal # 32: Everything is bright yellow
  Unicolorous
    Pal # 33: Whiteness
    Pal # 34: FFness (use with translucency to brighten things up)
  Color filters/replacers
    Pal # 35: Blue is orange
    Pal # 36: Blue is pale brown
    Pal # 37: Blue is light blue
    Pal # 38: Blue is light red
    Pal # 39: Blue is light gray
    Pal # 40: Blue and red are spectral
    Pal # 41: Some colors desaturated
    Pal # 42: Colors are red-shifted
    Pal # 43: Blue is dark brown
    Pal # 44: Blue is sand-colored
    Pal # 45: Blue is bright brown
    Pal # 46: Colors are blue-shifted; red is blue
    Pal # 47: Various colors exchanged
    Pal # 48: Green is violet
    Pal # 49: Blue is violet
  Color lighters
    Pal ID   Coloration       Gain (f-stops)
      50:   Bright orange         0
      51:   Pale orange           0
      52:   Pale brown            0
      53:   White                 0
      54:   Red                   0
      55:   Orange                0
      56:   Alt. bright orange    0
      57:   Yellow                0
      58:   Pale yellow           0
      59:   Brown                 0
      60:   Blue                  0
      61:   Pale blue             0
      62:   Green                 0
      63:   Violet                0
      
      64:   Bright orange        +1
      65:   Pale orange          +1
      66:   Pale brown           +1
      67:   White                +1
      68:   Red                  +1
      69:   Orange               +1
      70:   Alt. bright orange   +1
      71:   Yellow               +1
      72:   Pale yellow          +1
      73:   Brown                +1
      74:   Blue                 +1
      75:   Pale blue            +1
      76:   Green                +1
      77:   Violet               +1
      
      78:   Bright orange        +2
      79:   Pale orange          +2
      80:   Pale brown           +2
      81:   White                +2
      82:   Red                  +2
      83:   Orange               +2
      84:   Alt. bright orange   +2
      85:   Yellow               +2
      86:   Pale yellow          +2
      87:   Brown                +2
      88:   Blue                 +2
      89:   Pale blue            +2
      90:   Green                +2
      91:   Violet               +2
      
      92:   Bright orange        +3
      93:   Pale orange          +3
      94:   Pale brown           +3
      95:   White                +3
      96:   Red                  +3
      97:   Orange               +3
      98:   Alt. bright orange   +3
      99:   Yellow               +3
     100:   Pale yellow          +3
     101:   Brown                +3
     102:   Blue                 +3
     103:   Pale blue            +3
     104:   Green                +3
     105:   Violet               +3
     
     106:   Bright orange        +4
     107:   Pale orange          +4
     108:   Pale brown           +4
     109:   White                +4
     110:   Red                  +4
     111:   Orange               +4
     112:   Alt. bright orange   +4
     113:   Yellow               +4
     114:   Pale yellow          +4
     115:   Brown                +4
     116:   Blue                 +4
     117:   Pale blue            +4
     118:   Green                +4
     119:   Violet               +4
  Exotic filters
    Pal # 120: Collection of special colors (see below)
    Pal # 121: InvLog (negated logarithm of a source channel linear combination)
    Pal # 122: Yellow toon
    Pal # 123: Purple toon
    Pal # 124: Red toon
    Pal # 125: Green toon
    Pal # 126: Blue toon
    Pal # 127: One more collection of special colors (darkeners only)

  TRANSLUCENCY

Now gamma-corrected to 2.0, also fixed an error with the transparent color being purple instead of black. Removed unnecessary data in the end of PALETTE.DAT.

  UTILIZING REPEATED COLORS

There are 5 redundant blacks in the Duke palette; also 3 near-black shades are repeated. Shade and palette tables were modified to avoid using these colors. Use palette #120 with different textures to access them. They were adapted to support corresponding special effects when translucent:
  Color ID   Translucent    Reverse translucent   Pal #120 hues         Pal #127 hues
     32:       +2 stops       +1 stops              Gray                  -
     80:       Reverse        Negate                Brown                 -
     81:       RGB to BGR     Hue invert            Blue                  -
     96:       -2 stops       -1 stops              Green                 Gray, yellow, pale brown
     97:       -4 stops       -3 stops              Red                   Green, red, orange
    128:       -6 stops       -5 stops              Yellow, pale brown    Brown, violet
    160:       InvExp         InvLog                Orange                Blue
    161:       Grayscale      50% desaturated       Violet                -
    255:       3x bright      1.5x bright           -                     -
Color #239 is also the same as the #143, but has an alternate shading model and thence has been preserved. Color #255 is transparent, so it's never displayed in sprites or masks unless you're using palette #34 (FFness). Color #160 is the only one that alternates between various effects when shaded.

  POSSIBLE COMPATIBILITY ISSUES

- This mod is partially compatible with Polymost renderer, take note that the special color effects will work only in 8-bit software mode.
- Color fog pals are moved to 129-132.
- Some colors of the logo animation are screwed up due to palette #0 altered.
- Gamma-corrected translucency table alters the look of some structures (like sprite shadows which appear fainter). Nevertheless, in usual conditions it gives significantly better results.
- You won't see any changes in LEBuild, since it uses its own color tables.

  FORMAT OF BUILD TABLES

I made some reverse-engineering to examine these files. Use this section if you're gonna alter your files using a Hex editor. The addresses are listed for the extended files, not the original Duke DATs.

PALETTE.DAT:

  Address range        Description                   Size
0x0000  -  0x02FF    BGR main palette (0-63)       [0x0300]
0x0300  -  0x0301    Number of shades (up to 128)  [0x0002]
0x0302  -  0x2301    Shade tables                  [0x0100 * wordptr(0x0300)]
0x2302  - 0x12301    Translucency table            [0x10000]

LOOKUP.DAT:

  Address range        Description                                        Size
           0x0000    Number of pals                                     [0x0001]
0x0001  -  0x8080    Palettes (first byte is the mapped ID, up to 127)  [0x0101 * byteptr(0x0000)]
0x8081  -  0x8380    Underwater palette (BGR 0-63)                      [0x0300]
0x8381  -  0x8680    Night vision palette (BGR 0-63)                    [0x0300]
0x8681  -  0x8980    Duke3D logo palette (BGR 0-63)                     [0x0300]
0x8981  -  0x8C80    3DRealms logo palette (BGR 0-63)                   [0x0300]
0x8C81  -  0x8F80    Episode 1 Seq palette (BGR 0-63)                   [0x0300]
