# Unreal Directive Website Data

This is the official **Unreal Directive Website Data** repository, which contains the JSON files used to display content for the [Unreal Directive website](https://unrealdirective.com). The goal of this repository is to make it easy for the community to collaborate on and contribute to the website's data, ensuring it remains relevant, accurate, and up-to-date.

## Table of Contents

- [Introduction](#introduction)
- Getting Started
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- Data
  - [Unreal Engine Asset Naming Conventions](#unreal-engine-asset-naming-conventions)
  - [Unreal Engine Console Variables](#unreal-engine-console-variables)
- Contributing
  - [Submitting a Pull Request](submitting-a-pull-request)
  - [Forking the Repository](#forking-the-repository)
  - [Publishing Your Own Version](#publishing-your-own-version)
- [License](#license)
- [Contact](#contact)

## Introduction

The JSON files in this repository are used to dynamically generate content for the Unreal Directive website. By hosting these files in an open-source repository, I aim to foster a collaborative environment where anyone can contribute to the project and help maintain the website's data.

## Getting Started

To get started, you'll need to clone this repository to your local machine.

### Prerequisites

- Git

### Installation

1. Clone the repository:

```bash
git clone https://github.com/UnrealDirective/website-data.git
```

2. Change to the repository directory:

```bash
cd website-data
```

3. Browse and edit the JSON files as needed.

## Data

### Unreal Engine Naming Conventions

In this repository, we follow specific naming conventions for Unreal Engine assets. The JSON format for the naming conventions is as follows:

```json
{
    "Domain": "",
    "Asset Type": "",
    "Prefix": "",
    "Suffix": "",
    "Example": "",
    "Notes": ""
}
```

- **Domain**: The category or context of the asset (e.g., Animation, Material, Texture).
- **Asset Type**: The specific type of asset within the domain (e.g., Character, Prop, UI).
- **Prefix**: A short code added at the beginning of the asset name to indicate its type (e.g., `M_` for Material, `T_` for Texture).
- **Suffix**: A short code added at the end of the asset name to provide additional information (e.g., `_N` for Normal Map, `_D` for Diffuse Map).
- **Example**: A sample asset name that follows the naming convention (e.g., `T_Metal_Steel_BC`).
- **Notes**: Additional information or guidelines about the naming convention, if applicable.

Here's an example of a naming convention JSON entry for base color texture:

```json
{
    "Domain": "Texture",
    "Asset Type": "Texture (Base Color)",
    "Prefix": "T_",
    "Suffix": "_BC",
    "Example": "T_Example_BC",
    "Notes": "Base Color, Albedo, Diffuse"
},
```

By adhering to these naming conventions, we can maintain consistency and clarity throughout the project, making it easier for contributors to understand and work with the assets.

### Unreal Engine Console Variables

In this repository, we also store information about Unreal Engine Console Variables, which are used to configure various engine settings during development and debugging. The JSON format for these variables is as follows:

```json
{
    "name": "",
    "help": "",
    "type": "",
    "default": "",
    "notes": ""
}
```

- **name**: The console variable's name (e.g., `r.StaticMeshLODDistanceScale`).
- **help**: A brief description of the console variable's purpose and functionality (e.g., "Scales the distance at which Static Mesh LODs change.").
- **type**: The console variable's type (e.g., `Var`).
- **default**: The default value of the console variable (e.g., `1`).
- **notes**: Any additional notes or recommendations regarding the console variable, if applicable.

Here's an example of a naming convention JSON entry for an Unreal Engine Console Variable related to the level of detail (LOD) settings for static meshes:

```json
{
    "name": "r.StaticMeshLODDistanceScale",
    "help": "Scales the distance at which Static Mesh LODs change.",
    "type": "Var",
    "default": "1",
    "notes": "Values > 1 increase the LOD transition distance, and values < 1 decrease it."
}
```

By documenting these console variables, we aim to create a useful and easy-to-reference resource for developers working with Unreal Engine, making it easier to understand and use various engine settings.

## Contributing

I encourage and appreciate contributions from the community! Here are some ways to contribute:

### Submitting a Pull Request

1. Fork the repository.
2. Create a new branch with a descriptive name (e.g., `update-asset-naming-convention-data`).
3. Commit your changes to the new branch.
4. Submit a pull request to the `main` branch, providing a clear description of your changes.

### Forking the Repository

If you'd like to create your own fork of the repository, simply click the **Fork** button at the top of this page. This will create a copy of the repository under your GitHub account, allowing you to make changes independently.

### Publishing Your Own Version

If you've made significant changes to the data and would like to publish your own version of the Unreal Directive website, follow these steps:

1. Fork the repository.
2. Make the necessary changes to the JSON files.
3. Deploy your version of the website using a hosting provider of your choice (e.g., GitHub Pages, Netlify, Vercel, etc.).
4. Share your version with the community!

## License

This project is licensed under the CC0 1.0 Universal License, which means the content is dedicated to the public domain and can be used freely without any restrictions. See the [LICENSE](LICENSE) file for more information.

## Contact

If you have any questions, issues, or suggestions, please feel free to open an issue or reach out to the Unreal Directive team:

- Unreal Directive: https://unrealdirective.com/contact
- Email: [contact@unrealdirective.com](mailto:contact@unrealdirective.com)

Thank you for your interest in the Unreal Directive Website Data repository! I look forward to your contributions.