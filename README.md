# MetAge: Metabolic Transition Modeling in Aging Cells

MetAge is a computational biology framework for modeling metabolic transitions in aging cells, with a particular focus on NAD+/NADPH balance and pathway analysis in peripheral blood mononuclear cells (PBMCs).

## Overview

This project aims to understand metabolic changes during cellular aging by modeling and analyzing various metabolic pathways. The primary goal is to identify factors that lead to abnormal metabolic states and explore potential interventions for restoring "young" metabolic profiles.

### Key Research Questions
- How do metabolic pathway flows change during cellular aging?
- What factors lead to increased NADPH with NAD+ depletion?
- Can we identify interventions (e.g., glutamine supplementation) to restore normal metabolic states?

## Features

- Integration with metabolic databases (KEGG, Recon3D)
- Flux Balance Analysis (FBA) implementation
- Flux Variability Analysis (FVA)
- Compartment-specific metabolic modeling
- Pathway visualization and analysis tools
- HIF-1a regulation modeling

## Installation

```bash
# Clone the repository
git clone https://github.com/muzykantov/metage.git
cd metage

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Project Structure

```
metage/
├── notebooks/               # Jupyter notebooks for analysis
│   ├── 1_data_loading.ipynb
│   ├── 2_kegg_analysis.ipynb
│   ├── 3_model_building.ipynb
│   ├── 4_fba_analysis.ipynb
│   └── 5_visualization.ipynb
├── src/                    # Source code
│   ├── data_loader.py
│   ├── model_utils.py
│   └── visualization.py
├── data/                   # Data directory
│   ├── raw/               # Raw data files
│   └── processed/         # Processed data files
└── results/               # Analysis results
```

## Analyzed Pathways

1. TCA Cycle
2. Urea Cycle
3. Methionine Cycle
4. Folate Cycle
5. Glycine Cleavage System
6. Glycolysis
7. Pentose Phosphate Pathway
8. Glutathione Metabolism
9. De novo Serine Synthesis

## Dependencies

- Python 3.8+
- COBRApy
- BioPython
- python-libsbml
- pandas
- numpy
- matplotlib
- Jupyter

## Usage

1. Start with the notebooks in sequential order:
```bash
jupyter lab
```
2. Follow the analysis workflow in each notebook
3. Check results in the `results/` directory

## Contributing

Contributions are welcome! Please read our contributing guidelines and submit pull requests to our repository.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Citation

If you use this project in your research, please cite:

```bibtex
@software{metage2025,
  author = {Gennadii Muzykantov},
  title = {MetAge: Metabolic Transition Modeling in Aging Cells},
  year = {2025},
  url = {https://github.com/muzykantov/metage}
}
```

## Contact

Gennadii Muzykantov - gennadii@muzykantov.me

Project Link: https://github.com/muzykantov/metage

## Acknowledgments

- KEGG Database for metabolic pathway information
- Recon3D for human metabolic model
- COBRApy development team
- BiGG Models database
