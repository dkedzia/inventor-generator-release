# Inventor Generator

The `InventorGenerator.exe` is a utility for generating building structures in Autodesk Inventor. This application requires Autodesk Inventor to be running and have the necessary material libraries loaded before execution.

## Usage

To run the generator, execute the `InventorGenerator.exe` with the following required arguments:

```
./InventorGenerator.exe [size] [floors] [pillarWidth] [subsequenceThikness] [wallWidth] [baseMaterialName] [wallMaterialName]
```

### Parameters
- `size` (integer): Specifies the size of the building.
- `floors` (integer): Defines the number of floors.
- `pillarWidth` (integer): Width of the pillars in the building structure.
- `subsequenceThikness` (integer): Thickness of the subsequence layers.
- `wallWidth` (integer): Width of the walls.
- `baseMaterialName` (string): Name of the material to use for the building base.
- `wallMaterialName` (string): Name of the material to use for the walls.

### Example Command

To generate a building with:
- Size: 3
- Floors: 2
- Pillar Width: 25
- Subsequence Thickness: 20
- Wall Width: 15
- Base Material: `P1`
- Wall Material: `C25/30`

Run:

```
./InventorGenerator.exe 3 2 25 20 15 P1 C25/30
```

## Requirements

- **Autodesk Inventor**: Make sure Autodesk Inventor is running before launching the application.
- **Material Libraries**: Ensure that the required material libraries (`baseMaterialName` and `wallMaterialName`) are loaded in Autodesk Inventor.

## Notes

- If any required arguments are missing, the program will display the following error message:

```
Missing required args.
```

- Review and prepare all arguments before execution to avoid errors.

## License

This project is distributed under Apache-2.0 licence.