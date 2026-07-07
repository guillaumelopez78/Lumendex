# User interview synthesis

## 1. Individual User Profiles & Market Sentiment

| **User / Market** | **Sentiment Score** | **Core Pain Points** | **Functional Must-Haves** | **Low Interest / Antagonists** |
| --- | --- | --- | --- | --- |
| **Anders R.** (Denmark) | 5 | Low visibility into liquidity runway, especially the seasonality ebbs and flows. | **Web-First Visualization**: A dedicated top-corner dashboard widget for constant visibility of liquidity status. | Mobile-only features; he focuses on web-based monitoring. |
| **Bastiaan D.** (NL) | **9**  | Volatile seasonality (housing market); legal/familial tax implications. | Tax threshold alerts; advice on timing invoices for divorces/support. | Expensive full-service accounting packages. |
| **Jay H.** (DK) | **7** | Sporadic US credit payments vs. European net-30 terms. | Pattern recognition for late-paying debtors; product-level sales forecasting. | Automated "last word"—wants it as an aid, not a director. |
| **Sabine D.** (DE) | **6** | "Conservative anxiety"—idling excess cash due to tax deadline fears. | Clear views of upcoming tax dates (VAT/Income); vacation "What-if" scenarios. | Aggressive upselling of loans. |
| **Herke O.** (NL) | **6** | Irregular freelancer gaps; lack of supplier categorization in tools. | Cash-burn/Runway calculation; anomaly detection. | Generic automation that isn't customizable. |
| **Harry S.** (NL) | **7** | Client panic during liquidity dips; managing 40 years of manual habits. | 3-year long-term views; payment timetable popups. | "Fixed" programs that lack Excel-like flexibility. |
| **Pilu B.** (DK) | **5** | Debtors not paying on time; manual bank checking. | Short-term (14-day) view; investment impact simulations. | Abstract graphs without data click-through. |
| **Shota A.** (Intl) | **4** | German tax bureaucracy; high costs during pre-revenue phases. | Reliable data over "flooded" charts; mobile parity. | Complex manual testing/simulations. |
| **Rasmus L.** (DK) | **1** | Deep distrust of "artificial stupidity" (AI) and automated miscategorization. | **Drill-down transparency**: must see source data for every curve. | Automated forecasting; prefers "mental" modeling. |

## 2. The JTBD (Jobs to Be Done) Framework

- **The Safety Net Builder:** "When I have irregular project-based income , I want to see my **cash-burn rate, historical payment patterns** and **tax liabilities** , so I can know exactly how many months I can survive without a new contract."
- **The Strategic Invoicer:** "When I am nearing a tax threshold or legal maintenance limit , I want to **simulate delaying or moving an invoice date** , so I don't trigger unnecessary recalculations or taxes."
- **The Opportunity Optimizer:** "When I see a liquidity surplus , I want to **simulate a major purchase (e.g., a car or equipment)** , so I can grow my business without risking my ability to pay upcoming VAT."

Rephrasing

1. **The Safety Net Builder:** solopreneurs with difficulties to have a stable income, any help visualising next financial milestones is welcome. Not knowledgeable in Accounting.
2. **The Strategic Invoicer:** BO with 1 to 10 employees with a stable income, still wants to understand her/his cash-flow forecast but also wants to understand investment are possible in the future. No to little knowledge in Accounting.
3. **The Opportunity Optimizer:** solopreneurs with stable income and/or being independent as a hobby/second job, aim to optimise their finances and create long term simulation. Knowledgeable to expert in Accounting.

## **3. Cross-Market Strategic Comparison**

| **Feature / Factor** | **Germany (DE)** | **Denmark (DK)** | **The Netherlands (NL)** |
| --- | --- | --- | --- |
| **Primary Regulatory Fear** | **High Compliance Anxiety.** Focus on monthly VAT (Umsatzsteuer) and the 80% "fake employment" rule. | **Operational Efficiency.** Focus on seasonal "peak" planning (March–October) and managing complex credit cycles for international exports | **Legal & Life Complexity.** Demand for managing the intersection of business income and personal legal liabilities like spousal maintenance/child support. |
| **Cultural View of Cash** | **Conservative.** Keeping high reserves ("buckets") to mitigate fear of missing payments and seek "positive coaching" to reduce financial anxiety. | **Pragmatic/Old School.** Ranges from high-growth exporters to "hobby" owners who view cash as the only valid principle. | **Analytical.** Desire for "signals" or anomaly detection to prevent being "broke" unexpectedly. |
| **Platform Expectation** | **Desktop First.** High complexity requires a big screen for "slow thinking". | **Hybrid.** Desktop for planning ; mobile for scanning/quick check. | **Mobile Heavy.** High value on the phone for bus/travel uploads and daily monitoring. |

