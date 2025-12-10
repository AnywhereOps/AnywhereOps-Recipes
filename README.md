![[AnywhereOps](icons/AnywhereOps_Logo.PNG)](https://anywhereops.ai)


# [AnywhereOps](https://anywhereops.ai) - Customer-First IT for Innovative Organizations
AutoPkg recipes for automated macOS software deployment via Munki. These recipes automate downloading and importing software packages into your Munki repository.

## Available Recipes

| Application | Description | Status |
|-------------|-------------|--------|
| DellDisplayAndPeripheralManager | Dell monitor and peripheral management | 
| DYMO Connect | Label printer software |
| EndNote2025 | Citation management | Complete |
| InstallSQLAnywhere | SQL Anywhere database client |
| JohnsonControlsLauncher | Johnson Controls building automation |
| 3D Slicer | Medical imaging and visualization (KitwareInc) |
| Mitel MiTeam Meetings | Video conferencing |
| PasswordSafe | Password manager | 
| QuPath | Bioimage analysis for pathology | Complete |
| SeqGeq | Flow cytometry data analysis | In Development |
| Smartsheet | Project management and collaboration | Complete |
| Testcontainers Desktop | Docker testing framework | Complete |
| XCodeCLITools | Apple Xcode command line tools | TODO for .munki |
## Prerequisites

- [AutoPkg](https://github.com/autopkg/autopkg) v2.3 or later
- [Munki](https://github.com/munki/munki) repository configured

## Usage

### Add this recipe repository

```bash
autopkg repo-add https://github.com/anywhereops/AnywhereOps-recipes
```

### Run a recipe

```bash
# Download and import to Munki
autopkg run com.github.anywhereops.munki.Smartsheet

# Or run the download recipe only
autopkg run com.github.anywhereops.download.Smartsheet
```

### List available recipes

```bash
autopkg list-recipes | grep anywhereops
```

---


