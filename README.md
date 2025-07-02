# 🛍️ ShopAI - Smart Shopping Price Comparison Platform

<div align="center">

![ShopAI Logo](https://via.placeholder.com/120x120/ec4899/ffffff?text=ShopAI)

**An intelligent price comparison platform for makeup and skincare enthusiasts**

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Next.js](https://img.shields.io/badge/Next.js-14.0-black?logo=next.js)](https://nextjs.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104-green?logo=fastapi)](https://fastapi.tiangolo.com/)
[![Docker](https://img.shields.io/badge/Docker-Ready-blue?logo=docker)](https://www.docker.com/)
[![Free Deployment](https://img.shields.io/badge/Deployment-100%25%20Free-brightgreen)](./FREE_DEPLOYMENT.md)

[🚀 Live Demo](http://localhost:3000) • [📖 Documentation](./FREE_DEPLOYMENT.md) • [🤝 Contributing](#-contributing) • [💰 Cost Breakdown](./COST_BREAKDOWN.md)

</div>

---

## 🌟 **Why ShopAI?**

Ever tired of manually checking Nykaa, Myntra, Amazon, and Flipkart for the best beauty product prices? **ShopAI automates this for you!** 

✨ **Compare prices across multiple platforms**  
📍 **Location-based pricing with pincode**  
📊 **Price history and trend tracking**  
🚨 **Smart price alerts**  
🆓 **Completely free to build, deploy, and use**

---

## 🎯 **Features**

| Feature | Status | Description |
|---------|---------|-------------|
| 🔍 **Smart Search** | ✅ Ready | AI-powered product search across platforms |
| 💰 **Price Comparison** | ✅ Ready | Real-time price comparison with best deal finder |
| 📍 **Location Pricing** | ✅ Ready | Pincode-based pricing and delivery costs |
| 📊 **Price History** | ✅ Ready | Track price trends over time |
| 🚨 **Price Alerts** | 🚧 Coming Soon | Get notified when prices drop |
| 👤 **User Accounts** | 🚧 Coming Soon | Save favorites and manage alerts |
| 📱 **Mobile App** | ⏳ Planned | React Native mobile application |

---

## 🆓 **100% Free Tech Stack**

### **Frontend**
- **Next.js 14** - React framework with App Router
- **TypeScript** - Type safety and better DX
- **Tailwind CSS** - Utility-first CSS framework
- **Heroicons** - Beautiful SVG icons

### **Backend**
- **FastAPI** - Modern Python web framework
- **PostgreSQL** - Robust relational database
- **Redis** - High-performance caching
- **Celery** - Background task processing
- **SQLAlchemy** - Python SQL toolkit and ORM

### **Web Scraping**
- **BeautifulSoup** - HTML parsing
- **Scrapy** - Web crawling framework
- **Selenium** - Browser automation (when needed)

### **Free Deployment Options**
- **Railway** - Backend + Database (FREE tier)
- **Vercel** - Frontend hosting (FREE tier)
- **Supabase** - Alternative database (FREE tier)
- **Render** - Alternative backend hosting (FREE tier)

**💡 Total Monthly Cost: $0 forever!**

---

## 🚀 **Quick Start**

### **⚡ One-Command Setup**

```bash
# Clone the repository
git clone https://github.com/yourusername/ShopAI.git
cd ShopAI

# For macOS/Linux
./start.sh

# For Windows
start.bat

# Or manually with Docker
docker-compose up -d
```

**🎉 That's it! Visit [http://localhost:3000](http://localhost:3000)**

### **📱 What You'll See**

- Beautiful, responsive shopping interface
- Smart product search functionality
- Category browsing (Skincare, Makeup, Fragrance, etc.)
- Popular search suggestions
- Professional gradient design

---

## 🏗️ **Project Structure**

```
ShopAI/
├── 📱 frontend/                 # Next.js React application
│   ├── src/
│   │   ├── app/                # App router pages
│   │   ├── components/         # Reusable React components
│   │   └── lib/               # Utilities and helpers
│   ├── package.json
│   └── Dockerfile
├── 🔧 backend/                 # FastAPI Python application
│   ├── app/
│   │   ├── api/               # API routes and endpoints
│   │   ├── core/              # Core functionality
│   │   ├── db/                # Database models and config
│   │   ├── scrapers/          # Web scraping modules
│   │   └── services/          # Business logic
│   ├── requirements.txt
│   └── Dockerfile
├── 🐳 docker-compose.yml       # Multi-service Docker setup
├── 📚 docs/                    # Documentation files
│   ├── FREE_DEPLOYMENT.md     # Deployment guides
│   ├── QUICK_START.md         # Quick reference
│   └── COST_BREAKDOWN.md      # Cost analysis
├── start.sh / start.bat        # Quick start scripts
└── README.md                   # This file
```

---

## 🔧 **Development Setup**

### **Prerequisites**
- **Node.js 18+** (for frontend)
- **Python 3.9+** (for backend)
- **Docker & Docker Compose** (recommended)
- **Git** (for version control)

### **Local Development**

1. **Frontend Only** (Quick Preview)
   ```bash
   cd frontend
   npm install
   npm run dev
   # Visit http://localhost:3000
   ```

2. **Full Stack** (Backend + Frontend + Database)
   ```bash
   # Copy environment files
   cp backend/env.example backend/.env
   cp frontend/env.example frontend/.env.local
   
   # Start all services
   docker-compose up -d
   ```

3. **Manual Setup** (Without Docker)
   ```bash
   # Backend
   cd backend
   python -m venv venv
   source venv/bin/activate  # Windows: venv\Scripts\activate
   pip install -r requirements.txt
   python init_db.py
   uvicorn app.main:app --reload
   
   # Frontend (new terminal)
   cd frontend
   npm install
   npm run dev
   ```

### **Environment Variables**

**Backend (.env)**
```bash
DATABASE_URL=postgresql://shopai:password@localhost:5432/shopai
REDIS_URL=redis://localhost:6379
SECRET_KEY=your-secret-key-change-this-in-production
BACKEND_CORS_ORIGINS=["http://localhost:3000"]
```

**Frontend (.env.local)**
```bash
NEXT_PUBLIC_API_URL=http://localhost:8000
```

---

## 🌐 **Free Deployment**

### **🎯 Recommended: Railway + Vercel**
**Total Cost: $0/month**

1. **Deploy Backend to Railway**
   - Visit [railway.app](https://railway.app)
   - Connect your GitHub repository
   - Add PostgreSQL and Redis services
   - Deploy automatically

2. **Deploy Frontend to Vercel**
   ```bash
   cd frontend
   npx vercel
   # Follow the prompts
   ```

### **🏗️ Alternative: Oracle Cloud**
**Total Cost: $0/month forever**

- Get Oracle Cloud Always Free tier (1GB RAM, 2 CPUs)
- Deploy using Docker Compose
- Set up free domain with Cloudflare

**📖 See [FREE_DEPLOYMENT.md](./FREE_DEPLOYMENT.md) for detailed step-by-step guides**

---

## 🤝 **Contributing**

We welcome contributions from developers of all levels! Here's how you can help:

### **🎯 Priority Areas**
- **Web Scrapers**: Add support for more stores (Myntra, Amazon, Flipkart)
- **Price Alerts**: Implement email/SMS notifications
- **User Authentication**: Add login/signup functionality
- **Mobile App**: React Native implementation
- **Performance**: Optimize scraping and API performance
- **Testing**: Add unit and integration tests

### **🚀 Getting Started**

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make your changes**
4. **Test locally**
   ```bash
   docker-compose up -d
   # Test your changes
   ```
5. **Commit and push**
   ```bash
   git commit -m "Add amazing feature"
   git push origin feature/amazing-feature
   ```
6. **Open a Pull Request**

### **📋 Contribution Guidelines**

- **Code Style**: Follow existing patterns and use TypeScript/Python type hints
- **Documentation**: Update README and add comments for complex logic
- **Testing**: Test your changes locally before submitting
- **Commits**: Use clear, descriptive commit messages
- **Issues**: Check existing issues before creating new ones

---

## 📊 **Free Tier Limits**

| Service | Free Tier | Limits | Perfect For |
|---------|-----------|--------|-------------|
| **Railway** | ✅ | 512MB RAM, $5 credit/month | ~1000 API requests/day |
| **Vercel** | ✅ | 100GB bandwidth/month | Millions of page views |
| **Supabase** | ✅ | 500MB database, 2 CPU hours | Early development |
| **GitHub Codespaces** | ✅ | 60 hours/month | Cloud development |

**🎯 These limits are perfect for MVP, testing, and early users!**

---

## 🛣️ **Roadmap**

### **Phase 1: Foundation** ✅
- [x] Beautiful responsive frontend
- [x] Complete API structure
- [x] Database models and relationships
- [x] Docker containerization
- [x] Free deployment guides

### **Phase 2: Core Features** 🚧
- [ ] Real-time web scraping for all major stores
- [ ] Price history visualization
- [ ] User authentication and profiles
- [ ] Price alert system with notifications
- [ ] Advanced search filters

### **Phase 3: Enhancement** ⏳
- [ ] Mobile app (React Native)
- [ ] Chrome extension
- [ ] Advanced analytics and recommendations
- [ ] Wishlist and favorites
- [ ] Social sharing features

### **Phase 4: Scale** 🔮
- [ ] API for third-party developers
- [ ] Affiliate program integration
- [ ] Advanced scraping with ML
- [ ] Multi-language support
- [ ] iOS/Android native apps

---

## 📸 **Screenshots**

<div align="center">

### **Homepage**
![Homepage](https://via.placeholder.com/800x600/f8fafc/374151?text=Beautiful+Homepage+with+Search)

### **Search Results**
![Search Results](https://via.placeholder.com/800x600/f8fafc/374151?text=Price+Comparison+Results)

### **Product Details**
![Product Details](https://via.placeholder.com/800x600/f8fafc/374151?text=Detailed+Product+View)

</div>

---

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**TL;DR**: You can use this project for anything, including commercial purposes, for free!

---

## 🙏 **Acknowledgments**

- **Open Source Community** - For amazing free tools and libraries
- **Beauty Enthusiasts** - For inspiring this project
- **Contributors** - For making this project better
- **Free Tier Providers** - Railway, Vercel, Supabase for generous free tiers

---

## 📞 **Support**

- **📖 Documentation**: Check our [guides](./docs/)
- **🐛 Bug Reports**: [Create an issue](https://github.com/yourusername/ShopAI/issues)
- **💡 Feature Requests**: [Start a discussion](https://github.com/yourusername/ShopAI/discussions)
- **❓ Questions**: [Ask in discussions](https://github.com/yourusername/ShopAI/discussions)

---

## ⭐ **Star History**

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=yourusername/ShopAI&type=Date)](https://star-history.com/#yourusername/ShopAI&Date)

**If this project helped you, please consider giving it a ⭐!**

</div>

---

<div align="center">

**Built with ❤️ by the community**

[🚀 Deploy for Free](./FREE_DEPLOYMENT.md) • [🤝 Contribute](CONTRIBUTING.md) • [💰 $0 Cost Breakdown](./COST_BREAKDOWN.md)

</div>
