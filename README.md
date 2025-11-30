# Challenge Two - CRSS Data Analysis

## Overview
This project analyzes Crash Report Sampling System (CRSS) data from 2022 and 2023 to provide insights into traffic crash patterns, vehicle safety, and person-level crash statistics.

## Important Note About Large Files
This repository uses **Git Large File Storage (Git LFS)** to handle large CSV datasets. Before cloning or working with this repository, you must have Git LFS installed.

### Installing Git LFS

**macOS:**
```bash
brew install git-lfs
git lfs install
```

**Windows:**
Download from [git-lfs.github.com](https://git-lfs.github.com)

**Linux:**
```bash
sudo apt-get install git-lfs
git lfs install
```

### Cloning This Repository

```bash
# Clone the repository
git clone https://github.com/Shar-06/ChallengeTwo.git
cd ChallengeTwo

# Pull LFS files
git lfs pull
```

## Project Structure

```
ChallengeTwo/
├── datasets/
│   ├── CRSS2022CSV/
│   │   ├── person 10.37.10.csv (145.12 MB)
│   │   ├── vehicle 10.37.10.csv (163.54 MB)
│   │   └── vpicdecode.csv (70.70 MB)
│   └── CRSS2023CSV/
│       ├── person.csv (134.45 MB)
│       ├── vehicle.csv (156.74 MB)
│       └── vpicdecode.csv (60.53 MB)
├── src/
├── README.md
└── .gitattributes
```

## Datasets

The project uses CRSS (Crash Report Sampling System) data containing:

- **Person Data**: Information about individuals involved in crashes
- **Vehicle Data**: Vehicle characteristics and crash circumstances
- **VPIC Decode**: Vehicle Product Information Catalog decoding information

**Note:** All CSV files are tracked with Git LFS due to their size (60-163 MB each).

## Installation

1. Ensure Git LFS is installed (see above)
2. Clone the repository
3. Install dependencies:

```bash
# Add your specific installation commands
npm install
# or
pip install -r requirements.txt
```

## Usage

```bash
# Add your specific run commands
npm start
# or
python main.py
```

## Features

- [List your key features]
- [Feature 2]
- [Feature 3]

## Technologies Used

- [List technologies: Python, JavaScript, React, pandas, etc.]
- Git LFS for large file management

## Development

### Setting Up for Development

```bash
# Clone repository
git clone https://github.com/Shar-06/ChallengeTwo.git
cd ChallengeTwo

# Install Git LFS
git lfs install

# Pull large files
git lfs pull

# Install dependencies
[your install command]
```

### Making Changes

When working with the large CSV files:
- They are automatically managed by Git LFS
- No special commands needed for committing
- Regular git workflow applies

## Troubleshooting

### "File exceeds GitHub's file size limit" Error
Make sure Git LFS is properly installed:
```bash
git lfs install
git lfs track "datasets/**/*.csv"
```

### Large Files Not Downloading
```bash
git lfs pull
```

### Slow Clone Times
The large datasets may take time to download. Ensure you have a stable internet connection.

## Contributing

[Add contribution guidelines if applicable]

## License

[Add your license]

## Contact

**Author:** [Your Name]  
**GitHub:** [@Shar-06](https://github.com/Shar-06)

## Acknowledgments

- CRSS data provided by [source organization]
- [Any other acknowledgments]

---

**For Judges:** All large dataset files are managed through Git LFS. After cloning, run `git lfs pull` to ensure all data files are downloaded correctly.
