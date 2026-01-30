# Sales Lifecycle – Pre-Sale, Pilot, Post-Conversion

This document describes the end-to-end sales process from
client identification through pilot, conversion, and BAU sales.

---

## Step 1: Pre-Sale
**Goal:** Identify target clients and secure pilot opt-in  
**Primary Owner:** Sales Specialist

---

## Step 2: Pilot
**Duration:** 3 months  
**Start Date:** Landing page execution date  
**Primary Owner:** ACV (delivery), Sales Specialist (conversion)

---

## Step 3: Post-Conversion
**Outcome:** Multi-year agreement or BAU sales motion

---

## Process Flow

```mermaid
flowchart LR
flowchart LR

%% ======================================================
%% STEP 1 – PRE-SALE
%% ======================================================
subgraph STEP1[Step 1: Pre-Sale]
    A[Client Identification] --> A1{Source of Target List}

    A1 -->|SSO SBL| B1[SSO SBL Identifies Client<br/>Has Relationship / Contact]
    A1 -->|Current RR Client List| B2[Known RR Client<br/>Known Contact]
    A1 -->|CAM Warm Client List| B3[ADR Identifies Right Contact<br/>at Company]

    B1 --> C1[SSO SBL Sets Up Call]
    B2 --> C2[TPM Sets Up Call]
    B3 --> C3[CAM Receives Contact + Blurb<br/>CAM Sets Up Call]

    C1 --> D[Call Scheduled]
    C2 --> D
    C3 --> D

    D --> E[Sales Specialist Creates New Business Opportunity<br/>in Risk Recon Salesforce]

    E --> E1[Campaign Added<br/>(Mandatory – Same for All Opportunities)]
    E --> E2[Dashboard Updated<br/>Visible to SSO SBLs & CAMs]

    E --> F[Initial Sales Call]
    F --> F1[Sales Specialist Leads Call<br/>Support from SSO SBL / TPM / CAM]

    F --> G[Sales Specialist Sends Landing Page<br/>for Pilot Opt-In]

    G -->|Client Executes| H[Landing Page Executed<br/>(Execution Date Captured)]

    H --> H1[Execution Date = Pilot Start Date]
    H --> H2[Jeff Kahn Notified]
    H2 --> H3[Jeff Kahn Forwards to Sales Specialist]
    H3 --> H4[Sales Specialist Close-Won<br/>New Business Opportunity]
end

%% ======================================================
%% STEP 2 – PILOT
%% ======================================================
subgraph STEP2[Step 2: Pilot]
    H1 --> I[Create Salesforce Opportunity<br/>Type: Upsell]

    I --> J[3-Month Pilot Period<br/>Clock Starts on Execution Date]

    J --> J1[Sales Specialist<br/>Accountable for Conversion]
    J --> J2[SSO SBL<br/>Coordinates Services & Supports Sales]
    J --> J3[ACV Team<br/>Owns Delivery, Support, Reporting]

    J --> J4[Recurring Client Calls<br/>Led by ACV]
end

%% ======================================================
%% PILOT DECISION GATE
%% ======================================================
J --> M{Convert to Multi-Year?}

%% ======================================================
%% STEP 3 – POST-CONVERSION
%% ======================================================
subgraph STEP3[Step 3: Post-Conversion]

    %% YES PATH
    M -->|Yes| K[Client Opts into 3-Year Term<br/>$30k / Year]
    K --> K1[Opt-In Uses Same T&Cs<br/>as Landing Page]

    K --> L[Multi-Year Agreement Active]
    L --> L1[Solutions Consulting (Ashish Gupta)<br/>Primary Client Support]
    L --> L2[ACV Supports as Needed]
    L --> L3[Sales Specialist & SBL<br/>Support as Needed]

    %% NO PATH
    M -->|No| N[ACV Role Ends]
    N --> O[BAU Sales Motion]
    O --> O1[Sales Specialist Continues Engagement]
    O --> O2[SSO SBL Continues Relationship Management]
end

