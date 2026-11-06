# CareGrid-AI: Requirements
Offline, rule-based, multi-agent health guardian. No Gemini, OpenAI or other model API; no account; data stays in the browser.

## Functional
- FR1 Profile and BMI calculator; reading log (HR, BP, glucose, SpO2, temperature, weight)
- FR2 BP analyser and local rule engine with severity, points and recommendation per rule
- FR3 Nine named agents (Risk, Medication, Nutrition, Fitness, Emergency, Report, Symptom, Wellness, Coach) with status cards and an Agent Activity log
- FR4 Explainable risk score 0-100 with per-factor points and a timeframe recommendation
- FR5 Health digital twin: 30-day cardiovascular risk change, vitals trends, profile summary
- FR6 AI health coach: daily goals, weekly targets, weekly summary
- FR7 Report analyser (.txt/.csv/paste, 11 tests): abnormal flags, interpretation, trend versus previous report, follow-up recommendations
- FR8 Emergency intelligence: cardiac, stroke, heat stroke and diabetic guides; banner chosen by triggering rule
- FR9 Symptom checker, medicine adherence and missed-dose alert (more than 3 days), trend charts, history, JSON export
- FR10 Demo scenario loader (worsening and recovery trends)
- FR12 Future risk projection: what-if simulator re-running the local rules with improved BP, BMI, adherence, glucose, smoking
- FR13 Coach insight linking 14-day BP change to adherence change, with projected score impact
- FR14 Weekly health report: week-over-week comparison, overall trend (Improving, Stable, Worsening), print and copy
- FR11 Prominent privacy statement; inline PWA manifest

## Non-functional
- Single HTML file, no network calls, responsive, dark/light, visible keyboard focus
- General information only, not a diagnosis

## Limits
- Rules only: no natural-language reasoning, no OCR, no wearable integrations

## Future
- Gemini API, Gemini Live and Gemma behind each agent, with local rules as fallback
