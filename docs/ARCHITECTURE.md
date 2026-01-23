# Architecture: 10-typing-speed-trainer

## Overview
A high-fidelity typing speed trainer built with React 19 and Vite 6. The application focuses on real-time words-per-minute (WPM) calculation, accuracy tracking, and a premium minimal UI.

## Tech Stack
-   **Framework**: React 19
-   **Build Tool**: Vite 6
-   **Styling**: Tailwind CSS v4
-   **Animations**: Framer Motion 12
-   **Feedback**: Canvas Confetti
-   **Icons**: Lucide React

## Core Logic
-   **WPM Calculation**: Derived from the delta between `startTime` and current/end time, adjusted for valid word counts.
-   **Accuracy Tracking**: Real-time comparison of user input strings against target word arrays.
-   **Input Management**: Hidden focus input for a distraction-free typing experience.
-   **Shortcuts**: Global listener for `Tab + Enter` state resets.

## Performance
-   `useMemo` for derived statistics to prevent redundant re-renders during high-speed typing.
-   Optimized Framer Motion layout transitions for the typing caret.
-   Vite-bundled production assets for near-instant load times.
