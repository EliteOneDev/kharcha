# Graph Report - kharcha  (2026-10-15)

## Corpus Check
- Corpus is ~28,199 words - fits in a single context window. You may not need a graph.

## Summary
- 461 nodes · 1182 edges · 22 communities (19 shown, 3 thin omitted)
- Extraction: 97% EXTRACTED · 3% INFERRED · 0% AMBIGUOUS · INFERRED: 31 edges (avg confidence: 0.88)
- Token cost: 75,104 input · 0 output

## Community Hubs (Navigation)
- Mobile Screens & UI Kit
- Project Docs & Architecture
- SQLite Ledger & Data Model
- Backup API Server
- API Package Manifest
- Expo App Config
- Mobile Expo Dependencies
- Mobile Package Metadata
- Web Storage Fallback
- Encrypted Backup Client
- Bank SMS Parser
- API TypeScript Config
- App Root Layout
- Native SMS Module
- Brand Asset Generator
- Mobile npm Scripts
- Mobile TypeScript Config
- ESLint Config
- Mobile Dev Dependencies
- Repository Metadata
- Node Engine Pin

## God Nodes (most connected - your core abstractions)
1. `usePalette()` - 46 edges
2. `showMessage()` - 29 edges
3. `useLedger()` - 27 edges
4. `Screen()` - 26 edges
5. `ScreenHead()` - 26 edges
6. `Action()` - 24 edges
7. `Body()` - 22 edges
8. `react-native` - 21 edges
9. `Caption()` - 21 edges
10. `react` - 20 edges

## Surprising Connections (you probably didn't know these)
- `CI Workflow` --semantically_similar_to--> `Build and Verify Sequence`  [INFERRED] [semantically similar]
  .github/workflows/ci.yml → README.md
- `Feature Request Template` --references--> `Kharcha`  [INFERRED]
  .github/ISSUE_TEMPLATE/feature_request.md → README.md
- `Continuous Native Generation (no hand-edited ios/android)` --conceptually_related_to--> `KharchaSms Native Expo Module`  [INFERRED]
  mobile/AGENTS.md → README.md
- `Contributing Guide` --references--> `Bug Report Template`  [EXTRACTED]
  CONTRIBUTING.md → .github/ISSUE_TEMPLATE/bug_report.md
- `Redact SMS Personal Details in Bug Reports` --conceptually_related_to--> `On-Device SMS Parser (mobile/src/lib/parser.ts)`  [INFERRED]
  .github/ISSUE_TEMPLATE/bug_report.md → README.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **SMS-to-Ledger-to-Encrypted-Backup Data Flow** — readme_kharchasms_native_module, readme_on_device_sms_parser, readme_review_inbox, readme_local_sqlite_ledger, readme_backup_encryption_module, readme_render_backup_api, render_kharcha_backups_database [EXTRACTED 1.00]
- **Contributor Onboarding Documentation Set** — contributing_contributing_guide, code_of_conduct_contributor_covenant, security_security_policy, _github_issue_template_bug_report_bug_report_template, _github_issue_template_feature_request_feature_request_template, _github_pull_request_template_pull_request_template, _github_workflows_ci_ci_workflow [EXTRACTED 1.00]
- **Backup API Security Controls** — security_untrusted_input_validation, security_constant_time_comparison, security_zero_knowledge_boundary, contributing_api_input_validation, privacy_zero_knowledge_backup [INFERRED 0.85]

## Communities (22 total, 3 thin omitted)

### Community 0 - "Mobile Screens & UI Kit"
Cohesion: 0.10
Nodes (81): Backup(), run(), BudgetEditor(), save(), ImportSms(), parse(), save(), Manual() (+73 more)

### Community 1 - "Project Docs & Architecture"
Cohesion: 0.07
Nodes (36): Bug Report Template, Feature Request Template, PR Contributor Checklist (single concern, no secrets, privacy impact), Pull Request Template, CI api job (typecheck, test, build), CI Workflow, CI mobile job (lint, typecheck, test), Changelog (+28 more)

### Community 2 - "SQLite Ledger & Data Model"
Cohesion: 0.14
Nodes (37): KharchaSmsModule, addTransaction(), editTransaction(), exportSnapshot(), fromRow(), getDatabase(), listBudgets(), listSenders() (+29 more)

### Community 3 - "Backup API Server"
Cohesion: 0.08
Nodes (16): authorized(), BackupPayload, buildApp(), validBackup(), app, origins, port, shutdown() (+8 more)

