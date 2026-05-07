# Organization Surface Map

## Purpose

This graph separates the Foundation institutional public surface from Alexandra Caussade, K-ussade, YOSO-YAi LLC, YOSOR, private operations, and release surfaces.

## Mermaid Diagram

```mermaid
flowchart LR
    subgraph PersonAndProof["Person and public technical proof surface"]
        alexandra["Alexandra Caussade<br/>person / Founder identity"]:::entity
        kussade["K-ussade<br/>public technical brand/account surface"]:::public
    end

    subgraph Foundation["218 Network Foundation"]
        foundation["218 Network Foundation<br/>civic institutional voice"]:::foundation
        website["218.network<br/>canonical public website"]:::foundation
        github["218-network GitHub org<br/>institutional public repo surface"]:::public
    end

    subgraph Company["Separate company/product surfaces"]
        company["YOSO-YAi LLC<br/>company voice / engineering partner"]:::entity
        yosor["YOSOR<br/>YOSO-YAi LLC product"]:::entity
    end

    subgraph Private["Non-public sources"]
        privateOps["Foundation private operations<br/>private/not-public"]:::private
        sealedIp["Sealed YOSO-YAi LLC IP<br/>private/not-public"]:::sealed
    end

    alexandra --> kussade
    foundation --> website
    foundation --> github
    company --> yosor
    company -. reviewed public partnership language only .-> foundation
    kussade -. proof navigation with status labels .-> github
    privateOps -. excluded .-> github
    sealedIp -. excluded .-> github

    classDef entity fill:#e7f0ff,stroke:#315a9f,color:#0f274d
    classDef foundation fill:#e8f5ee,stroke:#2b6b4d,color:#123526
    classDef public fill:#fff7df,stroke:#9a6a12,color:#332100
    classDef private fill:#f4e9ff,stroke:#70479c,color:#2f1749
    classDef sealed fill:#ffe8e8,stroke:#a33a3a,color:#4a1111
    classDef release fill:#e8f7ff,stroke:#277491,color:#12323e
    classDef workflow fill:#eef0f3,stroke:#58606b,color:#20242a
```

## Interpretation Notes

- The GitHub org is institutional Foundation infrastructure, not K-ussade and not a company namespace.
- K-ussade can point to the org as public proof navigation, but it does not speak as the institution.
- YOSO-YAi LLC and YOSOR are separate boundary references only.

## Boundary Notes

- Private operations and sealed company IP are excluded from public GitHub.
- Public repo publication does not imply live deployments, reports, schools, NEURONAs, datasets, models, or Spaces.

## Follow-Up Actions

- Keep the org profile and repo index synchronized after every repo status change.
- Add new institutional repos only after boundary and status review.
