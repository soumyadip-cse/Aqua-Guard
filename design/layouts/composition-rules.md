# AquaGuard — Composition Rules Specification

> Version: 1.0.0  
> Status: Design Foundation  
> Product: AquaGuard  
> Scope: Layout, spatial composition, grid, viewport structure, 3D/2D relationship, navigation, panels, overlays, information density, responsive behavior and screen hierarchy

---

# 1. Purpose

This document defines how AquaGuard's visual elements are arranged in space.

It establishes the composition rules for:

- desktop layouts
- 3D scenes
- control panels
- navigation
- telemetry overlays
- hydraulic visualization
- charts
- event timelines
- alerts
- controls
- responsive layouts
- mobile layouts
- diagnostic views

The objective is to make AquaGuard feel like one coherent control environment rather than a collection of independent screens.

---

# 2. Core Composition Principle

AquaGuard uses a hybrid composition:

```text
3D SYSTEM
+
2D CONTROL INTERFACE
+
SPATIAL TELEMETRY