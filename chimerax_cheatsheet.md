# ChimeraX Cheatsheet

### Quickstart
```
open 2a1a # open PDB
open 1luz
rename #1 pkr_eif2a; rename #2 vacv_k3

# Align structures
mm #1/A to #2/A

# save and change view
view name 1
turn y -90; view name 2

# save image
save ~/Desktop/img/pkr_k3.png width 900 height 900 transparentBackground true supersample 10

# save movie

# Show the interface
interfaces select #1/B contacting #2/A bothSides true
name sel contacts
show contacts atoms
color contacts red atoms,cartoon

# AlphaFold
open alphafold:Q8IW76 # alphafold:YOUR_UNIPROT_ID
color bfactor #3 palette alphafold

# Renumber residues for AlphaFold predictions
renumber #1/A:1-302 start 250

# Measure distance between atoms
distance #1/B:375@Ca #2/A:45@Ca

# Select charged residues
select #2/A:arg,his,lys,asp,glu

# Label residues
label sel height 1 size 50 font Arial offset 0,0,0
```

### Parameters

pkr green =  #6dc091
vacv k3 purple = #786bac
```
lighting soft
lighting depthCue False
surface resolution 5.5
set bgColor white
graphics silhouettes true
preset cylinders # tubes for alpha-helices
graphics selection color black width 1
```

