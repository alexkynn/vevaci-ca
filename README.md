# VEVACI Strategic Diagnostic Engine 🚀

> **Stop Guessing. Start Measuring.**
> The VEVACI Diagnostic is a proprietary 25-question audit for Canadian business owners, medical professionals, and High-Net-Worth (HNW) individuals.

## 📖 Project Overview
The VEVACI Strategic Diagnostic Engine is a fully automated, AI-driven lead qualification and analysis pipeline. It is designed to evaluate a prospect's corporate financial chassis across critical pillars—such as Asset Protection, Tax Efficiency, Estate Liquidity, and Strategy Readiness—and instantly generate an elite, personalized tax and insurance strategy brief.

The system dynamically analyzes the prospect's data to recommend advanced corporate architectures (like Immediate Financing Arrangements - IFA) or pivot to holistic protection strategies (Critical Illness, Disability, Term/Permanent Life) based on algorithmic scoring.

## 🏗️ Architecture & Tech Stack

This pipeline is built on a "Zero-Code / High-Logic" automation stack:

* **Frontend Data Collection:** [Fillout Forms](https://www.fillout.com/) (Bilingual: English/Simplified Chinese)
* **Middleware & Automation:** [Make.com](https://www.make.com/) (Webhooks, Routing, Data Stores)
* **AI Analysis Engine:** Google Gemini 1.5 Pro API (via Google AI Studio)
* **Delivery System:** Gmail (HTML-formatted Executive Briefs)
* **Database & Logging:** Google Sheets
* **Scheduling:** Native Fillout Google Calendar Sync

## ⚙️ System Flow

1. **Gateway & Triage:** The client completes a highly structured, 25-question diagnostic covering their Wealth DNA, Corporate Architecture, Protection Gaps, and Estate Intelligence. 
2. **Abuse Protection:** Make.com intercepts the webhook and runs the email/IP through a Data Store "Bouncer" to prevent spam and protect AI API credits.
3. **Dynamic AI Analysis:** The data is passed to Google Gemini, which operates under a strict "Senior Canadian Tax Strategist & Insurance Architect" persona.
4. **Algorithmic Scoring (0-100):** Gemini calculates an alignment score for advanced leverage strategies (IFA) based on tax friction (e.g., SBD Grind), time horizon, and leverage comfort.
5. **Strategic Pivot:** * *High Score (>75):* Pitches Immediate Financing Arrangements (IFA) and Corporate Estate Bonds.
    * *Low Score (<75) or Individual Profile:* Elegantly pivots to Holistic Protection (Income Continuity, Family Estate Creation).
6. **Report Generation:** Make.com parses the AI's JSON output and injects it into a premium, Navy/Gold branded HTML email template.
7. **Data Logging:** The complete client profile and AI score/strategy are logged into a master Google Sheet for future marketing analysis.

## 🛡️ Canadian Compliance & Regulatory Logic

This engine is hardcoded with strict instructions to recognize and flag Canadian tax vulnerabilities, including:
* **The 'Clean Pipeline' Rule:** Flags the necessity of direct loan-to-investment flows for Paragraph 20(1)(c) interest deductibility.
* **The CDA ACB Trap:** Audits corporate structures (HoldCo/OpCo/Multiple Corps) to warn against the undue reduction of the Capital Dividend Account when designating multiple corporate beneficiaries.
* **The SBD Grind:** Recognizes when corporate passive income exceeds $50k and highlights the resulting tax friction.
* **2026 Capital Gains Inclusion:** Leverages the 2/3 (66.7%) inclusion rate hike to mathematically position tax-exempt insurance growth against traditional taxable portfolios.

## 🚀 Setup & Deployment Guide

To replicate or maintain this environment:

1. **Fillout:** Import the `VEVACI_Client_Diagnostic_E&SC.json` file into Fillout to generate the frontend form. Ensure the native Scheduling block is connected to your primary Google Calendar.
2. **Make.com Setup:**
   * Create a custom Webhook to catch Fillout submissions.
   * Add a Google Gemini module (Requires API Key from Google AI Studio). Map the System Instructions and JSON output schema.
   * Ensure `Parse JSON` is used to split the AI response into usable variables.
   * Add a Gmail module to send the customized HTML template.
3. **Data Security:** Ensure Make.com Data Stores are active to restrict submissions to 1-per-24-hours per email address to prevent API abuse.

## 🔒 Privacy & Confidentiality
All data collection adheres to SOC 2 Type 2 compliance via Fillout and Make.com. The AI analysis utilizes Google's enterprise API environment, ensuring no client financial data is used to train public LLM models. 

---
*Developed for VEVACI Strategic Wealth Architecture.*
