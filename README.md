![AnywhereOps](icons/AnywhereOps_Logo.PNG)

# AnywhereOps-recipes
[AnywhereOps](https://anywhereops.ai) - Customer-First IT for Innovative Organizations
AutoPkg recipes for automated macOS software deployment via Munki. These recipes automate downloading and importing software packages into your Munki repository.

## Available Recipes

| Application | Description |
|-------------|-------------|
| DellDisplayAndPeripheralManager | Dell monitor and peripheral management |
| DYMO Connect | Label printer software |
| EndNote | Citation management |
| InstallSQLAnywhere | SQL Anywhere database client |
| JohnsonControlsLauncher | Johnson Controls building automation |
| 3D Slicer | Medical imaging and visualization (KitwareInc) |
| Mitel MiTeam Meetings | Video conferencing |
| PasswordSafe | Password manager |
| QuPath | Bioimage analysis for pathology |
| SeqGeq | Flow cytometry data analysis |
| Smartsheet | Project management and collaboration |
| Testcontainers Desktop | Docker testing framework |
| XCodeCLITools | Apple Xcode command line tools |

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


