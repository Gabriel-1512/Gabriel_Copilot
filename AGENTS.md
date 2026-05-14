# AGENTS.md

## Project Overview
Bingo Mixer is a social bingo game built with React, TypeScript, and Tailwind CSS. It helps people mingle at events by finding others who match icebreaker questions to get 5 in a row.

## Build and Run Commands
- Install dependencies: `npm install`
- Start dev server: `npm run dev` (serves on http://localhost:5173)
- Build for production: `npm run build`
- Run tests: `npm run test`
- Lint code: `npm run lint`

## Code Structure and Conventions
- **Components**: Functional React components in `src/components/`, using hooks for state
- **Hooks**: Custom hooks in `src/hooks/` for game logic (e.g., `useBingoGame`)
- **Utils**: Pure functions in `src/utils/` (e.g., bingo logic)
- **Data**: Static data in `src/data/` (questions array)
- **Styling**: Tailwind CSS classes for responsive design
- **Testing**: Vitest for unit tests, colocated with code
- **TypeScript**: Strict typing throughout, types in `src/types/`

## Key Patterns
- Immutability: Use spread operators and new arrays/objects
- State management: Local state with `useState`, effects with `useEffect`
- Bingo logic: Separate concerns in utils, testable functions

## Potential Pitfalls
- Ensure questions array has enough unique items for board generation
- Free space is always in center (index 12)
- Winning lines: rows, columns, diagonals

## Links to Documentation
- [README.md](README.md): Setup and overview
- [workshop/GUIDE.md](workshop/GUIDE.md): Learning workshop
