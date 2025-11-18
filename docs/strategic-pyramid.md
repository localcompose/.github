# Strategic Pyramid for locom

## Vision
Make local apps feel like real websites — private, simple, and reliable — without cloud complexity.  
*Inspired by Einstein’s principle: keep things “as simple as possible, but not simpler.”*  

## Mission
Provide a lightweight tool that hides port/IP hassle and gives Docker Compose apps clean domains and HTTPS locally, so even low-experience users can set up usable environments quickly.  

## Strategic Goal (MVP target)
Release a stable CLI that:  
- Ships with **3–6 pre-defined app stacks** ready to run out of the box.  
- Supports **minimal auto-setup** for a custom stack from a single Docker image.  
- (Optional extended metric): keep the time of initial single-stage setup scenario to **30–90 minutes** from installation to running a web app (depending on image download speed).  

## Key Strategy
Keep everything minimal and transparent: automate only the common-sense defaults, and always leave room for manual adjustment.  

## Tactic (Execution Focus)
- Develop CLI commands that “just work” for most setups.  
- Provide clear, short documentation for users who want to tweak manually.  
- Ensure domain/HTTPS setup is predictable and frictionless.  

---

## Mermaid Diagram

```mermaid
flowchart TD
    %% Vision
    subgraph V["Vision"]
        V1["Local apps as real websites — private, simple, reliable"]
        V2["Guiding principle: 'As simple as possible, but not simpler.'"]
    end

    %% Mission
    subgraph M["Mission"]
        M1["Lightweight tool"]
        M2["Hides port/IP hassle"]
        M3["Clean domains & HTTPS for local Docker Compose apps"]
        M4["Quick setup for low-experience users"]
    end

    %% Strategic Goal
    subgraph G["Strategic Goal (MVP Target)"]
        G1["Release stable CLI"]
        G2["Ship 3–6 predefined app stacks"]
        G3["Support minimal auto-setup for a custom stack (single image)"]
        G4["(Optional) Setup time: 30–90 min"]
    end

    %% Key Strategy
    subgraph S["Key Strategy"]
        S1["Keep everything minimal & transparent"]
        S2["Automate only common-sense defaults"]
        S3["Always allow manual adjustment"]
    end

    %% Tactics
    subgraph T["Tactics (Execution Focus)"]
        T1["CLI commands that 'just work'"]
        T2["Clear, short docs for manual tweaks"]
        T3["Predictable, frictionless domain & HTTPS setup"]
    end

    %% Connections
    V1 --> M1
    V2 --> M4

    M1 --> G1
    M2 --> G2
    M3 --> G3
    M4 --> G4

    G1 --> S1
    G2 --> S2
    G3 --> S2
    G4 --> S3

    S1 --> T1
    S2 --> T2
    S3 --> T3
```