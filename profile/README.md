## NextGen Architecture solution: Evolution you architecture in programming way.

- [x] [ArchGuard](https://github.com/archguard/archguard) - ArchGuard backend, scan and analysis source code, feed to server.
- [x] [ArchGuard frontend](https://github.com/archguard/archguard-frontend) - visualization results & dashboard

```mermaid
sequenceDiagram
    Frontend->>Backend: create system with system info (like Git/SVN)
    Backend-->>Scanner: system info

    activate Scanner
    
    Scanner-->>Analyser(Scanner): features
    Analyser(Scanner)-->>Linter(Scanner): rules

    Analyser(Scanner)-->>Scanner: model
    Scanner-->>Backend: results

    Linter(Scanner)-->>Scanner: issues
    Scanner-->>Backend: results
    
    deactivate Scanner

    Backend-->>Frontend: results
```
