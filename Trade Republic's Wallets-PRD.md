# Trade Republic Wallets: Product Requirements Document (PRD)

**Product:** Trade Republic  
**Author:** Inder, Jose Manuel and Sakshi - Ironhack Students 
**Status:** Validating

**AI Assistance Disclosure:**

- **Tool:** ChatGPT
- **Use:** AI was used to draft the initial version of the Product Requirements Document (PRD), including the feature description, user stories, acceptance criteria, roadmap, and supporting documentation.
- **Human Contribution:** We defined the business goals, refined the feature scope, reviewed and modified the AI-generated content, validated assumptions, prioritised the roadmap, adjusted the epics and user stories, and ensured the document aligned with Trade Republic's business context and Agile best practices.
- **Validation:** All content was manually reviewed for accuracy, consistency, and alignment with Product Management principles. Requirements, KPIs, and roadmap decisions were validated against Agile methodologies, PRD best practices, and Trade Republic's existing product capabilities.


---

# 01. Problem Statement

Trade Republic currently allows users to hold uninvested cash in a single cash balance. While this is sufficient for investing, it does not support users who want to organise their money according to different financial goals (e.g., emergency fund, vacation, taxes, or a new car).

As a result, users often rely on external banking or budgeting apps to separate their savings, reducing Trade Republic's role in their day-to-day financial management and increasing the likelihood of transferring funds outside the platform.

The **Wallets** feature aims to solve this by allowing users to create multiple virtual wallets within their Trade Republic account, making it easier to organise, manage, and eventually automate their savings while keeping more funds within the ecosystem.

---

# 02. Goals & Success Metrics

## Business Goals

### Primary Goal

- **Increase the average cash balance held per customer by 10% within six months by encouraging users to keep more funds within the Trade Republic ecosystem.**

### Secondary Goals

- Increase customer engagement by 15% within six months by encouraging users to manage their cash more actively within Trade Republic.
- Increase the 90-day customer retention rate by 8% within six months by expanding Trade Republic's role in users' day-to-day financial management.
- Establish a scalable cash management infrastructure that enables future capabilities such as automated savings and investing.

---

## User Goals

- Organise money by financial goal.
- Easily move money between wallets.
- Manage wallets without opening multiple bank accounts.
- Gain better visibility over available cash.

---

## Success Metrics (KPIs)

### Business KPIs

| Business Goal | KPI | Target |
| --- | --- | --- |
| **Increase cash balances held within Trade Republic** | **Average cash balance per customer** | **+10% within 6 months** |
|  | **Total customer cash held** | **+15% within 6 months** |
| Increase customer engagement | Monthly Active Users (MAU) | +15% within 6 months of launch |
|  | Average sessions per active user | +10% within 6 months |
|  | Average cash management actions per user (e.g., transfers, deposits, withdrawals) | +20% within 6 months |
| Increase customer retention | 90-day customer retention rate | +8% within 6 months |
|  | Customer churn rate | -5% within 6 months |

---

### Feature Adoption KPIs (Leading Indicators)

| KPI | Target |
| --- | --- |
| Wallet adoption rate (% of active users who create at least one wallet) | ≥30% within 3 months |
| Average number of wallets per Wallet user | ≥2 wallets |
| Percentage of Wallet users who transfer money between wallets at least once per month | ≥40% |
| Average number of wallet transfers per active Wallet user | ≥3 per month |
| Wallet deletion rate | \<10% within the first month after creation |

---

# 03. User Stories

## Primary Persona

Retail investors who also use Trade Republic as their primary savings platform.


##  Persona 1: Sarah — "The Goal-Oriented Saver"PRIMARY TARGET FOR MVP

###  Demographics

| **Attribute** | **Details** |
| --- | --- |
| Age | 28-35 |
| Occupation | Full-time employee (salary: €45K-70K) |
| Location | Berlin, Germany |
| Financial status | Middle class, financially literate |

###  Current Behavior

