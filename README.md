# Stage Previs & LED Mapping App

Desktop MVP for stage previs, LED wall layout, local JSON project storage, defensive Resolume XML import, and local preview sharing.

## Stack
- Tauri v2
- Rust
- React
- TypeScript
- Vite
- Three.js
- React Three Fiber
- Zustand
- Axum WebSocket preview server

## Run
```bash
npm install
npm run tauri dev
```

## Frontend-only dev
```bash
npm run dev
```

## Build
```bash
npm run build
npm run tauri build
```

## Implemented in this MVP
- Desktop shell scaffolding for Tauri v2
- 3D viewport with orbit camera, grid, stage floor, default LED walls
- Object selection with inspector-driven transform editing
- LED cabinet and resolution calculation
- Texture mapping controls with test patterns
- Save/open project JSON via Rust commands
- Defensive Resolume XML parsing
- Local preview server start/stop and WebSocket broadcasting path
- Lightweight browser preview page served from Rust

## Placeholder-backed areas
- FBX and OBJ import currently registers imported assets and renders a placeholder box instead of the original mesh
- Preview client is currently a debug HTML page that displays live JSON updates instead of a full synced 3D scene
- Share/export workflow is MVP-level and focused on local operation

## Suggested next build targets
1. Replace placeholder imported-model rendering with real OBJ/FBX loaders.
2. Upgrade the preview page to a React Three Fiber client.
3. Add layer editing and richer Resolume slice-to-screen assignment.
4. Add camera preset management and screenshot export polish.
# 0.APP
