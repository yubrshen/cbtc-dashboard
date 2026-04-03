# AGENTS.md - Splunk Dashboard Development Guide

## Project Context
This project develops Splunk dashboards in Simple XML format for CBTC Dashboard.

## Guidelines for Agent Operations

### 1. XML Formatting
- Format all `.xml` files per standard XML conventions (proper indentation, closing tags, etc.)

### 2. File Organization
- **Generated documents**: Place in `./by-amp/` subdirectory
- **Other generated files**: Place in appropriately named folders (e.g., `src-python/`, `src-scripts/`, etc.)
- `.xml` files: Place in root directory

### 3. Dashboard Development Practices
- Use base queries whenever possible and appropriate
- Avoid unnecessary complexity in search logic

### 4. Code Deployment
- Generated code will NOT be directly executed by the agent
- The user will copy generated code to another host for testing
- No need to validate functionality through execution

### 5. Documentation Standards
- Document all changes
- Keep documentation high-level with minimal noise
- Focus on what changed and why, not excessive detail