- Uses Trade Republic for investing (stocks, ETFs)
- Has multiple bank accounts (Commerzbank for salary, ING for savings, N26 for daily spending)
- Manually tracks savings goals in a spreadsheet
- Checks banking apps 2-3x per week

###  Pain Points

- Multiple bank accounts are confusing
- Mixes "money to invest" with "emergency fund" with "vacation savings"
- Doesn't know how much she's saved toward each goal
- Feels scattered financially

###  Motivation to Use Wallets

- "I want ONE place to manage all my money (savings + investing)"
- "I need to see my progress toward my €2K vacation goal"
- "I want to automate my savings, not manually transfer"

###  Expected Usage

- Creates 3-4 wallets (Emergency Fund €5K, Vacation €2K, Down Payment €10K, Monthly Cash €2K)
- Transfers money weekly (after payday)
- Checks wallets 2-3x per week
- High engagement with wallet feature

###  Strategic Value

- HIGH: Likely to increase cash balance in Trade Republic
- HIGH: Long-term retention (+ 25-30%)

---

##  Persona 2: Marcus — "The Casual Investor"SECONDARY TARGET

###  Demographics

| **Attribute** | **Details** |
| --- | --- |
| Age | 22-27 |
| Occupation | Part-time/Freelancer |
| Location | Europe (Italy, Spain) |
| Financial status | Lower-middle income, variable cash flow |

###  Current Behavior

- Uses Trade Republic for small stock purchases (occasional)
- Checks app once per week
- Money is held in "main account" (no organisation)
- Plans to invest more but "doesn't know where to start"

###  Pain Points

- Variable income = doesn't know how much to invest vs. save
- Feels overwhelmed by financial complexity
- Hasn't invested because he can't separate "safe money" from "investment money"

###  Motivation to Use Wallets

- "I want to save for my car, but also keep money for emergencies"
- "I should separate my investment budget from daily spending"
- "I like Trade Republic, so I want to organise money here"

###  Expected Usage

- Creates 2-3 wallets (Emergency Fund, Car Savings, Investment Fund)
- Transfers money monthly (less frequent)
- Checks wallets once per week
- Medium engagement

###  Strategic Value

- MEDIUM: Moderate increase in cash balance
- MEDIUM: May increase investment activity (psychological confidence)
- MEDIUM: Moderate retention improvement (+5%)

---

## Epic 1 – Wallet Foundation (MVP)

### Goal

Enable users to organise and manage their cash using multiple wallets.

### User Stories

- Create onboarding for wallet creation
- Create First Wallet
- Rename a Wallet
- Delete a Wallet
- Create More Wallets
- Transfer money between wallets
- Add money to a wallet
- View Wallets

### Business Value

- Improve cash organisation.
- Increase user engagement.
- Increase average cash flow.
- Complete the wallet lifecycle.
- Establish the foundation for future Wallet capabilities.

### Business Rules

- Main Wallet cannot be deleted.
- Wallets with a positive balance cannot be deleted.
- Users must confirm wallet deletion.
- Duplicate names are not allowed.

---

## Epic 2 – Goal-Based Saving

### Goal

Help users save towards specific financial objectives.

### User Stories

- Set a savings goal for each wallet.
- Track savings progress.
- Customise wallets with icons and colours.
- Receive milestone notifications.
- Allow a digital credit/debit card per Wallet.

### Business Value

- Encourage disciplined saving.
- Improve user engagement.
- Increase cash retention.

---

## Epic 3 – Wallet Automation

### Goal

Help users save and invest automatically with minimal effort.

### User Stories

- Schedule recurring transfers into a wallet.
- Round up purchases into a wallet.
- Automatically invest a wallet's balance into an existing Savings Plan.
- Automatically invest the interest earned by a wallet into a selected investment.
- Pause or modify automation settings.

### Business Value

- Increase automation adoption.
- Increase Assets Under Management (AUM).
- Reduce idle cash.
- Improve long-term customer retention.

---

## Epic 4 – Smart Wallets

### Goal

Provide intelligent insights that help users make better financial decisions.

### User Stories

