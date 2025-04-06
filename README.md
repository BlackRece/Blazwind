# BlazWind - Blazor & TailwindCSS Fusion

[![.NET](https://img.shields.io/badge/.NET-6.0-purple)](https://dotnet.microsoft.com/)
[![Blazor](https://img.shields.io/badge/Blazor-WebAssembly-blue)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.3.0-06B6D4)](https://tailwindcss.com/)

**BlazWind** is an experimental project that merges Microsoft's Blazor framework with TailwindCSS to explore modern full-stack C# development with utility-first CSS.

## 🚩 Why BlazWind?

This repository demonstrates:
- Seamless integration of TailwindCSS in Blazor applications
- Modern UI development using C#/Razor syntax
- Performance considerations for CSS/JS in WASM environment
- Component-driven design system implementation

## 🎮 Quick Start

1. Clone the repo:
   ```bash
   git clone https://github.com/BlackRece/Blazwind.git
   cd Blazwind
   ```
2. One-time setup:
   ```bash
    dotnet restore && npm install
   ```
3. Development mode:
    ```bash
    dotnet run & npm run watch-tailwind
   ```
   
## 🌟 Highlighted Components
- ThemeSwitcher.razor - Dynamic dark/light mode toggle
- ResponsiveNav.razor - Mobile-first navigation with Tailwind breakpoints
- DataCard.razor - Reusable dashboard card component
- InteractiveChart.razor - SVG-based visualization component

## 📂 Project Structure
```text
BlazWind/
├── BlazWind.Client/     # Blazor WebAssembly core
├── BlazWind.Server/     # ASP.NET Core host
├── Tailwind/            # CSS configuration hub
│   ├── base.css         # Custom CSS variables
│   ├── components.css   # Custom component classes
│   └── utilities.css    # Extended Tailwind classes
├── SharedComponents/    # UI component library
└── Styles/              # PostCSS processing pipeline
```
## ⚡ Performance Notes
- CSS Size: Production build purges to ~12KB 
- WASM Load: First-load time ~1.8s (dev mode)
- Hot Reload: Combined CSS/Razor hot reload support

## 🧑💻 Development Workflow
- Create new component in SharedComponents/ 
- Add component-specific styles in Tailwind/components.css
- Reference in pages using:
```razor
<NewComponent class="bg-blazor-purple/10 hover:scale-105 transition-transform"/>
```
## 🚨 Common Issues
- Class Conflicts: Use @layer directives in CSS files
- Missing Styles: Ensure JIT watch is running
- Build Errors: Run npm run refresh-deps to reset CSS pipeline

## 📈 Next Steps
- Add authentication flow
- Implement dark mode persistence
- Create component library export
- Add e2e testing with Playwright

## 📄 License

MIT License - [View LICENSE](LICENSE)   

**Required Attribution:**  
```text
Copyright © 2025 BlackRece (BlazWind - https://github.com/BlackRece/Blazwind)
```

## 🚫 Contribution Policy

**This repository is maintained exclusively by its author**:
- Pull requests will not be reviewed or accepted
- Code contributions from others are not permitted
- The codebase will only be modified by the owner

**We welcome**:
- Bug reports
- Feature suggestions
- Usage questions
- Documentation feedback

Please open an Issue for any specific discussions.