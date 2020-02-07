

# LaRoMe

## What a strange name ! 
LaRoME = Label + Region Of Interest + Measure

**Label image** (aka Count Masks): An image in which pixels of an object have all the same value. Each object has a unique value.
 
**Measurement image**: An image in which pixels of an object have all the same value, corresponding to a measurement (Area, Angle, Mean...) 


## ImageJ plugin 

Plugins > BIOP > Image Analysis > ROIs >

## run("Label image to ROIs")

From a **Label Image**(§), generate ROIs and add them to the ImageJ ROI Manager.




<img src="https://github.com/BIOP/ijp-LaRoMe/raw/master/images/Label_image_to_ROIs.png" title="Label_image_to_ROIs" width="75%" align="center">


## run("ROIs to Label image", "")

From an **Image** and some **ROIs**, generates a **Label Image**.
<img src="https://github.com/BIOP/ijp-LaRoMe/raw/master/images/ROIs_to_Label_image.png" title="ROIs to Label Image" width="75%" align="center">


## run("ROIs to Measurement Image", "column_name=Area");

From an **Image**, some **ROIs** and a selected **Measurement** generates a **Measurement Image**.
<img src="https://github.com/BIOP/ijp-LaRoMe/raw/master/images/ROIs_to_Measurement_Image.png" title="ROIsto Measurement Image.png" width="75%" align="center">

Measurement list encompass (change column_name ) : 
"Area", "Angle", "AngleVert","AR", "Circ.", "Major","Minor","Mean","Median","Mode","Min","Max", "Perim."

**Angle** measure is based on horizontal, the **AngleVert** measure is based on vertical (substracting 90 )
 
**AR**, Aspect Ratio = Major / Minor

**Circ.**, Aspect Ratio = 4 * PI * Area / Perim.^2