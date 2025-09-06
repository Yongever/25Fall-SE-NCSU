<< Prompt 1. Finding Stakeholder >>

Based on the following project description:

[Project Perspective]
Now that you are familiar with our technology stack, you will work with a team to implement the WolfCafe system! WolfCafe is similar to GrubHub. A customer can order items, they are put together by a staff member, and the customer is notified when items are ready. You will reuse some code from CoffeeMaker in WolfCafe. Your team’s direct manager is your lab TA, but any of the TAs may serve as manager. Your instructors are Chief Technology Officers and product owners of the WolfCafe system. The goal is to deliver several new features, explore non-functional requirements, and new constraints.

[Problem Statement]
The CoffeeMaker system provides general functionality for creating ingredients, maintaining inventory, creating recipes, and ordering recipes. But the system is currently lacking user roles. Additionally, there is no functionality for making and fulfilling orders. The WolfCafe project has been created to set up user roles (admin, staff, and customer). You can port in your CoffeeMaker functionality around ingredients, inventory, recipes, and ordering recipes as a starting point for the WolfCafe project. The WolfCafe also comes with the idea of an “Item” — to move away from “Recipes” or to represent individual products (e.g., a bottle of water as distinct from a Latte).

Considering this project perspective and problem statement, identify all valid stakeholders for the WolfCafe system. Go beyond just admin, staff, and customer.

Please follow these steps:

1. Discovery by perspective — For each of these categories, brainstorm stakeholders:
- Users (direct users of the system)
- Clients/Sponsors (instructors, TAs, managers)
- Domain Experts (cafe managers, dining services)
- Developers/Engineers (student dev team, future maintainers)
- Regulators/Legal (IT, security, accessibility)
- Indirect/Negative stakeholders (suppliers, finance, university admin)

2. For each stakeholder, provide the following:

- [stakeholder]
    - role :
    - why this is stakeholder : 
    - how did I find it :

3. Organize your findings using a Power–Interest Grid and explain how different types of stakeholders should be engaged (manage closely, keep satisfied, keep informed, monitor).


<< Prompt 2. Clash Analysis >>

Draw stakeholder conflict/irrelevance graph like this.


### Functional Requirements Interactions

| Req ID | R1 | R2 | R3 | R4 | R5 | R6 | R7 | R8 | R9 | R10 |
|--------|----|----|----|----|----|----|----|----|----|------|
| R1=Auth                |    | –  |    |    |    |    |    |    |    |      |
| R2=Search              | +  |    |    |    | +  |    |    |    |    |      |
| R3=Booking             |    |    |    | –  |    | +  |    |    |    |      |
| R4=Passenger Mgmt      |    |    | –  |    |    |    |    |    |    |      |
| R5=Payment             |    | +  |    |    |    |    |    |    | –  |      |
| R6=Cancellation        |    |    | +  |    |    |    |    |    |    |      |
| R7=Status Updates      |    |    |    |    |    |    |    | +  |    |      |
| R8=Seat Selection      |    |    |    |    |    |    | +  |    |    | –    |
| R9=Loyalty             |    |    |    |    | –  |    |    |    |    |      |
| R10=Multilang Support  |    |    |    |    |    |    |    | –  |    |      |

#### Positive Interactions
- R1&R2: Auth enables personalization in search  
- R2&R5: Smooth flow into payment  
- R3&R6: Booking and cancellation cohesion  
- R7&R8: Live updates help seat choice  
- R9&R10: Multi-language enhances loyalty programs

#### Negative Interactions
- R1&R2: Auth may slow search  
- R3&R4: Conflicts if not synced  
- R5&R9: Loyalty adds complexity to payment  
- R8&R10: Multi-language complicates UI  
- R9&R5: Loyalty and payment overlap issues