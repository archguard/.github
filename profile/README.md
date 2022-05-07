## Evolution you architecture in programming way.

- [x] [ArchGuard](https://github.com/archguard/archguard) - connect scanner and show data.
- [x] [ArchGuard scanner](https://github.com/archguard/scanner/)  - scan source code, binary data and othes, and feed to database.
- [x] [ArchGuard frontend](https://github.com/archguard/archguard-frontend) - visualization results & dashboard

```mermaid
sequenceDiagram
    Frontend->>Backend: create system with system info (like Git/SVN)
    Backend-->>Scanner: system info
    Scanner-->>Analyser: features
    Scanner-->>Linter: rules
    Scanner-->>Backend: model
    Backend-->>Frontend: issues
```
