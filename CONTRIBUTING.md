# Contributing to Document Search Engine

Thank you for your interest in contributing to the Document Search Engine project! This document provides guidelines and instructions to help you get started.

## Table of Contents
- [Development Environment Setup](#development-environment-setup)
  - [Prerequisites](#prerequisites)
  - [Installation on macOS M1](#installation-on-macos-m1)
  - [Project Setup](#project-setup)
- [Development Workflow](#development-workflow)
  - [Branch Naming Conventions](#branch-naming-conventions)
  - [Commit Message Guidelines](#commit-message-guidelines)
  - [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Testing Guidelines](#testing-guidelines)
- [Documentation](#documentation)

## Development Environment Setup

### Prerequisites

To contribute to this project, you'll need the following tools:

- macOS on Apple Silicon (M1 or newer)
- Homebrew (package manager)
- Java 17
- Maven
- Docker
- IntelliJ IDEA (recommended IDE)
- PostgreSQL

### Installation on macOS M1

1. **Install Homebrew**:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
2.  echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
3.  brew install openjdk@17
4.  sudo ln -sfn $(brew --prefix)/opt/openjdk@17/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk-17.jdk
5.  brew install maven
6.  brew install --cask docker
7.  brew install --cask intellij-idea-ce
8.  brew install postgresql@14
9.  brew services start postgresql@14
10.  createdb document_search_engine

### Development Workflow
Branch Naming Conventions

Feature branches: feature/short-description
Bug fixes: bugfix/issue-short-description
Documentation: docs/what-changed
Performance improvements: perf/what-improved
Refactoring: refactor/what-refactored

Example: feature/semantic-search-implementation
Commit Message Guidelines

Use the imperative mood: "Add feature" not "Added feature"
Start with a capital letter
Keep the first line under 50 characters
Reference issues where appropriate: "Add search pagination (fixes #123)"

### Pull Request Process

Ensure your code adheres to the coding standards
Update documentation to reflect any changes
Include tests that verify your changes
Ensure all tests pass locally before submitting
Update the README.md with details of significant changes
Title your PR clearly with the purpose of the changes
Link any relevant issues in the PR description

### Coding Standards

Follow Google Java Style Guide
Use meaningful variable and function names
Write clear comments for complex logic
Keep methods small and focused on a single responsibility
Use appropriate design patterns
Include Javadoc comments for public APIs

### Testing Guidelines

Write unit tests for all new features
Ensure test coverage is at least 80% for new code
Mock external dependencies (GCP, etc.) in tests
Write integration tests for critical paths
Name tests clearly: shouldDoSomethingWhenCondition

### Documentation

Update README.md for any user-facing changes
Document APIs using Swagger/OpenAPI
Include diagrams for architectural changes
Document environment variables and configuration options
Keep documentation in sync with code
