# jp-scripts

A collection of command-line utilities to streamline Git workflows and development processes.

## Overview

This repository contains a set of shell scripts designed to improve developer productivity by simplifying common Git operations, branch management, testing workflows, and pull request creation. Each script focuses on a specific task and can be used independently.

## Scripts

### 🌿 [branch](./branch/)
A Git branch searching and switching utility with intelligent pattern matching.

- Smart pattern matching for branch names, ticket numbers, or keywords
- Automatic switching when single match is found
- Remote branch fallback when no local matches exist
- Colorized output for better readability

### 🧪 [component](./component/)
A test runner utility for running component tests with enhanced debugging and coverage reporting.

- Watch mode testing that re-runs tests when files change
- Coverage reporting with lcov format
- Extended debug output for detailed logs
- Pattern matching for specific tests or components

### 🔄 [mergedev](./mergedev/)
A Git utility for efficiently merging the latest develop branch changes into your current branch.

- Fetches develop updates without switching branches
- Automatic merge commits with `--no-edit`
- Safety checks to prevent running on develop branch
- Clear feedback and error handling

### 📝 [pr](./pr/)
A GitHub Pull Request URL generator and browser opener utility.

- One-command PR creation - opens GitHub PR page instantly
- Smart repository detection from Git remote
- Configurable GitHub organization via environment variable
- Direct browser integration

### 📋 [recent](./recent/)
A Git utility for quickly viewing and switching to your most recent branches.

- Lists 20 most recent local Git branches
- Numbered interface for easy selection
- Quick branch switching by number
- Input validation and error handling

## Installation & Usage

Each script has detailed installation instructions and usage examples in its individual README file. Simply navigate to the script's folder for complete documentation.

For quick setup: make the script executable (`chmod +x scriptname`) and place it in your PATH.

## Prerequisites

- **Git** - All scripts require Git to be installed and configured
- **Node.js & npm** - Required for the `component` script
- **Web browser** - Required for the `pr` script to open GitHub URLs

## Help and Documentation

Each script includes built-in help:
```bash
scriptname --help     # or -h for detailed usage information
scriptname --version  # or -v for version information
```

For complete documentation, installation instructions, and usage examples, see the README in each script's folder.
