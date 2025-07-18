# Communication Knowledge Graph Challenge

Welcome to the Communication Knowledge Graph challenge!

## The Challenge

Build an intelligent system that analyzes business communications to automatically discover entities, relationships, and evolving concepts. Transform scattered email conversations into a structured knowledge graph that reveals hidden patterns and connections.

## What You'll Build

Your system should:

- **Extract entities** (people, companies, projects, concepts) from communications
- **Map relationships** between entities and how they interact
- **Track evolution** of entities and relationships over time
- **Provide provenance** showing which communications support each insight

## Input Data

You'll work with realistic mock business communications covering:

- Investment due diligence discussions
- Partnership development conversations
- Team expansion and hiring communications
- Cross-cutting topics that span multiple threads

The dataset includes 18 interconnected emails that reference the same entities across different contexts and timeframes.

## Technical Requirements

### Core Functionality

1. **Entity Extraction**: Identify and classify key entities across all communications
2. **Relationship Mapping**: Detect connections and interactions between entities
3. **Timeline Construction**: Show how entities and relationships evolve chronologically
4. **Source Attribution**: Track which specific communications mention each entity/relationship

### Expected Output

Your solution must produce valid JSON containing at minimum:

- **Entities**: Including name, type, confidence score, and source references
- **Relationships**: Including source/target entities, relationship type, confidence, and evidence
- **Timeline**: Chronological events showing how entities and relationships evolve

The output should demonstrate clear source attribution - every insight must be traceable back to specific communications.

## Technology Requirements

- **Language**: Python (required - must match our stack)
- **Package Management**: We recommend using [uv](https://github.com/astral-sh/uv) for fast, reliable dependency management
- **LLM Integration**: Any provider (e.g., LiteLLM supports multiple providers including local models via Ollama)
- **Optional frameworks**:
  - DSPy for structured prompting
  - Pydantic for type-safe data structures
  - Any other libraries that help demonstrate your approach

## Evaluation Criteria

### Primary Focus Areas

1. **Problem Decomposition** (25%): How you break down this complex challenge
2. **LLM Integration** (30%): Quality of prompts and structured outputs
3. **Data Architecture** (25%): Clean entity/relationship modeling with source attribution
4. **Code Quality** (20%): Readable, organized, testable implementation

### Bonus Points

- **Confidence Scoring**: Thoughtful uncertainty quantification
- **Entity Resolution**: Handling name variations ("John Smith" vs "John")
- **Performance Optimization**: Efficient processing and caching strategies
- **Business Insights**: Meaningful analysis beyond raw extraction

## Success Examples

### Strong Implementation

- Extracts 10-15 entities with reasonable accuracy
- Identifies 15-20 meaningful relationships
- Provides clear source attribution for all insights
- Handles basic entity resolution and confidence scoring
- Clean, well-documented code structure

### Exceptional Implementation

- Sophisticated entity resolution across name variations
- Infers implicit relationships beyond direct mentions
- Tracks sentiment evolution in relationships over time
- Optimizes for performance with larger datasets
- Generates valuable business insights from the graph

## Deliverables

### Required

- **Working application** that processes the provided communications
- **Knowledge graph output** in valid JSON format
- **README documentation** explaining your approach, setup instructions, and how to run
- **Example output** from running your solution on the provided data

### Optional

- **Unit tests** for core functionality
- **Visualization** of the knowledge graph
- **Performance analysis** and optimization notes
- **Extended analysis** beyond basic requirements

## Submission Guidelines

1. **Clone this repo** using the "Use this template" button at the top right
2. **Create a new private repository** from the template
3. **In your repo settings**, add `tomwhale` and `MAlGIaT` as collaborators
4. **Build your solution** in the private repo
5. **Include in your submission**:
   - Complete working code
   - Clear README with setup and execution instructions
   - Example output from processing the provided dataset
   - Any additional documentation about your approach