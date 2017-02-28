README for file naming conventions

Layers:

	0_WOOD
	1_250BIT_500DEP
	2_250BIT_250DEP
	3_250BIT_500TAB
	4_250BIT_250TAB
	5_250BIT_250SPEC
	6_125BIT_500DEP
	7_VCARVE_BIT
	8_250BIT_500OUTLINE
	
- File names:

	- Example: "Lens_Oval_X750_Y1625.dxf"
		
		First field is type, in this case a "Lens"
		Second field is sub-type or geometry, in this case "Oval"
			Other sub-types would be:
				Circle
				Square
				Rectangle
				Triangle
				Diamond
		Third (and fourth) field is dimensions, in thousandths of inch
			Other examples:
				Radius == R1000 is 1"
				A == Altitude for triangle
				L == length for square

- Layer naming conventions

	- Example: "1_250BIT_500DEP"
	
		First field is the cut sequence, in this case, "1" is the first cut.
		Second field is the bit size in thousandths, in this case 1/4"
		Third field is the nominal depth in thousandths, in this case 1/2"
		
		Other fields:
			BIT == bit size in thousandths
			DEP == nominal depth in thousandths
				Note if you generate a toolpath with more depth.
			TAB == layers where the cuts are large and need tab routing.
			SPEC == for pockets, etc.
			OUTLINE == outside cut as opposed to normal inside cut.
			VCARVE == 45deg bit
			