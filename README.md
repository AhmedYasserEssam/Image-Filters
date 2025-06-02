# ImageFilters

## Overview

**ImageFilters** is a Windows Forms application developed in C# for applying advanced image filtering techniques to grayscale images. The application provides implementations of Alpha-Trimmed Mean and Adaptive Median filters, allowing users to experiment with different window sizes, trimming parameters, and sorting algorithms. It also features graphical visualization of algorithm performance using ZedGraph.

## Features

- **Open and Display Images:** Load and view grayscale images for processing.
- **Alpha-Trimmed Mean Filter:** Remove noise by trimming extreme values and averaging the rest, with selectable window size, trim parameter, and sorting algorithm (Counting Sort or Merge Sort).
- **Adaptive Median Filter:** Reduce impulse noise using an adaptive window, with selectable window size and sorting algorithm (Insertion Sort or Quick Sort).
- **Graph Visualization:** Visualize algorithm performance and complexity using integrated ZedGraph tools.
- **User-Friendly Interface:** Simple Windows Forms UI for easy parameter selection and result display.

## Technologies Used

- **C# (.NET Framework 3.0)**
- **Windows Forms**
- **ZedGraph** (for plotting and visualization)
- **Custom Image Processing Algorithms**

## Getting Started

### Prerequisites

- **Windows OS**
- **.NET Framework 3.0 or higher**
- **Visual Studio 2010 or later** (recommended for building and running the solution)

### Installation

1. **Clone the repository:**
   ```sh
   git clone <repository-url>
   ```
2. **Open the Solution:**
   - Open `ImageFilters.sln` in Visual Studio.

3. **Restore Dependencies:**
   - Ensure `ZedGraph.dll` and `ZGraphTools.dll` are present in `ZGraphTools/bin/Release/`.
   - If missing, build the `ZGraphTools` project first.

4. **Build the Solution:**
   - Set `ImageFilters` as the startup project.
   - Build the solution (`Build > Build Solution`).

5. **Run the Application:**
   - Start debugging (`F5`) or run without debugging (`Ctrl+F5`).

## Usage

1. **Open an Image:** Click the "Open" button and select a grayscale image.
2. **Select Filter and Parameters:** Choose the desired filter (Alpha-Trim or Median), set window size, trim parameter, and sorting type.
3. **Apply Filter:** Click the corresponding button to process the image.
4. **View Results:** The filtered image will be displayed. Use the graphing feature to visualize performance if desired.

## Project Structure

```
.
ImageFilters/
├── ImageFilters/           # Main application source code
│   ├── Form1.cs            # Main form and UI logic
│   ├── ImageOperations.cs  # Image processing algorithms
│   ├── Program.cs          # Application entry point
│   ├── Properties/         # Project properties and resources
│   ├── bin/                # Compiled binaries
│   └── obj/                # Intermediate build files
│
├── ZGraphTools/            # Graphing utilities and dependencies
│   ├── ZGraphForm.cs       # Graph form implementation
│   ├── ZGraphClass.cs      # Graph class implementation
│   ├── Properties/         # Project properties
│   ├── bin/                # Compiled binaries
│   └── obj/                # Intermediate build files
│
├── Samples/                # Sample images
├── ImageFilters.sln        # Visual Studio solution file
└── Image Filters.pdf       # Project documentation

```
## License

This project is for educational purposes.
