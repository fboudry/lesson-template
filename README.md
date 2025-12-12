# Lesson Template Repository

This repository is a template for creating lessons based on Quarto files. Each file in the `lecture/`, `tutorial/` and `practicum/` directories is a separate module, and a global file (`template.qmd`) combines them into a complete lesson. Alternatively you can use a git submodule containing all your modules, set up as `Lessons-modules` in this template.

## Directory Structure

- `Lessons-modules`: Contrains all modules in an external repository.
- `lecture/`: Contains individual lesson modules.
- `tutorial/`: Contains individual tutorial modules.
- `practicum/`: Contains individual practicum modules.
- `assets/`: Contains images, videos, and other media files.
- `styles/`: Contains custom CSS or themes.
- `scripts/`: Contains custom JavaScript or R scripts.
- `output/`: Contains the final combined output files.

## How to Add a New Module

1. Create a new Quarto file in the `lecture/`, `tutorial/` or `practicum/` directory.
2. Add a reference to the new module in the global Quarto file.

> [!NOTE]  
> You can indicate assets path as if you were in the `assets/` folder.

## How to Generate the Combined Output

1. Open the global Quarto file.
2. Render the file with `quarto render _filename_` to generate the combined output. Or preview the file with `quarto preview`.

> [!IMPORTANT]  
> **All** Quarto files in the repository are rendered in the `output/` directory when pushing on `main`.

## License

This repository is licensed under the MIT License.
