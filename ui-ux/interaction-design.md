# AquaGuard Interaction Design

## 1. Purpose

AquaGuard is designed as an interactive water-management control room rather than a conventional dashboard.

Interaction design must make the physical water system understandable, controllable, and trustworthy.

Every interaction should answer one or more of these questions:

- What is happening now?
- What changed?
- Why did it change?
- What can the user control?
- What will happen if the user takes an action?
- Has the physical system actually confirmed that action?
- How serious is the current condition?

The interface should feel responsive and technologically advanced while remaining calm, precise, and engineering-oriented.

---

# 2. Core Interaction Principles

## 2.1 State before decoration

Visual effects must communicate system state.

Do not introduce animation, glow, particles, transitions, or 3D effects merely for visual spectacle.

Examples:

- Flow animation = water is actually flowing or simulated as flowing.
- Pump animation = pump is running.
- Valve movement = valve state is changing.
- Red leak visualization = leak condition is detected.
- Amber state = warning or uncertainty exists.
- Gray/inactive state = offline, unavailable, disabled, or unknown.

---

## 2.2 Physical truth

The interface must distinguish between:

1. Desired state
2. Commanded state
3. Confirmed physical state
4. Derived analytical state

Example:

```text
User clicks "Pump ON"

        ↓

Commanding

        ↓

ESP32 receives command

        ↓

Pump relay changes

        ↓

Telemetry confirms pump current / pump state

        ↓

Confirmed: RUNNING