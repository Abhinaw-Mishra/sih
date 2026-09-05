---
name: WebGL preview fallback
description: Browser previews may not expose a usable WebGL context even when Three.js dependencies are installed.
---

Use a capability check before mounting a React Three Fiber Canvas and keep a visually equivalent non-WebGL fallback for restricted browsers or automated previews.

**Why:** The workspace preview environment can reject WebGL context creation and surface the renderer error through the Vite overlay, making an otherwise healthy page look broken.

**How to apply:** Treat WebGL as an enhancement, not a rendering prerequisite; keep the fallback accessible and consistent with the surrounding hero.