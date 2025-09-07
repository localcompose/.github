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
    end

    %% Mission
    subgraph M["Mission"]
        M1["Remove local dev friction (ports, IPs, certs)"]
        M2["Enable fast & usable environments for any user level"]
    end

    %% Strategic Goal
    subgraph G["Strategic Goal (MVP Target)"]
        G1["Deliver stable CLI"]
        G2["3–6 predefined app stacks"]
        G3["Minimal custom stack setup from one image"]
        G4["(Optional) Setup time: 30–90 min"]
    end

    %% Key Strategy
    subgraph S["Key Strategy"]
        S1["Stay minimal & transparent"]
        S2["Automate defaults only"]
        S3["Always allow manual adjustment"]
    end

    %% Tactics
    subgraph T["Tactics (Execution Focus)"]
        T1["CLI commands that 'just work'"]
        T2["Concise docs for tweaks"]
        T3["Predictable, frictionless HTTPS/domains"]
    end

    %% Connections
    V1 --> M1
    V1 --> M2

    M1 --> G1
    M1 --> G2
    M1 --> G3
    M2 --> G4

    G1 --> S1
    G2 --> S2
    G3 --> S2
    G4 --> S3

    S1 --> T1
    S2 --> T2
    S3 --> T3

```