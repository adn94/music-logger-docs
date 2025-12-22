# Testing Strategy

This document outlines the testing philosophy and priorities for the Music Logger project. Given the current development phase (active feature development, design not finalized), we prioritize logic and stability over visual regression testing.

## 1. Core Philosophy
**Functionality First, Aesthetics Later.**
Our primary goal is to ensure the application is reliable in a live environment (clubs, events). A crash during a set is unacceptable. Visual perfection is secondary until the design is finalized.

## 2. Testing Priorities

### ✅ Priority 1: Robustness & Resilience ("Unhappy Paths")
The app runs for hours in unstable environments. We must test failure states as rigorously as success states.

*   **Network Stability:** What happens if the internet cuts out for 1 second? 1 minute?
*   **API Failures:** Handling timeouts (e.g., ACRCloud/Shazam API not responding) gracefully without crashing the UI.
*   **Resource Management:** Verify that timers and streams are disposed of correctly to prevent memory leaks during long sessions.

### ✅ Priority 2: Algorithmic Verification
Logic that involves calculation or complex state transitions must be verified in isolation (Pure Unit Tests).

*   **Time & Drift:** Verify calculations for drift compensation and timestamping independent of the system clock or UI.
*   **Logic Isolation:** Test the mathematical formulas and parsing logic without spinning up the UI or Simulator.

### ✅ Priority 3: Test Hygiene & Isolation
To maintain a healthy test suite, we strictly adhere to:

*   **Tabula Rasa:** Every test starts with a clean state. No shared state between tests.
*   **Fixtures:** Use static data files for API responses instead of dynamic or real network calls.
*   **Determinism:** Tests must produce the same result every single time.

## 3. Deferred / Out of Scope

### ⏸️ Visual Regression ("Golden Tests")
**Status: Postponed.**
Since the UI/UX design is still iterating, pixel-perfect tests (Golden Tests) would be too brittle and require constant maintenance.
*   **Plan:** We will introduce Golden Tests only for critical, stable screens (e.g., the main logging view) once the design is frozen.
