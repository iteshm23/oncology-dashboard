RISA Labs | Oncology Decision Support Dashboard (v1.0)

🏥 Project Overview

This dashboard is a clinician-first, read-only decision support prototype designed for the RISA Labs Technical APM Assignment.
Oncology workflows are hindered by fragmented data scattered across EHR tabs. This tool synthesizes genomics, longitudinal biomarkers, treatment arcs, and laboratory results into a single "White-Paper" interface. By prioritizing longitudinal trends over static values, the prototype aims to reduce cognitive load and facilitate faster, safer clinical reviews.

Live Demo: [https://oncology-dashboard-five.vercel.app/]

🎯 Product Design Logic & Pillars

1. 5-Second Clinical Orientation

Unified Context Card: The header immediately identifies the patient's current state (Age, Sex, Stage, Line of Therapy, and Performance Status) before the clinician dives into the details.
Contextual Change Alert: A focused summary at the top highlights exactly what shifted since the last visit (e.g., "50% mass reduction" or "New AST/ALT elevation").

2. Longitudinal Reasoning (Trends > Snapshots)

Response Correlation Matrix: The dashboard features a line chart plotting CEA biomarkers over time. This helps clinicians identify "biochemical progression" which often precedes physical radiological changes.
Lab Sparklines: Every safety lab (AST, ALT, Creatinine) includes a mini-trend chart with reference ranges to help clinicians distinguish between a "stable abnormal" value and a worsening clinical decline.

3. Responsible AI Framework

The "AI-Assisted Clinical Summary" follows a "Summarize, Don't Prescribe" philosophy:
Data Referencing: Every bullet point cites underlying evidence (e.g., "confirmed on 2024-12-08 scan").
Transparency on Uncertainty: The module explicitly flags missing data (e.g., "Missing: Recent Albumin") or pending imaging (e.g., PT-106) to ensure the clinician maintains ultimate decision-making agency.
Neutral Language: All treatment-related text is framed as "biological context" rather than clinical recommendations.

4. Minimalist Clinical Aesthetic

The UI uses a neutral "White-Paper" palette—utilizing Inter typography and high-density grids. This reduces visual noise, ensuring that life-critical alerts (like abnormal LFTs) stand out without being overshadowed by decorative UI elements.

🧬 Data Coverage

The dashboard supports 10 unique, high-fidelity patient profiles (PT-101 to PT-110) across three primary areas:
NSCLC: Focus on EGFR/ALK driver mutations and CNS sanctuary failure.
Breast Cancer: Highlighting HER2+ ADC response and rare populations (Male Breast Cancer).
Colorectal Cancer: Addressing MSI-High immunotherapy responders and BRAF V600E aggressive phenotypes.

🛠️ Technical Stack

Frontend: Standard HTML5 / Tailwind CSS (Medical-grade styling).
Visualization: Chart.js (used for longitudinal biomarker plotting and lab sparklines).
Iconography: Lucide-React.
Deployment: Optimized for Vercel (Static Site Deployment).

⚠️ Safety Disclaimer

This tool is a prototype designed to support clinical review. It does not provide medical recommendations, definitive diagnoses, or specific treatment instructions. All clinical decisions remain at the discretion of the licensed healthcare professional.

Developed by: [Itesh Mishra]

Candidate for: Technical APM | RISA Labs
