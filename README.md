# AccessibilityMonitoring

A comprehensive tool for monitoring and documenting accessibility compliance in buildings and facilities.

## Overview

AccessibilityMonitoring is a desktop application designed to help professionals assess and document accessibility standards in various types of buildings and facilities. The application provides a user-friendly interface for conducting accessibility audits, capturing photographic evidence, and generating comprehensive reports.

## Features

- **Visual Documentation**: Capture and organize photos by category (apartment, bathroom, kitchen, movement areas, territory)
- **Structured Assessment**: Systematic evaluation of accessibility features across different areas
- **Report Generation**: Create professional reports using customizable document templates
- **Project Management**: Organize assessments by location and date
- **User-Friendly Interface**: Built with PyQt5 for intuitive operation

## System Requirements

- Windows operating system
- No additional installation required (standalone executable)

## Installation

1. Download the AccessibilityMonitoring folder
2. Run `AccessibilityMonitoring.exe` to start the application
3. No additional setup required

## Usage

### Starting the Application

1. Navigate to the AccessibilityMonitoring folder
2. Double-click `AccessibilityMonitoring.exe`
3. The application will launch with the main interface

### Conducting an Assessment

1. Create a new project or open an existing one
2. Document findings by category:
   - **Apartment/Living Areas**: General living spaces accessibility
   - **Bathroom**: Bathroom accessibility features
   - **Kitchen**: Kitchen accessibility compliance
   - **Movement Areas**: Corridors, entrances, and pathways
   - **Territory**: External areas and building surroundings

3. Capture photos for each category using the built-in camera interface
4. Add notes and observations for each area
5. Generate reports when assessment is complete

### Managing Projects

- Projects are automatically saved in the `projects` folder
- Each project includes:
  - Assessment data in JSON format
  - Categorized photos in a dedicated subfolder
  - Metadata including location and date information

### Report Generation

- The application uses professional document templates (located in `_internal/docx/templates/`)
- Reports include:
  - Assessment summary
  - Categorized findings
  - Photo documentation
  - Compliance recommendations

## File Structure

```
AccessibilityMonitoring/
├── AccessibilityMonitoring.exe    # Main application
├── README.md                       # This file
├── _internal/                      # Application dependencies
│   ├── docx/templates/            # Report templates
│   └── img/                       # Application images
├── img/                           # User interface images
└── projects/                      # Assessment projects
    └── [project_name]/
        ├── project_data.json      # Assessment data
        └── photos/                # Project photos
```

## Photo Categories

The application organizes documentation into the following categories:

- **Apartment**: Living spaces, bedrooms, general areas
- **Bathroom**: Toilets, sinks, bathing facilities, grab bars
- **Kitchen**: Counters, appliances, storage accessibility
- **Movement**: Doorways, corridors, ramps, stairs
- **Territory**: Parking, entrances, outdoor pathways

## Technical Details

- **Framework**: Python with PyQt5 GUI
- **Document Processing**: python-docx for report generation
- **Image Handling**: PIL (Python Imaging Library)
- **Data Storage**: JSON format for project data
- **Deployment**: PyInstaller for standalone executable

## Supported Standards

The application is designed to help assess compliance with:
- ADA (Americans with Disabilities Act) guidelines
- Local accessibility building codes
- International accessibility standards
- Custom organizational requirements

## Troubleshooting

### Common Issues

1. **Application won't start**: Ensure all files in the `_internal` folder are present
2. **Photos not saving**: Check write permissions in the projects folder
3. **Report generation fails**: Verify document templates are intact

### Getting Help

- Check that all application files are in the same directory
- Ensure the `_internal` folder contains all necessary dependencies
- Verify that the `projects` folder exists and is writable

## Data Privacy

- All data is stored locally on your computer
- No information is transmitted to external servers
- Photos and assessment data remain under your control

## Version Information

- Application uses Python 3.10
- Built with PyQt5 for cross-platform compatibility
- Includes modern document processing capabilities



