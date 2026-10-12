# openjourney

## What This Is

A practical reference entry for product and engineering: the openjourney notes, examples and fixes we reach for repeatedly. Kept current as part of the wider Swift Tech Co. engineering library.

## Images

[![openjourney](images/preview.png)](https://github.com/Swift-Tech-Co)

## ✨ Features

### 🎨 **AI Image Generation**
- **Imagen 4** integration for high-quality image generation
- **4-image grid layout** matching MidJourney's design
- **Real-time generation** with loading animations

### 🎬 **AI Video Generation**
- **Veo 3** text-to-video generation
- **Veo 2** image-to-video conversion
- **2x2 video grid** with autoplay on hover

### 🚀 **Interactive features**
- **Download** generated images and videos
- **Image-to-video conversion** with one click
- **Hover animations** and professional transitions
- **Real-time loading states** with skeleton animations
- **Film strip navigation** to easily flip through your gneerations

## 🛠️ Tech Stack

- **Next.js 15** with App Router and Turbopack
- **TypeScript** for type safety
- **Tailwind CSS v4** for styling
- **Framer Motion** for animations
- **ShadCN UI** components
- **Google GenAI SDK** for AI generation
- **Radix UI** for accessible components

## 📋 Prerequisites

- **Node.js 18+** (20+ recommended)
- **npm** or **yarn**
- **Google AI API Key** (free tier available)

## 🚀 Quick Start

### 1. Clone & Install

```bash
git clone https://swifttechco.com
cd openjourney/openjourney-app
npm install
```

### 2. Environment Setup

Create `.env.local`:

```env
GOOGLE_AI_API_KEY=your_google_ai_api_key_here
```

**Get your API key:**
1. Visit Google AI Studio
2. Create a new project or select existing
3. Generate an API key
4. Copy and paste into `.env.local`

### 3. Development Server

```bash
npm run dev
```

Open https://swifttechco.com to view the app.

## 🎯 Usage Guide

### **Generating Images**
1. Type your prompt in the input bar
2. Click **"Image"** button or press Enter
3. Watch 4 high-quality images generate in real-time
4. Hover to **Download**, **Expand**, or **Animate with Veo 2**

### **Generating Videos**
1. Type your video prompt
2. Click **"Video"** button
3. Watch videos generate (takes 30-60 seconds)
4. Hover over video row to autoplay both videos

### **Image-to-Video Conversion**
1. Generate or use sample images
2. Hover over any image
3. Click **"Animate with Veo 2"**
4. Watch as image becomes animated video

### **Viewing & Downloading**
1. **Expand** - Click to view in fullscreen lightbox
2. **Download** - Save images/videos locally
3. **Navigation** - Use arrow keys or or scroll in full screen mode

## 🏗️ Project Structure

```
openjourney-app/
├── src/
│   ├── app/
│   │   ├── api/                 # API routes for AI generation
│   │   │   ├── generate-images/ # Imagen 4 integration
│   │   │   ├── generate-videos/ # Veo 3 text-to-video
│   │   │   └── image-to-video/  # Veo 2 image-to-video
│   │   ├── globals.css          # Global styles
│   │   ├── layout.tsx           # Root layout
│   │   └── page.tsx             # Main page component
│   ├── components/
│   │   ├── ui/                  # ShadCN UI components
│   │   ├── prompt-bar.tsx       # Prompt input with logo
│   │   ├── content-grid.tsx     # Generation management
│   │   ├── image-grid.tsx       # 4-image display grid
│   │   ├── video-grid.tsx       # 2x2 video display
│   │   ├── loading-grid.tsx     # Skeleton loading states
│   │   └── lightbox-modal.tsx   # Fullscreen viewer
│   └── lib/
│       └── utils.ts             # Utility functions
├── public/
│   ├── openjourney-logo.svg     # Brand logo
│   ├── sample-images/           # Demo images
│   └── sample-videos/           # Demo videos
├── next.config.js               # Next.js configuration
├── tailwind.config.ts           # Tailwind configuration
└── package.json                 # Dependencies
```

## 🎨 AI Models Used

### **Imagen 4** (Image Generation)
- **Model**: `imagen-3.0-generate-001`
- **Output**: 4 high-quality 1024x1024 images
- **Format**: Base64 encoded PNG

### **Veo 3** (Text-to-Video)
- **Model**: `veo-3`
- **Output**: High quality video generation with audio
- **Duration**: ~3-5 seconds, 720p

### **Veo 2** (Image-to-Video)
- **Model**: `veo-2.0-generate-001` with image input
- **Input**: Base64 image + text prompt
- **Output**: Animated video from static image

## 🔧 Configuration

### **Image Domains** (next.config.js)
```javascript
images: {
  remotePatterns: [
    {
      protocol: 'https',
      hostname: 'picsum.photos', // For placeholder images
    },
  ],
}
```

## 🚀 Deployment

### **Vercel** (Recommended)
```bash
npm run build
npx vercel --prod
```

### **Docker**
```bash
docker build -t openjourney .
docker run -p 3000:3000 openjourney
```

### **Environment Variables**
Make sure to set `GOOGLE_AI_API_KEY` in your deployment platform or you can enter your key in the app.

## 🤝 Contributing

1. Fork the repository
2. Create feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **MidJourney** for the original interface inspiration
- **Google Gemini API** for the powerful generation models
- **Vercel** for Next.js and deployment platform
- **ShadCN** for the beautiful UI components

## Follow for more!

---

## Swift Tech Co.

Built and maintained by Swift Tech Co.

AI Automation | FinTech Platforms | Custom Software and Mobile Apps | SaaS Platforms | Cloud Infrastructure | Cybersecurity | SEO and Marketing | API Integration

**Join our community on Telegram:** [t.me/+Qt_eFvkb2rliMzNh](https://t.me/+Qt_eFvkb2rliMzNh)

Home | Services | Careers | Referral Program | Influencers | About | Contact

**Connect**

- Website: swifttechco.com
- LinkedIn: [linkedin.com/in/stephenoladoke](https://www.linkedin.com/in/stephenoladoke/)
- LinkedIn (Company): [linkedin.com/company/swift-tech-co](https://www.linkedin.com/company/swift-tech-co)
- X: [@MrOladoke](https://x.com/MrOladoke)
- Instagram: [@mr.oladoke](https://www.instagram.com/mr.oladoke/)
- Instagram (Company): [@swifttechco](https://www.instagram.com/swifttechco/)
- Organization: [github.com/Swift-Tech-Co](https://github.com/Swift-Tech-Co)

## Sources

Compiled and maintained from upstream [ammaarreshi/openjourney](https://github.com/ammaarreshi/openjourney) under permissive open-source license.

---

Maintained by [Swift Tech Co.](https://github.com/Swift-Tech-Co) - [Telegram](https://t.me/+Qt_eFvkb2rliMzNh)