
# Copilot input

Based on the feature requests in the most popular apps, users are looking for several key features to enhance their experience:

- User-Friendly Interface: A well-designed and intuitive interface is crucial for a seamless user experience1.
- ‘How-To’ Screens: Educational screens that help users understand how to use the app’s features1.
- Chat Support/Callback Functions: Quick and easy access to support through the app1.
- Search Option: An essential feature that allows users to easily find what they’re looking for within the app1.
- Battery Preservation: Apps should be optimized to minimize battery drain1.
- Push Notifications: Timely and relevant notifications to keep users informed and engaged2.
- Offline Functionality: Allowing users to use the app without an internet connection2.

These features are considered must-haves for successful, user-friendly mobile apps. It’s important to note that the specific importance of each feature can vary depending on the type of app and its target audience. For a more detailed exploration, you might want to look into the sources provided for a comprehensive list of features valued by users.

## Tauri + Vue 3 + TypeScript

This template should help get you started developing with Vue 3 and TypeScript in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)

## Type Support For `.vue` Imports in TS

Since TypeScript cannot handle type information for `.vue` imports, they are shimmed to be a generic Vue component type by default. In most cases this is fine if you don't really care about component prop types outside of templates. However, if you wish to get actual prop types in `.vue` imports (for example to get props validation when using manual `h(...)` calls), you can enable Volar's Take Over mode by following these steps:

1. Run `Extensions: Show Built-in Extensions` from VS Code's command palette, look for `TypeScript and JavaScript Language Features`, then right click and select `Disable (Workspace)`. By default, Take Over mode will enable itself if the default TypeScript extension is disabled.
2. Reload the VS Code window by running `Developer: Reload Window` from the command palette.

You can learn more about Take Over mode [here](https://github.com/johnsoncodehk/volar/discussions/471).
