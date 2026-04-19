# Workonomia

An economic management simulator built in Java with Swing. You start with zero capital and a dead-end gig selling water at a traffic light — under the "mentorship" of Jombson, a corporate buzzword-spewing antagonist who thinks he's disrupting the economy.

Progress from grinding manual labor to building a passive income empire by hiring and managing employees. Each worker has their own salary cost and profitability. Scale up, balance the payroll, survive the tax system, and dodge random events (like employees demanding raises) before your balance hits -100 and Jombson wins.


https://github.com/user-attachments/assets/4c08f98b-3f53-4523-855d-1acfb338d480


## Gameplay

- **Work** — click the work button to earn money manually
- **Hire** — recruit employees once you've built enough capital
- **Survive** — a game loop fires every 4–5 seconds: employees generate profit, wages get deducted, progressive taxes apply (10% / 25% / 40% based on net income), and random events can spike your costs
- **Story** — narrative chapters unfold as you hit milestones; Jombson and Pedrinho the Capybara will make appearances

**Lose condition:** balance drops below -R$100 — bankruptcy, Jombson wins.

## Tech Stack

- Java + Swing (NetBeans GUI forms)
- `ScheduledExecutorService` for the game loop
- Spring Boot backend (`/backend`) with Spring Security and JPA
- Audio via `javax.sound.sampled`

## Running

Open in NetBeans and run `src/trabalho/Trabalho.java`, or compile and run from the project root.

Requires Java 11+.

---

## Contributors

- **João Luis Almeida Santos** — [@lyszt](https://github.com/lyszt)
- **Francinildo Felix Guedes** — [@Felix0w](https://github.com/Felix0w)
