

```
TaL
├─ .dockerignore
├─ .editorconfig
├─ .env.app
├─ .env.docker
├─ .eslintignore
├─ .eslintrc.cjs
├─ .npmrc
├─ Dockerfile
├─ LICENSE
├─ README.md
├─ android
│  ├─ app
│  │  ├─ build.gradle
│  │  ├─ capacitor.build.gradle
│  │  ├─ proguard-rules.pro
│  │  └─ src
│  │     ├─ androidTest
│  │     │  └─ java
│  │     │     └─ com
│  │     │        └─ getcapacitor
│  │     │           └─ myapp
│  │     │              └─ ExampleInstrumentedTest.java
│  │     ├─ main
│  │     │  ├─ AndroidManifest.xml
│  │     │  ├─ java
│  │     │  │  └─ app
│  │     │  │     └─ aiaw
│  │     │  │        └─ MainActivity.java
│  │     │  └─ res
│  │     │     ├─ drawable
│  │     │     │  ├─ ic_launcher_background.xml
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-hdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-ldpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-mdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-night-hdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-night-ldpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-night-mdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-night-xhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-night-xxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-night-xxxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-xhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-xxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-land-xxxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-night
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-hdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-ldpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-mdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-night-hdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-night-ldpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-night-mdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-night-xhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-night-xxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-night-xxxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-xhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-xxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-port-xxxhdpi
│  │     │     │  └─ splash.png
│  │     │     ├─ drawable-v24
│  │     │     │  └─ ic_launcher_foreground.xml
│  │     │     ├─ layout
│  │     │     │  └─ activity_main.xml
│  │     │     ├─ mipmap-anydpi-v26
│  │     │     │  ├─ ic_launcher.xml
│  │     │     │  └─ ic_launcher_round.xml
│  │     │     ├─ mipmap-hdpi
│  │     │     │  ├─ ic_launcher.png
│  │     │     │  ├─ ic_launcher_background.png
│  │     │     │  ├─ ic_launcher_foreground.png
│  │     │     │  └─ ic_launcher_round.png
│  │     │     ├─ mipmap-ldpi
│  │     │     │  ├─ ic_launcher.png
│  │     │     │  ├─ ic_launcher_background.png
│  │     │     │  ├─ ic_launcher_foreground.png
│  │     │     │  └─ ic_launcher_round.png
│  │     │     ├─ mipmap-mdpi
│  │     │     │  ├─ ic_launcher.png
│  │     │     │  ├─ ic_launcher_background.png
│  │     │     │  ├─ ic_launcher_foreground.png
│  │     │     │  └─ ic_launcher_round.png
│  │     │     ├─ mipmap-xhdpi
│  │     │     │  ├─ ic_launcher.png
│  │     │     │  ├─ ic_launcher_background.png
│  │     │     │  ├─ ic_launcher_foreground.png
│  │     │     │  └─ ic_launcher_round.png
│  │     │     ├─ mipmap-xxhdpi
│  │     │     │  ├─ ic_launcher.png
│  │     │     │  ├─ ic_launcher_background.png
│  │     │     │  ├─ ic_launcher_foreground.png
│  │     │     │  └─ ic_launcher_round.png
│  │     │     ├─ mipmap-xxxhdpi
│  │     │     │  ├─ ic_launcher.png
│  │     │     │  ├─ ic_launcher_background.png
│  │     │     │  ├─ ic_launcher_foreground.png
│  │     │     │  └─ ic_launcher_round.png
│  │     │     ├─ values
│  │     │     │  ├─ ic_launcher_background.xml
│  │     │     │  ├─ strings.xml
│  │     │     │  └─ styles.xml
│  │     │     └─ xml
│  │     │        ├─ file_paths.xml
│  │     │        └─ network_security_config.xml
│  │     └─ test
│  │        └─ java
│  │           └─ com
│  │              └─ getcapacitor
│  │                 └─ myapp
│  │                    └─ ExampleUnitTest.java
│  ├─ build.gradle
│  ├─ capacitor.settings.gradle
│  ├─ gradle
│  │  └─ wrapper
│  │     ├─ gradle-wrapper.jar
│  │     └─ gradle-wrapper.properties
│  ├─ gradle.properties
│  ├─ gradlew
│  ├─ gradlew.bat
│  ├─ settings.gradle
│  └─ variables.gradle
├─ capacitor.config.ts
├─ docs
│  ├─ .vitepress
│  │  ├─ config.ts
│  │  └─ theme
│  │     ├─ custom.css
│  │     └─ index.ts
│  ├─ index.md
│  ├─ public
│  │  ├─ combine.webp
│  │  ├─ icon-256x256.png
│  │  ├─ lighthouse_score_desktop.png
│  │  ├─ lighthouse_score_mobile.png
│  │  ├─ plugin-market.png
│  │  └─ ui.webp
│  ├─ self-host
│  │  ├─ advanced.md
│  │  └─ index.md
│  ├─ usage
│  │  ├─ artifacts.md
│  │  ├─ assistants.md
│  │  ├─ common-issues.md
│  │  ├─ cross-platform.md
│  │  ├─ custom-provider.md
│  │  ├─ data-sync.md
│  │  ├─ file-parse.md
│  │  ├─ index.md
│  │  ├─ mcp.md
│  │  ├─ plugin-dev.md
│  │  ├─ plugins.md
│  │  ├─ prompt-vars.md
│  │  ├─ res
│  │  │  ├─ assistant-prompt-vars.png
│  │  │  ├─ code-convert-artifact.png
│  │  │  ├─ custom-provider.webp
│  │  │  ├─ gen-image.webp
│  │  │  ├─ message-edit.png
│  │  │  ├─ mobile-install-btn.webp
│  │  │  ├─ pc-install-btn.png
│  │  │  ├─ prompt-var-input.png
│  │  │  ├─ quote.png
│  │  │  ├─ selection-convert-artifact.png
│  │  │  ├─ text-file.png
│  │  │  ├─ use-custom-provider.png
│  │  │  ├─ video-parse.png
│  │  │  └─ workspace-list.png
│  │  └─ share-link.md
│  └─ zh
│     ├─ index.md
│     ├─ self-host
│     │  ├─ advanced.md
│     │  └─ index.md
│     └─ usage
│        ├─ artifacts.md
│        ├─ assistants.md
│        ├─ common-issues.md
│        ├─ cross-platform.md
│        ├─ custom-provider.md
│        ├─ data-sync.md
│        ├─ file-parse.md
│        ├─ index.md
│        ├─ mcp.md
│        ├─ plugin-dev.md
│        ├─ plugins.md
│        ├─ prompt-vars.md
│        ├─ res
│        │  ├─ assistant-prompt-vars.png
│        │  ├─ code-convert-artifact.png
│        │  ├─ custom-provider.webp
│        │  ├─ gen-image.webp
│        │  ├─ message-edit.png
│        │  ├─ mobile-install-btn.webp
│        │  ├─ pc-install-btn.png
│        │  ├─ prompt-var-input.png
│        │  ├─ quote.png
│        │  ├─ selection-convert-artifact.png
│        │  ├─ text-file.png
│        │  ├─ use-custom-provider.png
│        │  ├─ video-parse.png
│        │  └─ workspace-list.png
│        └─ share-link.md
├─ index.html
├─ package.json
├─ pnpm-lock.yaml
├─ postcss.config.mjs
├─ public
│  ├─ ai-avatars
│  │  ├─ 33.avif
│  │  ├─ alice.webp
│  │  ├─ android.webp
│  │  ├─ arona.webp
│  │  ├─ atri.webp
│  │  ├─ cyberlife.png
│  │  ├─ delamain.webp
│  │  ├─ detroit.webp
│  │  ├─ evil.webp
│  │  ├─ glados.webp
│  │  ├─ neuro.webp
│  │  ├─ ptilopsis.webp
│  │  ├─ rhine.webp
│  │  └─ win11.webp
│  ├─ banner.svg
│  ├─ emotions
│  │  └─ nachoneko
│  │     ├─ 0.webp
│  │     ├─ 1.webp
│  │     ├─ 10.webp
│  │     ├─ 11.webp
│  │     ├─ 12.webp
│  │     ├─ 13.webp
│  │     ├─ 14.webp
│  │     ├─ 15.webp
│  │     ├─ 16.webp
│  │     ├─ 17.webp
│  │     ├─ 18.webp
│  │     ├─ 19.webp
│  │     ├─ 2.webp
│  │     ├─ 20.webp
│  │     ├─ 21.webp
│  │     ├─ 22.webp
│  │     ├─ 23.webp
│  │     ├─ 24.webp
│  │     ├─ 25.webp
│  │     ├─ 26.webp
│  │     ├─ 27.webp
│  │     ├─ 28.webp
│  │     ├─ 29.webp
│  │     ├─ 3.webp
│  │     ├─ 30.webp
│  │     ├─ 31.webp
│  │     ├─ 32.webp
│  │     ├─ 33.webp
│  │     ├─ 34.webp
│  │     ├─ 4.webp
│  │     ├─ 5.webp
│  │     ├─ 6.webp
│  │     ├─ 7.webp
│  │     ├─ 8.webp
│  │     └─ 9.webp
│  ├─ fonts
│  │  └─ material-symbols-outlined-lite.woff2
│  ├─ icons
│  │  ├─ apple-icon-120x120.png
│  │  ├─ apple-icon-152x152.png
│  │  ├─ apple-icon-167x167.png
│  │  ├─ apple-icon-180x180.png
│  │  ├─ apple-launch-1080x2340.png
│  │  ├─ apple-launch-1125x2436.png
│  │  ├─ apple-launch-1170x2532.png
│  │  ├─ apple-launch-1179x2556.png
│  │  ├─ apple-launch-1242x2208.png
│  │  ├─ apple-launch-1242x2688.png
│  │  ├─ apple-launch-1284x2778.png
│  │  ├─ apple-launch-1290x2796.png
│  │  ├─ apple-launch-1536x2048.png
│  │  ├─ apple-launch-1620x2160.png
│  │  ├─ apple-launch-1668x2224.png
│  │  ├─ apple-launch-1668x2388.png
│  │  ├─ apple-launch-2048x2732.png
│  │  ├─ apple-launch-750x1334.png
│  │  ├─ apple-launch-828x1792.png
│  │  ├─ favicon-128x128.png
│  │  ├─ favicon-32x32.png
│  │  ├─ favicon-96x96.png
│  │  ├─ icon-128x128.png
│  │  ├─ icon-192x192.png
│  │  ├─ icon-256x256.png
│  │  ├─ icon-384x384.png
│  │  ├─ icon-512x512.png
│  │  ├─ ms-icon-144x144.png
│  │  └─ safari-pinned-tab.svg
│  ├─ json
│  │  ├─ assistants.en-US.json
│  │  ├─ assistants.zh-CN.json
│  │  ├─ assistants.zh-TW.json
│  │  ├─ plugins.en-US.json
│  │  ├─ plugins.zh-CN.json
│  │  └─ plugins.zh-TW.json
│  ├─ robots.txt
│  └─ svg
│     ├─ aiaw.svg
│     ├─ alibaba-c.svg
│     ├─ alibaba.svg
│     ├─ anthropic.svg
│     ├─ aperture.svg
│     ├─ claude-c.svg
│     ├─ claude.svg
│     ├─ cohere-c.svg
│     ├─ deepseek-c.svg
│     ├─ deepseek.svg
│     ├─ gemini-c.svg
│     ├─ gemini.svg
│     ├─ gemma-c.svg
│     ├─ gemma.svg
│     ├─ github.svg
│     ├─ google-c.svg
│     ├─ google.svg
│     ├─ grok.svg
│     ├─ groq.svg
│     ├─ huggingface-c.svg
│     ├─ huggingface.svg
│     ├─ meta-c.svg
│     ├─ meta.svg
│     ├─ microsoft-c.svg
│     ├─ mistral-c.svg
│     ├─ mistral.svg
│     ├─ ollama.svg
│     ├─ openai.svg
│     ├─ openrouter.svg
│     ├─ qwen-c.svg
│     ├─ qwen.svg
│     └─ togetherai-c.svg
├─ quasar.config.js
├─ resources
│  ├─ android
│  │  ├─ icon-background.png
│  │  └─ icon-foreground.png
│  ├─ icon.png
│  ├─ splash-dark.png
│  └─ splash.png
├─ scripts
│  └─ sync-version.js
├─ src
│  ├─ App.vue
│  ├─ assets
│  │  └─ quasar-logo-vertical.svg
│  ├─ boot
│  │  ├─ global-components.ts
│  │  ├─ i18n.ts
│  │  └─ unocss.ts
│  ├─ components
│  │  ├─ AAvatar.vue
│  │  ├─ ATip.vue
│  │  ├─ AbortableBtn.vue
│  │  ├─ AccountBtn.vue
│  │  ├─ AddInfoBtn.vue
│  │  ├─ AddMcpPluginDialog.vue
│  │  ├─ ArtifactItemIcon.vue
│  │  ├─ ArtifactItemMenu.vue
│  │  ├─ ArtifactsExpansion.vue
│  │  ├─ AssistantItem.vue
│  │  ├─ AssistantsExpansion.vue
│  │  ├─ AutocompleteInput.vue
│  │  ├─ AvatarPanel.vue
│  │  ├─ CodeJar.vue
│  │  ├─ ConvertArtifactDialog.vue
│  │  ├─ CopyBtn.vue
│  │  ├─ CustomProviders.vue
│  │  ├─ DarkSwitchBtn.vue
│  │  ├─ DialogList.vue
│  │  ├─ DialogsExpansion.vue
│  │  ├─ DragableSeparator.vue
│  │  ├─ EnablePluginsItems.vue
│  │  ├─ EnablePluginsMenu.vue
│  │  ├─ GetModelList.vue
│  │  ├─ HctPreviewCircle.vue
│  │  ├─ HintCard.vue
│  │  ├─ HueSlider.vue
│  │  ├─ HueSliderDialog.vue
│  │  ├─ ImageAvatar.vue
│  │  ├─ ImageInputArea.vue
│  │  ├─ ImportDataDialog.vue
│  │  ├─ InstallPluginBtn.vue
│  │  ├─ InstalledPlugins.vue
│  │  ├─ JsonInput.vue
│  │  ├─ JsonInputDialog.vue
│  │  ├─ LazyInput.vue
│  │  ├─ ListInput.vue
│  │  ├─ MenuItem.vue
│  │  ├─ MessageAudio.vue
│  │  ├─ MessageFile.vue
│  │  ├─ MessageImage.vue
│  │  ├─ MessageInfoDialog.vue
│  │  ├─ MessageItem.vue
│  │  ├─ ModelDragSortDialog.vue
│  │  ├─ ModelInputItems.vue
│  │  ├─ ModelItem.vue
│  │  ├─ ModelOptionsBtn.vue
│  │  ├─ ModelsInput.vue
│  │  ├─ ParseFilesDialog.vue
│  │  ├─ PayDialog.vue
│  │  ├─ PayMethodItem.vue
│  │  ├─ PickAvatarDialog.vue
│  │  ├─ PlatformEnabledInput.vue
│  │  ├─ PluginTypeBadge.vue
│  │  ├─ PromptVarEditor.vue
│  │  ├─ PromptVarInput.vue
│  │  ├─ PromptVarItem.vue
│  │  ├─ ProviderInputItems.vue
│  │  ├─ SaveDialog.vue
│  │  ├─ SearchDialog.vue
│  │  ├─ SelectFileBtn.vue
│  │  ├─ SelectWorkspaceDialog.vue
│  │  ├─ ShortcutKeyInput.vue
│  │  ├─ SubproviderInput.vue
│  │  ├─ SubscribeDialog.vue
│  │  ├─ TextareaDialog.vue
│  │  ├─ ToolContent.vue
│  │  ├─ TopupDialog.vue
│  │  ├─ TypesInput.vue
│  │  ├─ UnifiedInput.vue
│  │  ├─ VarsInput.vue
│  │  ├─ ViewCommonHeader.vue
│  │  ├─ ViewFileDialog.vue
│  │  ├─ ViewImageDialog.vue
│  │  ├─ WorkspaceListItem.vue
│  │  ├─ WorkspaceListSelect.vue
│  │  ├─ WorkspaceNav.vue
│  │  └─ global
│  │     └─ AInput.js
│  ├─ composables
│  │  ├─ avatar-image.ts
│  │  ├─ back.ts
│  │  ├─ call-api.ts
│  │  ├─ close-artifact.ts
│  │  ├─ create-artifact.ts
│  │  ├─ create-dialog.ts
│  │  ├─ file-url.ts
│  │  ├─ filter-options.ts
│  │  ├─ first-visit.ts
│  │  ├─ get-model.ts
│  │  ├─ install-plugin.ts
│  │  ├─ key-composition.ts
│  │  ├─ listen-key.ts
│  │  ├─ live-query.ts
│  │  ├─ local-reactive.ts
│  │  ├─ locate-id.ts
│  │  ├─ login-dialogs.ts
│  │  ├─ md-preview-props.ts
│  │  ├─ open-last-workspace.ts
│  │  ├─ order.ts
│  │  ├─ persistent-reactive.ts
│  │  ├─ set-theme.ts
│  │  ├─ set-title.ts
│  │  ├─ subscription-notify.ts
│  │  ├─ sync-ref.ts
│  │  └─ workspace-actions.ts
│  ├─ css
│  │  ├─ app.scss
│  │  └─ quasar.variables.scss
│  ├─ env.d.ts
│  ├─ i18n
│  │  ├─ en-US
│  │  │  ├─ components.ts
│  │  │  ├─ composables.ts
│  │  │  ├─ index.ts
│  │  │  ├─ others.ts
│  │  │  ├─ pages.ts
│  │  │  └─ views.ts
│  │  ├─ index.ts
│  │  ├─ zh-CN
│  │  │  ├─ components.ts
│  │  │  ├─ composables.ts
│  │  │  ├─ index.ts
│  │  │  ├─ others.ts
│  │  │  ├─ pages.ts
│  │  │  └─ views.ts
│  │  └─ zh-TW
│  │     ├─ components.ts
│  │     ├─ composables.ts
│  │     ├─ index.ts
│  │     ├─ others.ts
│  │     ├─ pages.ts
│  │     └─ views.ts
│  ├─ layouts
│  │  └─ MainLayout.vue
│  ├─ pages
│  │  ├─ AccountPage.vue
│  │  ├─ AssistantsPage.vue
│  │  ├─ EmptyPage.vue
│  │  ├─ ErrorNotFound.vue
│  │  ├─ ModelPricing.vue
│  │  ├─ PluginsPage.vue
│  │  ├─ SetProvider.vue
│  │  ├─ SettingsPage.vue
│  │  └─ WorkspacePage.vue
│  ├─ quasar.d.ts
│  ├─ router
│  │  ├─ index.ts
│  │  └─ routes.ts
│  ├─ shims-vue.d.ts
│  ├─ stores
│  │  ├─ assistants.ts
│  │  ├─ index.ts
│  │  ├─ plugins.ts
│  │  ├─ providers.ts
│  │  ├─ store-flag.d.ts
│  │  ├─ ui-state.ts
│  │  ├─ user-data.ts
│  │  ├─ user-perfs.ts
│  │  └─ workspaces.ts
│  ├─ utils
│  │  ├─ artifacts-plugin.ts
│  │  ├─ audio-process.ts
│  │  ├─ config.ts
│  │  ├─ cors-fetch.ts
│  │  ├─ db.ts
│  │  ├─ doc-parse.ts
│  │  ├─ functions.ts
│  │  ├─ image-process.ts
│  │  ├─ local-data.ts
│  │  ├─ mcp-client.ts
│  │  ├─ mcp-sse-transport.ts
│  │  ├─ middlewares.ts
│  │  ├─ platform-api.ts
│  │  ├─ plugins.ts
│  │  ├─ sessions.ts
│  │  ├─ tauri-shell-transport.ts
│  │  ├─ tauri-stream.ts
│  │  ├─ template-engine.ts
│  │  ├─ templates.ts
│  │  ├─ types.ts
│  │  ├─ update.ts
│  │  ├─ values.ts
│  │  └─ web-search-plugin.ts
│  ├─ version.json
│  └─ views
│     ├─ AssistantView.vue
│     ├─ AssistantsMarket.vue
│     ├─ CustomProvider.vue
│     ├─ DialogView.vue
│     ├─ EditArtifact.vue
│     ├─ PluginAdjust.vue
│     ├─ PluginSettings.vue
│     ├─ PluginsMarket.vue
│     ├─ SettingsView.vue
│     ├─ ShortcutKeys.vue
│     ├─ WorkspaceIndex.vue
│     └─ WorkspaceSettings.vue
├─ src-backend
│  ├─ app.py
│  └─ requirements.txt
├─ src-pwa
│  ├─ custom-service-worker.js
│  ├─ manifest.json
│  ├─ pwa-flag.d.ts
│  └─ register-service-worker.js
├─ src-tauri
│  ├─ Cargo.lock
│  ├─ Cargo.toml
│  ├─ build.rs
│  ├─ capabilities
│  │  ├─ default.json
│  │  └─ desktop.json
│  ├─ icons
│  │  ├─ 128x128.png
│  │  ├─ 128x128@2x.png
│  │  ├─ 32x32.png
│  │  ├─ 64x64.png
│  │  ├─ Square107x107Logo.png
│  │  ├─ Square142x142Logo.png
│  │  ├─ Square150x150Logo.png
│  │  ├─ Square284x284Logo.png
│  │  ├─ Square30x30Logo.png
│  │  ├─ Square310x310Logo.png
│  │  ├─ Square44x44Logo.png
│  │  ├─ Square71x71Logo.png
│  │  ├─ Square89x89Logo.png
│  │  ├─ StoreLogo.png
│  │  ├─ icon.icns
│  │  ├─ icon.ico
│  │  └─ icon.png
│  ├─ src
│  │  ├─ is_deb.rs
│  │  ├─ lib.rs
│  │  ├─ main.rs
│  │  └─ stream.rs
│  └─ tauri.conf.json
├─ tsconfig.json
├─ tsconfig.vue-tsc.json
└─ uno.config.ts

```