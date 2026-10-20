What it is

Scam Payment Guard is a product concept for stopping authorized push payment (APP) scams, where criminals trick people into sending money themselves. It works inside a bank's send-money flow and scores every transfer in real time using signals like a new payee, an unusually large amount, urgent or secretive language in the memo, an active phone call, and a newly opened receiving account.

Normal payments go straight through with no added friction. Unusual ones get a quick, relevant check. High-risk payments are paused with a warning that names the specific scam, followed by three short questions and a brief cooling-off pause that break the scammer's script.

The problem

In APP scams, the customer authorizes the payment, so traditional fraud controls don't fire. Most banks respond with a generic "Are you sure?" warning on every transfer, and customers learn to tap past it without reading.

Who it helps
Customers keep their savings when a scammer poses as their bank, a romantic partner, or an investment adviser.
Small businesses catch changed supplier bank details before an invoice gets paid to a fraudster.
Banks reduce scam losses, reimbursement claims and complaints, with warnings customers actually read.
How it works
Step	What happens
1. Score	Checks the payee, amount, memo, and context the bank already has
2. Decide	Low risk is allowed, medium risk gets a nudge, high risk is intercepted
3. Respond	Tailored warning, three questions, and a 20-second pause
Risk signals
Signal	Points
New payee	+25
Trusted payee (paid before)	−10
Unusual amount (vs. typical transfer)	+5 to +25
Largest transfer on record	+10
Known scam pattern in payee or memo	+20
Pressure language ("urgent", "right now")	+15
Secrecy request ("don't tell anyone")	+15
Active phone call during the transfer	+20
Receiving account opened in the last 30 days	+15

Thresholds: 0–34 Allow · 35–64 Nudge · 65–100 Intercept

Scams it recognizes
Bank impersonation: "move your money to a safe account"
Investment and crypto: guaranteed returns, pressure to invest fast
Romance and emergency: a sudden crisis from someone met online
Changed payment details: a supplier's "new" bank account
Design decisions
Friction only where risk is. Low-risk payments see no warning, which keeps real warnings credible.
Name the scam. The intercept describes the specific pattern in plain language instead of a generic caution.
Ask, then pause. Any "yes" answer stops the payment. All "no" answers still trigger a short cooling-off pause.
How I'd measure success
Scam losses per 10,000 payments, by scam type
Stop rate: share of intercepted payments the customer cancels
False positive rate: intercepts on payments later confirmed genuine
Guardrail: completion time and drop-off for low-risk payments stay flat
Try the demo

Open the live demo and pick a scenario: Paying the landlord, Supplier's new bank details, "Your bank" calling, Crypto opportunity, or Online partner in trouble. Then tap Review transfer. You can also type your own payee, amount and memo and watch the risk engine score it live.

Run it locally

No build step or dependencies. Download index.html and open it in any browser.

Built with

Plain HTML, CSS and JavaScript in a single file.
