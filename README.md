# WinDis — Window Disassembly Ontology

**IRI:** `http://example.org/windis#`  
**Format:** OWL 2 (Turtle)

WinDis models window components, their connections, and disassembly steps for reuse-oriented renovation planning.

## Files
- `windis.ttl`: ontology
- `examples/windis-instances.ttl`: demo instances
- `examples/queries/`: sample SPARQL

## Class Hierarchy (overview)

owl:Thing
├─ PhysicalElement
│ ├─ FenestrationAssembly
│ ├─ Component
│ │ ├─ FrameSystem
│ │ │ ├─ Frame
│ │ │ ├─ Subframe
│ │ │ └─ Sash
│ │ ├─ GlazingSystem
│ │ │ ├─ SingleGlazingUnit
│ │ │ ├─ InsulatingGlazingUnit
│ │ │ └─ VacuumIGU
│ │ └─ RetentionAndSealSystem
│ │ ├─ Bead
│ │ ├─ Gasket
│ │ │ ├─ SettingBlock
│ │ │ └─ WedgeGasket
│ │ ├─ GlazingCompound
│ │ └─ Weatherseal
│ └─ WallOpening
│
├─ Connection
│
├─ ProcessModel
│ ├─ DisassemblyPlan
│ ├─ DisassemblyStep
│ │ ├─ RemoveBead
│ │ ├─ RemoveGlazing
│ │ ├─ DetachSash
│ │ ├─ ReleaseBracketOrScrew
│ │ ├─ CutPerimeterFoam
│ │ └─ ExtractFrame
│ ├─ ProcessTool
│ └─ ProcessConstraint
│
├─ Other
│ ├─ ConditionAssessment
│ ├─ EndOfLifeOption
│ └─ ReuseBarrier
│
└─ Attribute
├─ WidthAttribute
├─ HeightAttribute
├─ ThicknessAttribute
├─ UValueAttribute
├─ DurometerAttribute
└─ ResidualServiceLifeAttribute

## How to open in Protégé
1. File → Open → `windis.ttl`
2. (Optional) File → Import… → `examples/windis-instances.ttl`
3. SPARQL tab → paste queries from `examples/queries/`

## Citation
> Fritz Trede (2025). WinDis: Window Disassembly Ontology. GitHub repo: https://github.com/wrldedit/windis-ontology