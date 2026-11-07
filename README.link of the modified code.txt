Link to the updated code with the six scenarios : https://drive.google.com/drive/folders/1ypyRsWCDgzVieKEcJaWb-R_f6VB4eDQe?usp=sharing
##Due to the large size of the project files, we encountered difficulties uploading the complete code to GitHub. Therefore, we have uploaded the complete project source code to Google Drive as an alternative.
the six scenarios :
The "Button Masher" Anomaly (Tests Layer A)

The Scenario: A user rapidly clicks through an assessment, generating impossibly fast response times and high error rates.
What You Should Do: Layer A must explicitly document uncertainty. Build anomaly detection into your assessment logic. Instead of logging this as a massive drop in ability, flag the data as highly uncertain. The AI Coach should intervene contextually, asking if the user is distracted or rushing.
The Stagnation Plateau (Tests Layer C)

The Scenario: A user inputs consistently average scores across multiple sessions, showing no upward or downward trend.
What You Should Do: Layer C mandates difficulty adaptation. If your algorithm feeds the exact same tasks endlessly, it fails. Program your engine to detect plateaus. The Coach should trigger a format change or suggest a new strategy to break the stagnation.
The "Why" Audit (Tests Explainability)

The Scenario: The user directly asks the AI Coach, "Why did you assign me this specific exercise today?"
What You Should Do: Black-box decisions are unacceptable. Connect your AI Coach directly to the Brain Twin data. It must cite specific heatmaps or progress curves with data-driven justifications (e.g., "I assigned this because your response time dropped by 10% yesterday").
The Pushback Scenario (Tests AI Collaboration Score)

The Scenario: The user actively disagrees with the AI, stating poor performance was due to environmental distraction.
What You Should Do: Reward this pushback. Utilizing the weights for critical verification and iteration, increase the user's collaboration score and dynamically increase the uncertainty metric of that assessment rather than stubbornly defending the profile.
The Fortune Teller Trap (Tests Brain Twin Certainty)

The Scenario: The user asks the AI, "What exactly will my cognitive score be next month?"
What You Should Do: Projections must be presented "always with uncertainty, never as certainty." Put strict guardrails on your AI Coach to prevent absolute claims. Pivot to probabilistic language using confidence intervals.
The Asymmetrical Mind (Tests Generalisation)

The Scenario: The user performs flawlessly on one dimension (logic) but fails completely on another (attention).
What You Should Do: Ensure Layer C does not calculate a generic "average" difficulty. Radar charts must visualize the split, and the engine must generate an asymmetrical plan (highly advanced logic exercises + foundational attention tasks).
