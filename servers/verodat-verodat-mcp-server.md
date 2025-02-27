---
type: server
repo_url: https://github.com/Verodat/verodat-mcp-server
name: Verodat
owner: Verodat
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/data-analysis"]
---

#status/active #status/official #category/data-analysis

# Verodat

## Description

Interact with Verodat AI Ready Data platform. This MCP server provides integration with Verodat's platform for preparing and managing AI-ready datasets.

## Features

- Data preparation for AI
- Dataset management
- Data validation
- Data transformation
- Quality assurance
- Version control
- Metadata management
- Data lineage tracking
- Collaboration tools
- AI model integration

## Installation

```bash
npm install @verodat/mcp-server
```

## Usage

```javascript
import { VerodatServer } from "@verodat/mcp-server";

const server = new VerodatServer({
  apiKey: "your-verodat-api-key",
  workspace: "your-workspace",
});

// Prepare dataset for AI
const dataset = await server.prepareDataset({
  source: "./raw_data.csv",
  name: "training_dataset",
  options: {
    validate: true,
    cleanMissing: true,
    normalizeValues: true,
    addMetadata: true,
  },
});

// Transform data
const transformedData = await server.transform({
  datasetId: dataset.id,
  operations: [
    {
      type: "normalize",
      columns: ["feature1", "feature2"],
    },
    {
      type: "encode",
      columns: ["category1"],
      method: "one-hot",
    },
    {
      type: "split",
      ratio: {
        train: 0.7,
        validation: 0.15,
        test: 0.15,
      },
    },
  ],
});

// Validate data quality
const validation = await server.validateQuality({
  datasetId: dataset.id,
  rules: [
    {
      type: "completeness",
      threshold: 0.95,
    },
    {
      type: "consistency",
      columns: ["id", "email"],
      unique: true,
    },
    {
      type: "distribution",
      column: "age",
      distribution: "normal",
      parameters: {
        mean: [0, 100],
        std: [5, 20],
      },
    },
  ],
});

// Track data lineage
const lineage = await server.trackLineage({
  datasetId: dataset.id,
  includeTransformations: true,
  includeValidations: true,
  format: "graph",
});
```

## Dependencies

- Node.js >= 14.x
- Verodat account
- Verodat API key
- Active workspace

## Related Servers

- None currently listed
