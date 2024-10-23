# CSV to JSON Glossary Converter

This project is a simple web-based tool for converting CSV files into a structured JSON format. It provides an easy way for users to upload a CSV, map the language codes, and generate a JSON file, all without needing any backend services. The project uses HTML, JavaScript, and the PapaParse library to make the CSV parsing straightforward.

## Features

- Upload CSV File: Users can upload a CSV file that contains terms and their translations.

- Language Code Mapping: The tool automatically detects the language codes from the CSV and allows the user to map them to predefined language codes or add new ones if needed.

- Guess "kind" Field: The tool guesses whether a term is a "name" or a "general" term based on capitalization rules.

- Download JSON: After processing the CSV, users can download the resulting JSON file with all the mapped translations.

## How to Use

- Upload a CSV File: Click on the "Choose File" button to select a CSV file from your computer. The CSV should have a column named en representing the English term, and other columns representing translations in different languages.

- Map Language Codes: After uploading, you can map the detected language codes from the CSV to the standard language codes provided. If a language code isn't listed, you can add a new one.

- Download JSON: Once everything is mapped, click the "Download JSON" button to generate and download the translated terms as a JSON file.

## File Structure

- HTML File: The main HTML file (index.html) contains the structure and logic for the tool.

- JavaScript: Embedded in the HTML file, the JavaScript handles file parsing, language code mapping, and JSON generation using the PapaParse library.

- CSS: The layout is styled using Bootstrap to ensure a simple and user-friendly interface.

## Dependencies

- PapaParse: Used to parse CSV files directly in the browser.

- Bootstrap: Used for styling the UI components to make them clean and responsive.


## Example CSV Format

The CSV should have the following format:

```
en,ar,fr,de
Account,الحساب,Compte,Konto
Add-on,إضافة,Add-on,Add-on
```
en: The English term.

Other columns (ar, fr, de, etc.) represent translations in respective languages.

## Development

To make changes to the project:

- Clone the repository.

- Open index.html in your favorite code editor.

- Modify the HTML, JavaScript, or CSS as needed.

- To test locally, simply open the HTML file in your browser.

## License

This project is licensed under the MIT License.