## **4. Red Flags & Friction Points**

- **Categorization Failure:** Users lose trust immediately when AI misidentifies regular suppliers or creates "noise".
- **"Black Box" Graphs:** Static curves are rejected. Users demand "drill-down" transparency—the ability to click any visual element to see the underlying invoice or bank transaction.
- **Data Trust vs. Reality:** Users will abandon the tool if the forecast doesn't align with their historical bank results.
- **The "Opt-Out" Need:** For micro-users (like Rasmus), forced automation is viewed as "annoying". The tool must be an optional "layer".
- **Manual Entry Fatigue:** If the tool requires manual input for data the bank already holds, adoption will fail.

## 5. The "Golden Path" Synthesis

### The #1 Problem to Solve: **"Buffer Anxiety"**

Entrepreneurs hoard cash unproductively because they lack a reliable, data-backed view of *when* their tax and creditor obligations will overlap with debtor inflows.

### 3 Critical UI/UX Elements for High Adoption

1. **The "Drill-Down" Auditor:** Every peak or dip in a graph must be interactive. Clicking a point must reveal the specific invoices (paid/unpaid) and recurring bank transactions that generated it.
2. **The "What-If" Simulation Toggle:** A sandbox mode to drag-and-drop payment dates or add "Draft Events" (e.g., "Hire New Staff" or "Buy Equipment") to visualize the immediate impact on runway.
3. **Anomaly & Signal Alerts:** Moving beyond simple "Low Balance" alerts to "Pattern Signals" (e.g., "Regular Rent payment missed" or "Unusually high utility bill detected". ).

### Strategic Insight: The "Good Job" Signal

Users across markets noted that financial software is historically punitive (negative alerts). An "unspoken" need exists for **Positive Reinforcement**: AI that alerts the user when they have *enough* surplus to safely pay a pension, invest, or take a vacation. This shifts the product from an "Accounting Chore" to a "Financial Partner."

---

|  | Focus | Features |
| --- | --- | --- |
| Visibility | Clarity & Trust | Intuitive Graph, Drill-down, Historical Trends. |
| Intelligence | Proactive Insight | Anomaly Detection, Pattern Signals, Action Suggestions,  Seasonality Alerts. |
| Strategy | Future Planning | "What-if" Scenarios, Runway Visualization, Funding Recommendations. |

