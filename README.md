# Chunk Auditor

Chunk Auditor is a read-only Python utility for auditing production storage and identifying exact duplicate files.

It is designed for motion graphics and post-production environments where large source media, project assets, renders, and backups can accumulate across shared storage.

## Core safety guarantee

Chunk Auditor never deletes, moves, renames, overwrites, or modifies scanned files. It only reads file metadata and contents needed to identify exact duplicates, then generates audit reports.

## Status

Planning and technical-design phase.