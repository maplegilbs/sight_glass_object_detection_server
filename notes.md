# Calculating constants for formulas for GPM calculation based off float level.

## Float formula workbook
From image
- sightglass top (ST) = 932
- sightglass height (SH) = 1026
- ruler top (RT) = 1229
- ruler height (RH) = 415

## Desired Output: Flow in gpm as indicated by the float
Given:
- the vertical position (Yf) of the float using 
- the vertical position of the sight glass (Ysg)
- a constant for the position within the sightglass defining the "ruler" determined as the top and the bottom


### Ruler position
- RT - ST / SH = shift % to calculate top of ruler (add to Y coord of sight glass to get Y coord of ruler)
- (1229 - 932) / 1029 = **.2886** *this number may be adjusted to better fit*
- **(SH * .2886 shift %) + ST** = caclulation of top of ruler (Y position)
- (1026 * .2886) + 932 = 1228 

### Calculate Ruler Bottom
- Ruler Size (as % of SH) RH / SH = Ruler Height as % of Sightglass Height
- 415/1026 = **.4045**
- RT + (SH * ruler height %) = ruler bottom
- 1228 + (1026 * .4045) = 1643