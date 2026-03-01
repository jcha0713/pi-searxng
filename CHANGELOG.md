# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.4] - 2025-03-01

### Changed
- Code cleanup: removed experimental query editor feature to maintain clean agent workflow.

## [1.0.3] - 2025-03-01

### Fixed
- Gist URLs (gist.github.com) are now fetched as regular web content instead of attempting to clone them as repositories.

## [1.0.2] - 2025-03-01

### Fixed
- GitHub blob and tree URLs now clone correctly. Previously, URLs like `github.com/owner/repo/blob/main/file.md` would fail because the full URL was passed to `git clone`. Now the URL is parsed to extract the owner, repo, and branch, and a clean clone URL is constructed.

## [1.0.1] - 2025-02-25

### Changed
- Updated package description and metadata

## [1.0.0] - 2025-02-25

### Added
- Initial release
- `web_search` tool - Search the web via SearXNG
- `fetch_content` tool - Extract article content from URLs
- `get_search_results` tool - Retrieve cached search results by ID
- Automatic GitHub repository cloning when fetching GitHub URLs
