# 🚀 Reethesh Portfolio Website

A modern, fully responsive portfolio website showcasing full-stack development, data analytics, and AI projects. Built with React, TypeScript, and GSAP animations for a smooth, professional user experience.

![Portfolio Preview](https://img.shields.io/badge/Status-Live-success)
![React](https://img.shields.io/badge/React-19.2.0-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5.9.3-blue)
![Vite](https://img.shields.io/badge/Vite-7.2.4-purple)

## ✨ Features

### 🎨 Design & UI
- **Modern Dark Theme** with violet/purple gradient accents
- **Fully Responsive** - Optimized for mobile, tablet, and desktop
- **Smooth Animations** - GSAP-powered scroll animations and transitions
- **3D Elements** - Rotating project cylinder showcase
- **Custom Cursor** - Interactive cursor effects
- **Gradient Blobs** - Animated background elements

### 📱 Mobile Optimized
- Fast fade-in animations (0.3-0.4s duration)
- Touch-friendly interactions
- Optimized scroll triggers (95% viewport)
- No blur effects for better performance
- Responsive typography and spacing

### 🎯 Sections
1. **Hero Section** - Dynamic typing animation, orbital rings, tech stack badges
2. **Quote Section** - Parallax scrolling quote with background images
3. **About Section** - Pinned portrait with scrolling content (desktop)
4. **Experience Section** - Expandable internship cards
5. **Projects Section** - 3D rotating cylinder with 10 featured projects
6. **Skills Section** - Animated progress bars and specialty cards
7. **Certifications Section** - Industry-recognized credentials
8. **Contact Section** - Social links and contact information

## 🛠️ Tech Stack

### Frontend
- **React 19.2.0** - UI library
- **TypeScript 5.9.3** - Type safety
- **Vite 7.2.4** - Build tool & dev server
- **Tailwind CSS 3.4.19** - Utility-first CSS
- **GSAP 3.15.0** - Animation library
- **Lenis 1.3.23** - Smooth scroll

### UI Components
- **Radix UI** - Accessible component primitives
- **Lucide React** - Icon library
- **Shadcn/ui** - Component collection

### Additional Libraries
- **React Hook Form** - Form management
- **Zod** - Schema validation
- **Three.js** - 3D graphics (if needed)
- **Recharts** - Data visualization

## 📂 Project Structure

```
├── public/
│   └── assets/          # Project images, portraits, quotes
├── src/
│   ├── components/      # Reusable components
│   │   ├── ui/         # Shadcn UI components
│   │   ├── CustomCursor.tsx
│   │   ├── Footer.tsx
│   │   ├── GradientBlobs.tsx
│   │   ├── LoadingScreen.tsx
│   │   ├── Navigation.tsx
│   │   ├── NeonGlowCard.tsx
│   │   ├── SectionDivider.tsx
│   │   └── SectionLabel.tsx
│   ├── hooks/          # Custom React hooks
│   │   ├── use-mobile.ts
│   │   ├── useLenis.ts
│   │   └── useScrollEntrance.ts
│   ├── lib/            # Utility functions
│   │   └── utils.ts
│   ├── pages/          # Page components
│   │   └── Home.tsx
│   ├── sections/       # Main sections
│   │   ├── AboutSection.tsx
│   │   ├── CertificationsSection.tsx
│   │   ├── ContactSection.tsx
│   │   ├── ExperienceSection.tsx
│   │   ├── HeroSection.tsx
│   │   ├── ProjectsSection.tsx
│   │   ├── QuoteSection.tsx
│   │   └── SkillsSection.tsx
│   ├── App.tsx         # Main app component
│   ├── main.tsx        # Entry point
│   └── index.css       # Global styles
├── index.html
├── package.json
├── tailwind.config.js
├── tsconfig.json
└── vite.config.ts
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/rxth7/portfolio.git
cd portfolio
```

2. **Install dependencies**
```bash
npm install
```

3. **Start development server**
```bash
npm run dev
```

The site will be available at `http://localhost:3000`

### Build for Production

```bash
npm run build
```

The optimized build will be in the `dist/` folder.

### Preview Production Build

```bash
npm run preview
```

## 📋 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

## 🎨 Customization

### Colors
Edit `tailwind.config.js` to customize the color scheme:
```js
colors: {
  violet: { /* ... */ },
  purple: { /* ... */ }
}
```

### Animations
Adjust animation speeds in section files:
```typescript
duration: 0.3,  // Animation duration in seconds
ease: 'power2.out',  // Easing function
```

### Content
Update personal information in:
- `src/sections/HeroSection.tsx` - Name, title, bio
- `src/sections/ProjectsSection.tsx` - Projects array
- `src/sections/ExperienceSection.tsx` - Work experience
- `src/sections/SkillsSection.tsx` - Skills and expertise

## 📱 Mobile Optimization

The website is fully optimized for mobile devices with:
- Responsive breakpoints: `sm` (640px), `md` (768px), `lg` (1024px)
- Fast animations (0.3-0.4s)
- Touch-optimized interactions
- Reduced motion for better performance
- Adaptive layouts and typography

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Reethesh Shettigar**
- GitHub: [@rxth7](https://github.com/rxth7)
- LinkedIn: [Reethesh Shettigar](https://linkedin.com/in/reethesh-shettigar)
- Email: ritheshshettigar46@gmail.com
- Website: [Portfolio](https://your-domain.com)

## 🙏 Acknowledgments

- [GSAP](https://greensock.com/gsap/) - Animation library
- [Lenis](https://lenis.studiofreight.com/) - Smooth scroll
- [Radix UI](https://www.radix-ui.com/) - UI primitives
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework
- [Shadcn/ui](https://ui.shadcn.com/) - Component library

## 📊 Performance

- **Lighthouse Score**: 95+ (Performance, Accessibility, Best Practices, SEO)
- **Bundle Size**: 
  - CSS: 92 KB (15.5 KB gzipped)
  - JS: 431 KB (137 KB gzipped)
- **First Contentful Paint**: < 1.5s
- **Time to Interactive**: < 3s

## 🔧 Troubleshooting

### Development server not starting
```bash
# Clear node_modules and reinstall
rm -rf node_modules package-lock.json
npm install
```

### Build errors
```bash
# Clear cache and rebuild
npm run build -- --force
```

## 📝 Changelog

### Version 1.0.0 (2026)
- Initial release
- Fully responsive design
- 10 featured projects
- Smooth scroll animations
- Mobile optimizations

---

⭐ **Star this repo** if you find it helpful!

Made with ❤️ by Reethesh Shettigar
