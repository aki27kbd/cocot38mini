# cocot38mini Case Guide

cocot38mini provides various case data depending on mounting methods, ball support styles and ball holding geometries. This guide shows the overview of each method, including pros/cons as well as BOM of it.

![cocot38mini_main00](/images/main_00.jpg)

# Mounting Method

![mounting_method](/images/Mounting_Method.jpg)

### Integrated
Plate-integrated mount is the simplest mounting method with fewer parts required to assemble. No additional parts are required to build this case. As the plate is thick and integrated with the case structure, it provides a solid feeling relative to other mounting methods.

|Parts|Qty|Note|
|---|---|---|
|3D Printed Top Case|1|Top case named with "_integrated"|
|3D Printed Bottom Case|1|cocot38mini_v2_bottom.stp|

### Top Mount
Top mount is the general mounting method which is also used for some of custom keyboards. Assembly is relatively difficult due to the need of heated insert nuts. Typing softness can be adjusted depending on the plate material.   
**SLA (Resin) is not suitable for heated insert nut. If you use it as a case material, make sure you fix insert nuts with glue.**

|Parts|Qty|Note|
|---|---|---|
|3D Printed Top Case|1|Top case named with "_topmount"|
|3D Printed Switch Plate|1|Plate named with "_topmount"|
|3D Printed Bottom Case|1|cocot38mini_v2_bottom.stp|
|Heated Insert Nut|8|[HFB-2001](https://hirosugi.co.jp/products/B/HFB.html#bx1)|
|M2 Screw 3mm|8||

### Tadpole Mount
Tadpole mount is designed considering the balance of simple structure and better typing feel. Assembly is relatively easy as long as tadpoles are available. Typing softness can be adjusted depending on the hardness of tadpoles.

|Parts|Qty|Note|
|---|---|---|
|3D Printed Top Case|1|Top case named with "_tadpole"|
|3D Printed Switch Plate|1|Plate named with "_tadpole"|
|3D Printed Bottom Case|1|cocot38mini_v2_tadpole_bottom.stp|
|Tadpole|8|Available at [GEONWORKS](https://geon.works/products/tadpole) or [GREENKEYS](https://shop.green-keys.info/products/tadpole)|

# Ball Supporting Method

![ball_support_method](/images/Ball_Support_Method.jpg)

### Zirconia Balls
3x Φ2mm zirconia balls support the ball. No additional parts needed. Once zirconia balls are installed, <u>**bearing rollers can not coexist with them**</u>.

|Parts|Qty|Note|
|---|---|---|
|Zirconia Ball|3|Φ2mm|

### Bearing Rollers
3x bearing rollers support the ball. Ball handling is smoother with less resistance. Bearing roller dimension is ID: 3mm / OD: 6mm / W: 2.5mm.　　　
Refer to [picot5400](https://github.com/aki27kbd/picot5400/blob/main/doc/buildguide_en.md#ball-case) for assembly.

|Parts|Qty|Note|
|---|---|---|
|Bearing Roller|3|ID:3mm x OD:6mm x W:2.5mm|
|Steel Pin|3|Φ2mm x L:6mm|
|Silicon Tube|1|ID: 2mm x OD:3mm|

# Ball Holding Method

![ball_holding_method](/images/Ball_Holding_Method.jpg)

### Claw Holder
Claw holder is integrated with the top case and no additional parts needed. Due to the thin structure, it is <u>**not recommended**</u> printing this model with FDM printers.

|Parts|Qty|Note|
|---|---|---|
|3D Printed Top Case|1|Top case named with "_claw"|

### Magnet Cover
Magnet cover is an additional part attached to the top case with magnets. Depending on case clearance, glue might be needed to fix magnets.

|Parts|Qty|Note|
|---|---|---|
|3D Printed Top Case|1|Top case named with "_magnet"|
|3D Printed Ball Cover|1|cocot38mini_v2_ballcover.stp|
|Magnet|8|Φ3mm x H:2mm|
