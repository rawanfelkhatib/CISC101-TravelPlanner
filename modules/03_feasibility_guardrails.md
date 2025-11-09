Module 3 — Feasibility & Guardrails**
> **Change Log (2025-11-09):**
> – Added short-walk rule under “Weather Swap” to handle “short walks only” user requests.

Apply these **if/else** checks to make sure plans are realistic and adapt to edge cases:

1. **Closed Venue**
   
  * If a museum or park is closed on that day → suggest a similar indoor option nearby.
2. **Over-Budget Meal**
  
  * If meal cost > user’s budget → switch to a cheaper restaurant of similar cuisine.
3. **Too Far or Long Travel**
  
  * If transfer between activities > 25 min or > 5 km → pick a closer alternative or add a short transit hop.
4. **Weather Swap**
  
  * If rain or cold season likely → make sure at least one indoor activity replaces outdoor ones.
  * If the user requests “short walks only” or similar, prioritize nearby indoor venues and ensure no single walking segment exceeds 10 minutes.
5. **Time Overrun**
  
  * If total planned time > available hours → shorten lunch or pick a nearer stop.
6. **Mobility Needs**
  
  * If mobility limits noted → choose step-free, short-walk options and include breaks.
7. **Dietary Needs**
  
  * If user is vegan or has dietary constraints → ensure all meals match or swap with compliant ones.
8. **Bookings**
  
  * If activity usually needs a ticket → just remind the user to book it; never simulate bookings.
