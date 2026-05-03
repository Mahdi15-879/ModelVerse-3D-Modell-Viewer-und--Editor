# ModelVerse – 3D Model Viewer and Editor

ModelVerse is a web-based 3D model viewer and editor built with Next.js, TypeScript, React, and Babylon.js.  
The application allows users to import 3D models, inspect their meshes, select individual mesh objects, customize mesh colors in real time, add optional mesh event handlers, and export the edited model as a GLB file.

## Overview

ModelVerse was developed as a portfolio project to explore 3D rendering in the browser and to practice building a more advanced interactive frontend application.

The project combines modern web development with real-time 3D rendering.  
It focuses on file import, 3D scene setup, mesh selection, UI state management, color customization, and model export.

## Core Features

- Import 3D models from the local file system
- Support for common 3D file formats:
  - `.glb`
  - `.gltf`
  - `.obj`
  - `.babylon`
  - `.stl`
- Render imported models on a Babylon.js canvas
- Automatically create and manage a 3D scene, camera, and lighting
- Display all detected meshes in a sidebar
- Select meshes from the sidebar or directly from the 3D canvas
- Change the color of a selected mesh in real time
- Add optional custom event handler code for selected meshes
  - onClick handler
  - onHover handler
- Export the edited model as a `.glb` file
- Save mesh event handler data as a separate JSON file
- Clear the current model and import a new one
- Responsive canvas resizing
- User feedback through toast notifications

## Tech Stack

| Technology | Purpose |
|---|---|
| Next.js | React framework and application structure |
| TypeScript | Type-safe development |
| React | UI components and state management |
| Babylon.js | 3D rendering, scene management, model loading, and GLB export |
| Tailwind CSS | Styling and responsive layout |
| Radix UI | Accessible UI primitives |
| Lucide React | Icons |
| React Hook Form / Zod | Form-related utilities available in the project setup |

## Project Structure

```text
src/
├── app/
│   ├── globals.css
│   ├── layout.tsx
│   ├── loading.tsx
│   └── page.tsx
├── components/
│   ├── icons/
│   ├── model-verse/
│   │   ├── BabylonCanvas.tsx
│   │   ├── FileImporter.tsx
│   │   ├── MeshSidebar.tsx
│   │   └── ModelVerseApp.tsx
│   └── ui/
├── hooks/
├── lib/
└── ai/
