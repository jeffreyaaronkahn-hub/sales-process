flowchart LR

%% =========================
%% STEP 1: PRE-SALE
%% =========================
PRE1[Step1: Client Identification] --> PRE2[Identify Target List: SSO SBL / RR Client / CAM Warm List]
PRE2 --> PRE3[Determine Best Contact]
PRE3 --> PRE4[Outreach: SSO SBL / TPM / CAM Set Up Call]
PRE4 --> PRE5[Sales Specialist Creates New Business Opportunity in Salesforce]
PRE5 --> PRE6[Add Campaign to Opportunity & Update Dashboard]
PRE6 --> PRE7[Initial Sales Call Led by Sales Specialist, Supported by SSO SBL/TPM/CAM]
PRE7 --> PRE8[Send Landing Page for Pilot Opt-In]
PRE8 --> PRE9[Landing Page Executed (Execution Date Captured)]
PRE9 --> PRE10[Jeff Kahn Notified, Forwards to Sales Specialist for Close-Won]

%% =========================
%% STEP 2: PILOT
%% =========================
PIL1[Create New Salesforce Opportunity: Type = Upsell] --> PIL2[3-Month Pilot Period Starts on Execution Date]
PIL2 --> PIL3[Sales Specialist Accountable for Conversion]
PIL2 --> PIL4[SSO SBL Coordinates Services & Supports Sales Specialist]
PIL2 --> PIL5[ACV Team Owns Delivery, Support, Reporting]
PIL2 --> PIL6[Recurring Client Calls Led by ACV, Sales Specialist & SBL Build Relationship]

%% =========================
%% DECISION GATE: Convert to Multi-Year?
%% =========================
PIL6 --> DEC{Convert to Multi-Year?}

%% YES PATH
DEC -->|Yes| POST1[Client Opts into 3-Year Term ($30k/yr)]
POST1 --> POST2[Opt-In Uses Same T&Cs as Landing Page]
POST2 --> POST3[Multi-Year Agreement Active]
POST3 --> POST4[Solutions Consulting (Ashish Gupta) Primary Support]
POST3 --> POST5[ACV Provides Support as Needed]
POST3 --> POST6[Sales Specialist & SBL Support as Needed]

%% NO PATH
DEC -->|No| POST7[ACV Role Ends]
POST7 --> POST8[BAU Sales Motion]
POST8 --> POST9[Sales Specialist Continues Engagement]
POST8 --> POST10[SSO SBL Continues Relationship Management]
