# Useful Node.js Scripts

Welcome to the **Useful Node.js Scripts** repository! This collection features a variety of scripts that can help you streamline your Node.js development workflow, automate tasks, and enhance your productivity.

## Table of Contents

- [Getting Started](#getting-started)
- [Scripts](#scripts)
  - [Script 1: Generate a Secure Random String](#script-1-generate-a-secure-random-string)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

To use these scripts, make sure you have Node.js installed on your machine. You can download Node.js from [here](https://nodejs.org/).

1. Clone this repository:
   ```bash
   git clone https://github.com/TomoyaKuroda/useful-nodejs-scripts.git
   ```
   
2. Navigate into the cloned repository:
   ```bash
   cd useful-nodejs-scripts
   ```

## Scripts

### Script 1: Generate a Secure Random String

**NPM Script**: `"generate-secure-key"`

**Description**: This script generates a secure, random 32-byte string encoded in Base64. This is useful for creating secure tokens, passwords, or keys for encryption.

**NPM Script Configuration**:
You can add the following script to your `package.json` under the `scripts` section:
```json
"scripts": {
  "generate-secure-key": "node -e \"console.log(require('crypto').randomBytes(32).toString('base64'))\""
}
```

**Usage**:
To generate a secure key, simply run the following command in your terminal:
```bash
npm run generate-secure-key
```

**Explanation**:
- The script uses Node.js's built-in `crypto` module to generate 32 random bytes.
- These bytes are then converted to a Base64-encoded string, which is printed to the console.
- This string can be used in your application wherever a secure, random value is needed, such as for generating API keys, authentication tokens, or encryption keys.

## Contributing

Contributions are welcome! If you have a useful Node.js script you'd like to add or improve upon, feel free to open a pull request. Please ensure your contributions adhere to the existing style and structure of the repository.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.