### Community 4 - "API Package Manifest"
Cohesion: 0.06
Nodes (31): bugs, dependencies, fastify, pg, devDependencies, tsx, @types/node, @types/pg (+23 more)

### Community 5 - "Expo App Config"
Cohesion: 0.06
Nodes (31): backgroundColor, backgroundImage, foregroundImage, monochromeImage, adaptiveIcon, package, permissions, predictiveBackGestureEnabled (+23 more)

### Community 6 - "Mobile Expo Dependencies"
Cohesion: 0.09
Nodes (22): dependencies, expo, expo-clipboard, expo-constants, expo-crypto, expo-font, @expo-google-fonts/bricolage-grotesque, @expo-google-fonts/hanken-grotesk (+14 more)

### Community 7 - "Mobile Package Metadata"
Cohesion: 0.11
Nodes (17): bugs, homepage, typescript, license, main, name, private, version (+9 more)

### Community 8 - "Web Storage Fallback"
Cohesion: 0.25
Nodes (17): addTransaction(), editTransaction(), empty(), exportSnapshot(), getDatabase(), listBudgets(), listSenders(), listTransactions() (+9 more)

### Community 9 - "Encrypted Backup Client"
Cohesion: 0.24
Nodes (14): apiUrl, Credentials, decodeRecoveryCode(), deleteRemoteBackup(), downloadBackup(), enableBackup(), endpoint(), getCredentials() (+6 more)

### Community 10 - "Bank SMS Parser"
Cohesion: 0.23
Nodes (10): categoryFor(), contextualAmountPatterns, isTransactionMessage(), merchantPatterns, parseBankSms(), titleCase(), transactionAmount(), transactionConfidence() (+2 more)

### Community 11 - "API TypeScript Config"
Cohesion: 0.18
Nodes (10): compilerOptions, esModuleInterop, module, moduleResolution, outDir, rootDir, skipLibCheck, strict (+2 more)

### Community 12 - "App Root Layout"
Cohesion: 0.22
Nodes (9): Index(), RootLayout(), LoadingScreen(), expo-font, @expo-google-fonts/bricolage-grotesque, @expo-google-fonts/hanken-grotesk, @expo-google-fonts/ibm-plex-mono, expo-status-bar (+1 more)

### Community 14 - "Brand Asset Generator"
Cohesion: 0.31
Nodes (4): cover(), ticket(), txt(), xy()

### Community 15 - "Mobile npm Scripts"
Cohesion: 0.22
Nodes (9): scripts, android, check, ios, lint, start, test, typecheck (+1 more)

### Community 16 - "Mobile TypeScript Config"
Cohesion: 0.29
Nodes (6): compilerOptions, paths, strict, extends, include, expo/tsconfig.base

### Community 17 - "ESLint Config"
Cohesion: 0.40
Nodes (4): { defineConfig }, expoConfig, eslint, eslint-config-expo

### Community 18 - "Mobile Dev Dependencies"
Cohesion: 0.40
Nodes (5): devDependencies, eslint, eslint-config-expo, @types/react, typescript

### Community 19 - "Repository Metadata"
Cohesion: 0.50
Nodes (4): repository, directory, type, url

## Knowledge Gaps
- **19 isolated node(s):** `@types/node`, `@types/pg`, `tsx`, `typescript`, `expo-constants` (+14 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 171 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `parseBankSms()` connect `Bank SMS Parser` to `Mobile Screens & UI Kit`, `SQLite Ledger & Data Model`?**
  _High betweenness centrality (0.084) - this node is a cross-community bridge._
- **What connects `@types/node`, `@types/pg`, `tsx` to the rest of the system?**
  _19 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `Mobile Screens & UI Kit` be split into smaller, more focused modules?**
  _Cohesion score 0.09839432412247946 - nodes in this community are weakly interconnected._
- **Why does `dependencies` connect `Mobile Expo Dependencies` to `Mobile Package Metadata`?**
  _High betweenness centrality (0.066) - this node is a cross-community bridge._
- **Should `Project Docs & Architecture` be split into smaller, more focused modules?**
  _Cohesion score 0.07180851063829788 - nodes in this community are weakly interconnected._
- **Why does `react-native` connect `Mobile Screens & UI Kit` to `SQLite Ledger & Data Model`, `App Root Layout`, `Mobile Package Metadata`?**
  _High betweenness centrality (0.054) - this node is a cross-community bridge._
- **Should `SQLite Ledger & Data Model` be split into smaller, more focused modules?**
  _Cohesion score 0.14396456256921372 - nodes in this community are weakly interconnected._