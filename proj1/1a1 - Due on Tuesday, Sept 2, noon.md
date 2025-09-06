> Create list of stakeholders (e.g., Admin, Staff, Customer, etc.)
> - Who else? How to find? Brainstorm with an LLM.

- Users: Customer, Staff
- Sponsors: Instructors, Teaching Assistants
- Domain Experts: Cafe Manager, Dining Service Supervisor
- Developers: Current Developers, Future Developers, Maintenance Team
- Regulators: University IT/Security, Accessibility Officers, Compliance Officers
- Indirect Stakeholders: Suppliers, Vendors, University Administration, Finance Department

## Users
### Customer
- role: Places orders, pays for items, receives notifications.
- why: Their satisfaction defines whether the system succeeds; they influence usability and service features.

### Staff (baristas, kitchen, cashiers)
- role: Prepares items, updates order status, interacts with inventory.
- why: Their workflow efficiency directly depends on the system.

## Sponsors
### Instructors (Professors, acting as CTOs/Product Owners)
- role: Define high-level requirements, set grading and constraints.
- why: They determine what counts as success in the project.

### Teaching Assistants (TAs, acting as project managers)
- role: Manage student teams, assign tasks, evaluate progress.
- why: They influence priorities and scope management.

## Domain Experts
### Cafe Manager, Dining Service Supervisor
- role: Oversees menu, pricing, inventory, and reports.
- why: Needs accurate inventory tracking and sales data.

## Developers
### Student Development Team
- role: Builds, tests, and delivers WolfCafe features.
- why: Their feasibility concerns (time, scope, skills) shape requirements.

### Future Developers, Maintenance Team
- role: Extend or maintain the system after initial development.
- why: They depend on code quality, documentation, and modularity.

## Regulators
### University IT / Security
- role: Provide infrastructure, authentication, and enforce security.
- why: Their policies constrain design choices.

### Accessibility / Compliance Officers
- role: Ensure ADA-compliant interfaces and inclusivity.
- why: They enforce non-functional requirements like accessibility.

## Indirect Stakeholders

### Suppliers, Vendors
- role: Provide ingredients and goods.
- why: Inventory features must reflect supplier restocking cycles.

### University Administration / Finance Department
- role: Oversee budgets, branding, and overall dining services.
- why: They impose policies on cost, pricing, and reporting.


## Power–Interest Grid
| Power / Interest | High Interest | Low Interest |
| - | - | - |
| **High Power**   | **Sponsors**: Instructors (define scope, grade), TAs (manage project) <br> **Domain Experts**: Cafe Manager, Dining Service Supervisor (control operations, inventory)                                                           | **Regulators**: University IT/Security, Accessibility/Compliance Officers (set rules, but not daily users) <br> **Indirect Stakeholders**: University Administration, Finance Dept (control budgets/policies, but not engaged in daily use) |
| **Low Power**    | **Users**: Customers (want usability, variety), Staff (want workflow simplicity, speed) <br> **Developers**: Current Dev Team, Future Maintenance Team (care deeply about feasibility and sustainability, but limited authority) | **Indirect Stakeholders**: Suppliers/Vendors (impacted through inventory/orders, but little direct say)                              |


- Manage closely: Instructors, Cafe Manager, ㅆㅁ.
- Keep satisfied: University IT/Security, Admin, Finance.
- Keep informed: Customers, Staff, Developers.
- Monitor: Suppliers, Future Developers, Vendors.



> Identify stakeholder biases:

- Customers : speed, low cost, convenience.
- Staff : efficiency, less complexity.
- Admin : accuracy, control, reports.
- Developers : feasibility, limited workload.
- IT : security, compliance.
- Instructors : ambitious scope, educational value.

> - List 5 ways needs of one stakeholder might clash/be irrelevant to another.
> - How to find? Brainstorm with an LLM.

# Clash/Irrelevant Matrix
| Stakeholder ID | S1 | S2 | S3 | S4 | S5 | S6 |
| - | - | - | - | - | - | - |
| **S1 Customers**   |              | Clash        | Irrelevant        | Irrelevant              | Clash             | Clash              |
| **S2 Staff**       | Clash            |          | Clash        | Irrelevant              | Irrelevant             | Irrelevant              |
| **S3 Admin**       | Irrelevant            | Clash        |          | Irrelevant              | Irrelevant             | Irrelevant              |
| **S4 Instructors** | Irrelevant            | Irrelevant        | Irrelevant        |                | Clash             | Irrelevant              |
| **S5 Developers**  | Clash            | Irrelevant        | Irrelevant        | Clash              |               | Clash              |
| **S6 IT/Security** | Clash            | Irrelevant        | Irrelevant        | Irrelevant              | Clash             |                |



### Clash
- S1 Customers - S2 Staff : Variety vs. Simplicity
    Customers want heavy customization and variety in orders, while staff prefer a simplified workflow to prepare items quickly.
- S1 Customers - S5 Developers : Expectation vs. Feasibility
    Customers desire a polished, feature-rich app experience, but the development team is constrained by time and skills within one semester.
- S1 Customers - S6 IT/Security : Usability vs. Security
    Customers want quick, possibly guest-style checkout, while IT insists on strong authentication and data protection.
- S2 Staff - S3 Admin : Flexibility vs. Control
    Staff want the ability to quickly adjust inventory or substitute items, while Admin demands strict accuracy and central control of records.
- S4 Instructors - S5 Developers : Ambition vs. Resources
    Instructors want ambitious features to meet educational objectives, but developers must keep scope realistic to deliver within deadlines.

### Irrelevance
- S1 Customers - S3 Admin: Customers care about order status, not admin’s detailed revenue reports.
- S2 Staff - S5 Developers: Staff focus on day-to-day operations; developers care about code quality and deadlines.
- S4 Instructors - S6 IT/Security: Professors set educational scope, while IT enforces technical compliance, with little overlap.



Comment on prompt crafting:
- Compare zero-shot prompting to careful prompting.

Write at least 10 use cases (≈5 pages total):
- Each with: Preconditions, Main Flow, Subflows, Alternative Flows.
- How to find? Feed structure to LLM as prompt, then provide examples from slides.