- Budget tracking.
- Personalised savings recommendations.
- Cash flow forecasting.
- Allow deleting wallets with money (a pop-up notification confirmation appears, and the money is transferred to the main account)

### Business Value

- Differentiate Trade Republic from competitors.
- Increase feature engagement.
- Position Trade Republic as a comprehensive financial platform.

---

# 04. Proposed Solution

## In Scope (MVP)

The Wallets feature will introduce multiple virtual wallets within a user's Trade Republic account.

Users will be able to:

- Create wallets
- Rename wallets
- Delete empty wallets
- Transfer money between wallets
- Add money to wallets
- View wallet transactions

Wallets share the same IBAN and legal account; they are internal cash allocations, not separate bank accounts.

---

## Out of Scope

The following capabilities are excluded from the MVP:

- Savings goals
- Wallet customisation (icons/colors)
- Automatic transfers
- Automatic investing
- Shared wallets
- Individual IBANs per wallet
- Budget analytics

These will be considered in future releases.

---

# 05. Functional Requirements (MoSCoW)

## Must Have

- Create an onboarding for wallet creation
- Create First wallet
- Create More Wallets
- Rename wallets.
- Delete empty wallets
- Transfer money between wallets 
- View wallet

---

## Should Have

- Customize wallets with icons and colors
- Set a savings goal for each wallet.
- Track savings progress
- Receive milestone notifications
- Allow a digital credit/debit card per Wallet

---

## Could Have

- Schedule recurring transfers into a wallet
- Automatically invest a wallet's balance into an existing Savings Plan
- Automatically invest the interest earned by a wallet into a selected investment.
- Pause or modify automation settings
- Round up purchases into a wallet

---

## Won't Have (MVP)

- Allow a digital credit/debit card per Wallet
- Budget tracking
- Personalized savings recommendations
- Cash flow forecasting

---

# 06. Non-Functional Requirements

## Performance

- Wallet creation \<2 seconds.
- Internal transfers processed in real time (\<1 second).
- Wallet overview loads in \<2 seconds.

---

## Security

- Existing authentication mechanisms apply.
- Transfers require standard Trade Republic security checks.
- All wallet actions are logged for auditing.

---

## Privacy

- Wallet data follows GDPR requirements.
- No additional personal information is collected.

---

## Accessibility

- WCAG 2.1 AA compliant.
- Screen reader compatible.
- Keyboard navigation supported.
- Colour contrast meets accessibility standards.

---

## Technical Constraints

- Wallets use the existing cash ledger.
- No new bank accounts or IBANs are created.
- Existing payment infrastructure remains unchanged.
- Wallet balances must always reconcile with the total cash balance.

---

# 07. Risks & Trade-offs

| Risk | Mitigation |
| --- | --- |
| Users may think wallets are separate bank accounts | Clear onboarding and in-app explanations |
| Increased complexity in cash management | Keep MVP simple and intuitive |
| Users accidentally delete wallets | Confirmation dialogue and delete only when balance is €0 |
| Additional backend complexity | Reuse existing cash management infrastructure where possible |

---

## Trade-offs

### We are choosing:

- Simplicity over advanced budgeting.
- Virtual wallets over multiple IBANs.
- Fast MVP delivery over feature completeness.

This enables faster validation while minimising technical and regulatory complexity.

---

# 08. Open Questions

| Question | Owner | Target Date |
| --- | --- | --- |
| Should wallet transfer history have a dedicated screen? | Product | Sprint 2 planning |
| Will Wallets support joint accounts in the future? | Product Strategy | Future Release planning |

---

# Appendix: Future Roadmap

The Wallets feature is designed as the foundation for a broader cash management experience:

- **Epic 1:** Wallet Foundation (MVP)
- **Epic 2:** Goal-Based Saving
- **Epic 3:** Wallet Automation (recurring transfers and integration with existing automatic investing)
- **Epic 4:** Smart Wallets (budgeting insights and personalised recommendations)

This phased approach allows Trade Republic to validate the core Wallets concept quickly, while progressively expanding it into a comprehensive financial management solution that increases customer engagement, cash retention, and Assets Under Management (AUM).
