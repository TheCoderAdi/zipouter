# zipouter

[![npm version](https://img.shields.io/npm/v/zipouter.svg)](https://www.npmjs.com/package/zipouter)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

A simple npm package to extract and process the contents of a zip file.

## Installation

```bash
npm install zipouter
```

## Additional Package to Install

```bash
npm install adm-zip
```

## Usage

```javascript
const { extractAndProcessZip } = require("zipouter");
or;
import { extractAndProcessZip } from "zipouter";

const zipFileName = "your-zip-file.zip";

extractAndProcessZip(zipFileName)
  .then((results) => {
    console.log("Compilation Results:", results);
  })
  .catch((error) => {
    console.error("Error:", error.message);
  });
```

## Important

Before proceeding further, ensure that you have Java, Node.js, and Python installed on your local machine. You can download and install them from the official websites:

- [Java](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Node.js](https://nodejs.org/)
- [Python](https://www.python.org/)

## Features

- Extract and process zip files.
- Support for multiple programming languages, including Java, JavaScript, Python, and more.

## API Reference

### `extractAndProcessZip(zipFileName: string): Promise<CompilationResult[]>`

Extracts and processes the contents of a zip file.

- `zipFileName`: The name of the zip file to process.

Returns a promise that resolves to an array of `CompilationResult` objects.

#### `CompilationResult`

- `fileName`: Name of the processed file.
- `output`: Compilation output or error message.

## Supported Languages

- **Java**: Files with a `.java` extension.
- **JavaScript**: Files with a `.js` extension.
- **Python**: Files with a `.py` extension.

## Example

# 0.First upload your zip file in the current directory <br/>

![image](https://github.com/TheCoderAdi/zipouter/assets/111285422/ff3118b7-9614-490c-b0ca-3aeb40dc6ea9)

# 1.import and use the extractAndProcessZip from zipouter

```javascript
import { extractAndProcessZip } from "zipouter";

const zipFileName = "example.zip";
extractAndProcessZip(zipFileName)
  .then((results) => {
    console.log("Compilation Results:", results);
  })
  .catch((error) => {
    console.error("Error:", error);
  });
```

# 2.Output<br/>

![image](https://github.com/TheCoderAdi/zipouter/assets/111285422/e322047e-5e68-4a86-a79a-19c5ce196cb9)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Issues

If you encounter any issues or have suggestions, please [open an issue on GitHub](https://github.com/TheCoderAdi/zipouter/issues).
