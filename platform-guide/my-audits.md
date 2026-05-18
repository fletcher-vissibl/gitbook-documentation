# My Audits

My Audits is where you plan, run, and record internal, external, and supplier audits. Each audit is scoped to specific clauses, and findings flow directly into Non Conformities.

***

When you open **My Audits**, you'll see a table of all your audits. Each row shows:

* **Audit ID.** Automatically assigned (e.g. `AUD-1`, `AUD-INT-12`, `AUD-EXT-13`).
* **Audit Name** and **Description**.
* **Audit Type.** Internal, External, or Supplier Audit.
* **Compliance Framework.** Which standard the audit is against (e.g. ISO 9001). An audit can cover multiple frameworks.
* **Start Date** and **End Date**.
* **Department Audited.**
* **Auditee Name.**

### Creating an Audit

Click + Audit in the top right. Fill in:

1. **Audit name and description.**
2. **Audit type** — Internal, External, or Supplier Audit.
3. **Compliance framework.**
4. **Start and end dates.**
5. **Department being audited.**
6. **Auditee name** (the person or team being audited).
7. **Internal Auditor Name** and/or **External Auditor Name**.

### Audit Detail View

Click any audit to open it. The detail view has three tabs: **Details**, **Clauses**, and **Attachments**.

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

**Expanded audit row.** Click a row to see its full details — clauses, status, assigned people.

#### Details Tab

Shows all the audit information plus:

* **Clauses.** The specific framework clauses included in this audit's scope. These appear as tags (e.g. "4.1 — Understanding the organization and its context", "5.1 — Leadership and commitment").
* **Status.** Whether the audit is Open or Closed.
* **People.** Additional people involved in the audit.
* **+ Add Property.** Add custom fields if needed.

#### Clauses Tab

This is where you conduct the audit. Every selected clause is listed with its requirement description. For each requirement you have two actions:

* Conform — The requirement is being met. Click to open a modal where you can add a description of how it's met and upload supporting documents as evidence. Click **Conform** to save.
* Raise NCR — The requirement is not being met. Click to open a form with fields for Type, Observation, Source, Date Reported, Priority, and Evidence. Click **Submit NCR** to create the non-conformity. It's added directly to the Non Conformities board, linked to this audit.

#### Attachments Tab

Upload any additional files related to the audit (e.g. audit plans, external auditor reports, correspondence).

### Running a Vissi Audit

You can also run an AI-powered audit from the **Frameworks** page. Open any framework and click **Run Vissi Audit** in the top right. Vissi analyses your documentation and evidence against every clause, updates your compliance statuses, and flags gaps.

This is separate from the manual audits in My Audits but complements them.

### Filtering Tables

Most list views in Vissibl — audits, non-conformities, vendors, risks — use tables with built-in column filters. This section shows you how to filter any table to quickly find the rows you need.

💡 Where filtering worksThe same column-filter pattern works on **every table** in Vissibl: Non Conformities, Vendors, Vendor Risks, Risk Assessment, People, and more.

#### How to Filter a Column

1. **Open the filter menu.** Click the filter icon in the column header you want to filter by. The icon appears when you hover over the column header area.
2. **Choose a filter condition.** A dropdown appears with options:\
   Contains rows where the value includes your text\
   Equals only exact matches\
   Starts with rows beginning with your text
3. **Type your filter value.** The table updates in real time as you type.
4. **Confirm.** Press <kbd>Enter</kbd> or click outside the filter to lock it in.

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

**Step 1–2.** Click the filter icon in a column header, then choose a condition (Contains, Equals, Starts with).

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

**Step 3.** Type your value — the table filters in real time as you type.

#### Active Filters

When one or more filters are active, Vissibl shows visual indicators so you always know what's being filtered:

**Clearing filters:**

* **Single filter:** Click the bin icon on the filtered column and clear the text field, or change the condition back.
* **All filters:** Click **View Settings** or the **×** on the filter badge.

💡 Filters are session-basedFilters reset when you navigate away from the page. They don't persist across sessions.

### Tips

**NCRs are auto-linked**NCRs raised during an audit are automatically linked to that audit. Filter the Non Conformities board by audit ID to see all findings from a specific cycle.

**Auditor impartiality**For internal audits, make sure the auditor is not auditing their own department. Impartiality is a requirement of the ISO standards.

**Spread audits across the year**Avoid doing everything at once. Continuous coverage gives better assurance and avoids a pre-audit scramble.

**Combine with Vissi Audit**Run a Vissi Audit from Frameworks before an external audit to catch documentation gaps. Then use My Audits for the formal clause-by-clause review.**Stack multiple filters**You can filter several columns at once. All conditions must match (AND logic).

**Status & dropdown columns**Columns with predefined values (like Audit Type or Status) offer selectable options instead of free-text search.

**Date columns**Date fields provide date-range pickers — filter by Before, After, Between, or On a specific date.

**View Settings**Use View Settings to toggle column visibility — hide columns you don't need to reduce clutter.

