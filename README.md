# Lesson Template Repository

This repository is a template for creating lessons based on Quarto files. Each file in the `lecture/`, `tutorial/` and `practicum/` directories is a separate lesson. Alternatively you can use a git submodule containing all your modules, set up as `Lessons-modules` in this template.

## Directory Structure

- `Lessons-modules`: Contrains all modules in an external repository.
- `Lessons-assets`: Contains all assets used in the modules and lessons.
- `lecture/`: Contains individual lessons.
- `tutorial/`: Contains individual tutorials.
- `practicum/`: Contains individual practicum.
- `scripts/`: Contains custom JavaScript or R scripts.
- `output/`: Contains the final combined output files.

## How to Add a New Module

1. Create a new Quarto file in the `lecture/`, `tutorial/` or `practicum/` directory.
2. Add a reference to the new module in the global Quarto file.

> [!NOTE]  
> You can indicate assets path as if you were in the root folder.

## How to Generate the Combined Output

1. Open the global Quarto file.
2. Render the file with `quarto render _filename_` to generate the combined output. Or preview the file with `quarto preview`.

> [!IMPORTANT]  
> **All** Quarto files in the repository are rendered in the `output/` directory when pushing on `main`. Only the submodules in `Lessons-modules` are not rendered.

## License

This repository is licensed under the MIT License.
