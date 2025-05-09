



Package Structure

mcpo_virtual_dataset/
│
├── core/                     # Core coordination and shared logic
│   ├── dataset.py            # MCPO_VirtualDataset (central coordinator)
│   └── base_types.py         # Shared enums, dataclasses, constants
│
├── nodes/                    # Node-specific logic
│   ├── manager.py            # NodeManager class
│   └── utils.py              # Utility functions for nodes
│
├── elements/
│   ├── manager.py            # ElementManager class
│   └── utils.py
│
├── results/
│   ├── time_series.py        # TimeManager or similar
│   ├── selection_sets.py     # SelectionSetManager
│   └── error_checks.py       # ErrorValidator
│
├── plotting/
│   └── plot_manager.py       # PlotManager class
│
├── io/
│   └── hdf5_utils.py         # Common routines for HDF5 access
│
└── __init__.py