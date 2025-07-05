# Personal Portfolio

This portfolio is a modified version of [dillionverma/portfolio](https://github.com/dillionverma/portfolio).

Built with Next.js, shadcn/ui, and magic ui, originally deployed on Vercel and now optimized for GitHub Pages deployment.

Includes:
- An interactive world map to highlight countries I've visited
- A real-time GitHub contribution graph
- An interactive 3D Rubik's Cube

## ✨ Features

- **Interactive World Map**: Highlights countries visited, with zoom, pan, and hover effects
- **GitHub Contribution Graph**: Real-time GitHub activity visualization
- **Interactive 3D Rubik's Cube**: Built with Three.js and React Three Fiber
- **Responsive Design**: Optimized for all devices
- **Dark/Light Mode**: Built-in theme switching
- **Blog Support**: MDX-based blog with markdown support
- **Smooth Animations**: Powered by Framer Motion and Magic UI

## 🛠️ Tech Stack

- **Framework**: Next.js 14, React 18
- **Language**: TypeScript
- **Styling**: Tailwind CSS, shadcn/ui
- **Animations**: Framer Motion, Magic UI
- **Icons**: Lucide React
- **Content**: MDX
- **Deployment**: GitHub Actions
- **Package Manager**: pnpm

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- pnpm

### Installation
```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
pnpm install
pnpm dev
```

## ⚙️ Configuration

### World Map

- The map uses a local GeoJSON file: `public/world-countries.json`.
- To highlight countries, edit the `visitedCountries` array in `src/components/world-map.tsx` and add the ISO A3 codes (e.g., "USA", "CHN").
- You can update the GeoJSON file if you want to use a different map or add more features.

### GitHub Contribution Graph

1. **Create Personal Access Token**:
   - GitHub Settings → Developer Settings → Personal Access Tokens → Tokens (classic)
   - Generate token with `read:user` and `read:email` scopes

2. **Local Development**:
   - Create `.env.local` in project root
   - Add: `NEXT_PUBLIC_GITHUB_TOKEN=your_token_here`

3. **GitHub Pages Deployment**:
   - Repository Settings → Secrets and Variables → Actions
   - Create secret: `PERSONAL_ACCESS_TOKEN`
   - Set value to your GitHub token

4. **Update Username**:
   - Edit `src/app/page.tsx`
   - Change username in `<GitHubContributions username="your_username" />`

### 3D Rubik's Cube Solver

**Features:**
- Interactive 3D cube with realistic rendering
- Mouse controls for rotation
- Step-by-step solving animation
- Scrambled state generation
- Visual solving process

**Customization:**
- Modify solving steps in `src/components/rubiks-cube.tsx`
- Adjust colors and animation timing
- Add complex solving algorithms

## 📝 License

This project is based on [dillionverma/portfolio](https://github.com/dillionverma/portfolio) and modified for personal use.

