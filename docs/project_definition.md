# Chunk Auditor Project Definition

## 1. Identify the Problem

Our production media server is regularly under storage pressure and frequently approaches its available capacity. This creates an ongoing operational problem because the server holds active projects, source footage, renders, design assets, and archived production materials that the studio may still need to access.

One contributing cause is the accumulation of exact duplicate files across the server. In particular, large source-media files—such as 8K RED camera footage—may be copied into multiple folders during media imports, project migrations, manual backups, or other production workflows. These duplicate copies can consume a substantial amount of storage while remaining difficult to identify through normal file browsing.

At present, there is no efficient, reliable, or low-risk process for locating exact duplicate files across the storage server. Manually comparing filenames, file sizes, or folder structures is time-consuming and unreliable, especially when files may have different names or exist in unrelated project directories. As a result, duplicate storage remains a persistent issue without a clear way to measure its scale or provide actionable information for cleanup decisions.

Chunk Auditor is intended to address this visibility problem. The application will safely scan a selected storage location, identify files with identical contents, group those duplicate files together, and generate an audit report showing their locations and the amount of redundant storage they represent.

The application will not decide which files should be deleted or modify any files on the server. Its purpose is to provide trustworthy audit data so that storage cleanup decisions can be made deliberately by the appropriate people.