- **Temporary user comparison map (First round)**
    
    This analysis synthesizes the feedback from eight distinct user interviews regarding the development of a cash flow forecasting and liquidity management tool for small business owners and freelancers.
    
    ### User Comparison Matrix: Operational Reality vs. Implicit Needs
    
    | **User Profile** | **Current Workflow & Tools** | **The "Breaking Point"** | **Critical Data Inputs** | **Implicit Needs (The Insight)** | **The "Aha!" Quote** |
    | --- | --- | --- | --- | --- | --- |
    | **Anna** (Coach/Consultant, 1-man, Germany) | Spreadsheet (AirTable); uses Wise for non-Euro/Contest for Euro.  | December/May "pile up" of annual subscriptions & tax surprises.  | Forecasted income based on invoices; recurring subscription dates.  | **Emotional Grounding:** She needs a tool that mitigates "anxiety" and offers positive reinforcement, not just red alerts.  | "I just wish to outsource it from the back of my head to the front of my eyes."  |
    | **Bastiaan** (Interpreter, 2-man, Netherlands) | Checks bank app daily; separate savings for VAT/Income tax.  | Exceeding income thresholds that trigger legal/tax recalculations (e.g., child support).  | Current balance + estimated year-end total for tax brackets.  | **The "Safe Ceiling":** He doesn't just want more money; he wants to know when to *stop* working to avoid tax/legal penalties.  | "I'm a freelancer... I check it every single day and sometimes even several times... because it's just fun to watch."  |
    | **Herke** (Financial Risk Mgr, 1-man, NL) | Manual "envelope" math; moves money between current/savings.  | Large, irregular bills or missing a "big" recurring payment (rent/VAT).  | Historical patterns to prove the model is "reliable."  | **Auditability:** As a pro, he won't trust a "black box" AI. He needs to see the past reflected perfectly before trusting the future.  | "If you just give me a forecast and I don't recognize it from my actual results, I will probably not look at it." |
    | **Harry** (Accountant, 2-man, Netherlands) | Custom Excel models based on annual reports.  | Clients in "panic" mode due to sudden liquidity shortages.  | Creditors, debtors, and specific product-level seasonality.  | **Translation:** He needs a tool that translates complex accounting data into "commercial" or "technical" language for his clients.  | "The first thing is to calm people down and then to start looking forward how we going to solve the basic problems."  |
    | **Jay** (Retail/Manufacturing, 2-man, Denmark) | Bank account balance + manual tracking of customer credit.  | Sporadic US payments on large $200k orders.  | Individual product-level sales performance.  | **Inventory Intelligence:** Liquidity is a proxy for "When can I afford to manufacture the next container?" | "Everything is season-based... Peak is March to October... and then it is a bit more quiet."  |
    | **Pilu** (Bookkeeper, 1-man, Denmark) | Bank account "in and out" tracking.  | Debtors who buy more but don't pay on time.  | Upcoming bills vs. "accounts that may or may not pay."  | **Advisory Capability:** He needs a "white-label" insight tool to look smarter in front of her own clients.  | "It would be very interesting to look far into the future... but some data has to be fed in, which gives meaning."  |
    | **Rasmus** (Hobby Farm/Invest., 1-man, DK) | Bank account & "excellent cash book."  | Paying interest on loans (he only buys cash).  | Source of income (ability to "click" a graph and see the receipt).  | **Skepticism/Autonomy:** He views automation as "artificial stupidity" and wants a tool that is purely reactive to his clicks.  | "The smarter the automation, the worse it gets, in my opinion."  |
    | **Shota** (Tech Consultant, 2-man, Estonia) | Wife manages finances; he checks Azure cost tools. +1 | Bureaucratic misunderstanding of German tax reports.  | Automatic tax calculation/VAT reporting.  | **Peace of Mind:** As an engineer, he wants a "set and forget" system that guarantees legal/tax compliance.  | "If you violate something in business there is big fines... we are very careful to do everything correctly."  |
    
    ---
    
    ### Strategic Synthesis
    
    ### 1. The Core Paradox: Control vs. Automation
    
    There is a fundamental tension between **Expert Skepticism** and **Operational Fatigue**.
    
    - **The Conflict:** Users like Rasmus and Herke view automation as a risk to accuracy , while users like Anna and Shota are desperate to "outsource" the mental load to an automated system.
    - **Resolution:** The tool cannot be a "black box." It must be **"Glass Box" Automation**—automated by default, but every data point must be "clickable" to reveal the underlying transaction for manual verification.
        
        
    
    ### 2. High-Value Opportunities (Immediate ROI)
    
    Based on the interviews, the top three features are:
    
    1. **Scenario Simulations ("What-If" Mode):** Nearly every user requested the ability to simulate a large purchase (like a car or new hire) or the loss of a major client to see the impact on their 6-12 month runway.
    2. **Visual Seasonality/Pattern Recognition:** Users (especially in retail) need the tool to "learn" that January is always slow and December is always expensive, preventing "false alarm" panics.
    3. **Tax/Pension "Actionable Excess" Alerts:** Instead of just showing a balance, tell the user: *"You have €2,000 in excess cash that isn't needed for bills or VAT—you can safely move this to your pension account today"*.
    
    ### 3. The "Trust Gap"
    
    The primary barrier to adoption is **historical data integrity**. Several users noted that current bookkeeping systems often miscategorize suppliers (e.g., defaulting to "General Costs"). If the software cannot perfectly categorize the *past*, users will not trust its projections for the *future*. To win, the tool must prioritize a "cleanup" phase where the user validates historical patterns before the forecast is generated.
    
    B*ased on the synthesis of the eight user interviews, a high-performing cash flow forecasting system must transition from a passive data display to an active, "glass-box" advisory tool. To meet the needs of diverse small business owners—ranging from the "anxious controller" to the "expert skeptic"—the system should function as follows:*
    
    ## 1. The "Glass-Box" Data Foundation
    
    Trust is the primary barrier to adoption. The system must prove its reliability by accurately reflecting the past before the user will trust the future.
    
    - **Historical Pattern Recognition:** The engine must analyze past data to identify recurring expenses (e.g., annual software subscriptions) and seasonal income trends.
        
        > *Anna Kuliberda: So it will be super easy to tell me hey in December you usually pay for this and this is an annual subscription for instance because I do use the subscriptions and that would be really helpful.*
        > 
    - **Supplier & Category Integrity:** To prevent the "Artificial Stupidity" gap, the system must accurately categorize historical transactions; if it cannot identify a supplier, it should prompt for human verification rather than guessing.
        
        > *Anna Kuliberda: tell me what is it in order for me to put it in the right place that is absolutely fine not everything is that easy to be understand and even I don't know if I do understand it correctly I'm fine with that collaboration.*
        > 
    - **Deep Drill-Downs:** Users must be able to click any point on a forecast graph to see the specific underlying invoices or transactions that generated that data point.
        
        > *Anna Kuliberda: So if I'm safe or not head is it everything according in an accounting dashboard I would expect to have very precise numbers that would be very helpful.*
        > 
    
    ## 2. Dynamic Forecasting & Simulation
    
    Static graphs are insufficient for business owners with irregular project-based income or complex credit terms.
    
    - **"What-If" Simulation Mode:** Users require a "playground" layer where they can add hypothetical events—such as buying a car, hiring an employee, or losing a major client—to see how it impacts their 6–12 month liquidity.
    - **Manual Assumption Overrides:** Freelancers need the ability to manually adjust "AI-detected" income trends, especially when they know a project is ending or a new one is starting that the system cannot yet see.
        
        > *Herke Oudeboon: then I will just say, "Okay, just give me the past the sources and then I will not look at the forecast because it's not reliable to me. It's your prediction but it's not my view on the forecast expenses I think they are predictable mostly……*
        > 
    - **Payment Behavior Algorithms:** The system should calculate "Actual Due Dates" based on a customer's historical payment speed (e.g., if a client always pays 10 days late, the forecast should reflect that delay rather than the invoice due date).
        
        > *Harry Schutte: And I think for example, you can also learn by Your bookkeeping system knows exactly what will be the average time of payment from certain clients.*
        > 
    
    ## 3. The Advisory & "Safety Net" Layer
    
    The system should move beyond raw numbers to provide "Actionable Intelligence".
    
    - **Threshold-Based Alerts:** Instead of generic notifications, the system should trigger specific alerts for "Expected Overdraft" or when a balance dips below a user-defined "Peace of Mind" floor.
    - **Compliance Monitoring:** Specifically for contractors (e.g., in Germany or the Netherlands), the system should alert users when they are nearing income thresholds that trigger tax reclassifications or legal penalties.
        
        > *Anna Kuliberda: I think one more thing that would be amazing and I know it may be super stupid but from the taxes purposes to be able to see whether I have an income this German requirement of the fake employment that is 80% from one client only per year.*
        > 
    - **Positive Reinforcement & Excess Cash Suggestions:** For "anxious" users, the system should identify "Safe-to-Spend" or "Safe-to-Invest" moments, suggesting when excess liquidity can be moved to a pension or savings account.
        
        > *…but I don't know if that pays out. But if they say okay when your cash balance is above something and we know there are not payments due the coming months or coming week we can put it for you on a saving account.*
        > 
    
    ## 4. Operational Design
    
    The system must adapt to the user’s specific hardware and mental context.
    
    - **Desktop for Analysis, Mobile for Alerts:** High-level strategic planning (simulations and quarterly reviews) should be prioritized for desktop , while real-time alerts and simple "current status" colors (Green/Yellow/Red) should reside on mobile.
        
        > *Pilu Kasper Bech: And here I'm thinking of examples like, for example, that you come up with a proposal for a loan, if you could see that there's something that writes, or now you have an extra amount of bonus on your account, so now you might be able to think about investing, or some liquidity-driven tools that are also connected to this, or a home to get public support, or something else entirely.*
        > 
    - **Simplified Storytelling:** Financial data must be translated into plain language, using "storytelling" techniques to explain where numbers come from and why they matter, without relying solely on dense accounting terminology.

---

## 📚 Related Documentation

**Project Hub:**
- [[../../../../Cash Pilot - Overview.md|Cash Pilot - Overview]]

**Research & Pain Points:**
- [[Overall pain points.md]] - Top 5 pain points
- [[User Stories.md]] - Requirements
- [[Market study workspace.md]] - Research summary

**Design & Product:**
- [[../../../../product-and-features.md|product-and-features]] - Personas & features
- [[../../../../design-principles.md|design-principles]] - UX principles

**Individual Personas:**
- [[Anna Kuliberda.md]] | [[Sabine Devins.md]] | [[Shota Akhalaia.md]]
- [[Pilu Kasper Bech.md]] | [[Rasmus Larsen.md]] | [[Jay Holm.md]]
- [[Anders Rutkjær.md]] | [[Harry Schutte.md]] | [[Herke Oudeboon.md]] | [[Bastiaan Doedee.md]]