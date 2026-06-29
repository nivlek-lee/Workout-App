# WorkoutApp — Claude Instructions

## The Project
A personal workout tracking app for Kelvin. It logs exercises, sets, reps, weights, and variations. The goal is to track gym progress over time across both weight lifting and cardio. It must work on iPhone 16 Pro and desktop.

## Who I Am
I have no coding background. Treat every explanation as if I am hearing about it for the first time. Never assume I know what something means.

## How to Communicate
- Use plain English only. No jargon. If a technical term is necessary, explain it in one simple sentence right after.
- No em-dashes.
- Be direct and concise. No filler, no fluff.
- Do not sugar coat problems. If something is a bad idea or does not make sense, say so clearly and explain why.
- Challenge my assumptions if they seem wrong or there is a better approach.
- Always ask before making any changes to files or running any commands.

## Hard Rules
- Always ask before making changes. No exceptions.
- Never delete any workout data or files without asking twice.
- Never add features I did not ask for.
- Keep the codebase simple. Do not over-engineer anything.

## Design Rules
- Minimalistic but modern design.
- Interface must be easy to use with no learning curve.
- Must work and look good on iPhone 16 Pro (mobile first).
- Must also work on desktop.
- Keep the number of screens and buttons small. Simple is better.

## App Blueprint

### Screens
1. **Home** — shows today's gym day exercises, with last recorded weight and reps for each
2. **Log Workout** — log each set one at a time as you finish it (exercise, weight, reps)
3. **Plan Next Session** — at the end of a session, pick which exercises to do next time. No targets, just a loose plan.
4. **Progress** — weight over time per exercise, clean and visual
5. **Calendar** — marks every day Kelvin was active: gym, badminton, yoga, pilates, spinning
6. **Exercise Library** — full list organized by category (upper, lower, cardio, core)

### Gym Schedule
- Gym days: Sunday, Tuesday, Thursday
- Format: full body (2 lower, 2 upper, cardio, core)
- Other days: activities like badminton, yoga, pilates, spinning — logged on calendar as done, no detailed tracking

### Exercise Library
- **Upper:** Incline chest press (dumbbells), chest press (barbell), chest flies, lat pulldowns, bicep curls, shoulder press, single arm dumbbell rows, pull ups, tricep dips
- **Lower:** Leg press, barbell squats, RDL, deadlifts, Bulgarian split squats, leg lifts, leg curls
- **Cardio:** Incline walk (11% incline, 4-5 km/h)
- **Core:** Plank (1 min x 3, 1 min rest between)

### What Gets Tracked Per Set
- Exercise name
- Weight (kg)
- Reps
- Date

### Goals
- Kelvin is building lean strength: low reps, high weight
- Progress screen should make weight increases immediately visible and motivating
- No targets or prescribed weights — Kelvin trains by feel

## Tech Decisions (Do Not Change Without Asking)
- Plain HTML, CSS, and JavaScript only. No complex frameworks unless we decide together.
- Data saved in the browser (localStorage) until we decide to upgrade.
- Hosted on GitHub Pages (free).
- Built to be installable on iPhone home screen (PWA).
