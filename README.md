# VC Queries

A set of SPARQL queries for working with Verifiable Credentials (VCs) generated by [@jeswr/vc-cli](https://github.com/jeswr/vc-cli).

## Installation

```bash
npm install @jeswr/vc-queries
```

## Usage

This package provides a collection of SPARQL queries that can be used to query Verifiable Credentials. The queries are designed to work with the output format of the @jeswr/vc-cli tool.

### Available Queries

The package includes the following queries:

- `can-drive.rq`: Query to check driving permissions

### Running Queries

You can run queries using the following command:

```bash
npm run query
```

This will execute the default query (can-drive.rq) against the collected.ttl file.

### Generating Test Data

To generate test data and run the queries:

```bash
npm run test
```

This will:
1. Generate test VCs using vc-cli
2. Collect them into a single TTL file
3. Run the queries against the collected data

## Development

### Prerequisites

- Node.js
- npm
- @jeswr/vc-cli

### Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

### Adding New Queries

1. Create a new `.rq` file in the `queries` directory
2. Add your SPARQL query
3. Update the package.json scripts if you want to add a specific command for your query

## License

MIT © [Jesse Wright](https://github.com/jeswr/) 