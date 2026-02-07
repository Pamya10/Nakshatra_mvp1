# 🏠 Nakshatra Interiors Website

## Welcome!

This is your complete website for Nakshatra Interiors - a modern, professional interior design portfolio and lead generation website.

---

## 📚 Quick Links to Guides

1. **[How to Add Photos & Videos](./HOW_TO_ADD_PHOTOS.md)** - Add your project photos
2. **[Deployment Guide](./DEPLOYMENT_GUIDE.md)** - Put your website online

---

## 🌟 What's Included

### **Pages:**
1. **Home** - Hero, services, process, portfolio preview, USPs
2. **About** - Company story, founders, mission, vision, values
3. **Portfolio** - All your projects in a grid
4. **Project Detail Pages** - Individual project with 8-10 photos + videos
5. **Get Quote** - Pricing information and WhatsApp CTA
6. **Testimonials** - Client reviews
7. **Contact** - Contact form and information

### **Features:**
✅ Mobile-responsive design
✅ Floating WhatsApp button (all pages)
✅ Timed consultation popup (10 seconds)
✅ Portfolio with project detail pages
✅ 6 dummy projects (replace with your own)
✅ Brand colors: Pine Green (#047C74), Chalky (#E7D49E), Brandy Punch (#C68D28)
✅ Your actual logo integrated
✅ Google Forms integration ready

---

## 🎯 What You Need to Do

### **Step 1: Add Your Real Project Photos**

📖 **Follow:** [HOW_TO_ADD_PHOTOS.md](./HOW_TO_ADD_PHOTOS.md)

1. Upload photos to Google Drive/Imgur
2. Edit `/app/frontend/src/data/mockProjects.js`
3. Replace dummy URLs with your photo URLs
4. Add 8-10 photos per project

**File Location:**
```
/app/frontend/src/data/mockProjects.js
```

### **Step 2: Update Google Forms**

Replace placeholder Google Form URLs in:

**File 1:** `/app/frontend/src/components/ConsultationPopup.jsx`
- Line ~49: `const formUrl = 'YOUR_GOOGLE_FORM_URL_HERE';`

**File 2:** `/app/frontend/src/pages/Contact.jsx`
- Line ~52: `window.open('YOUR_GOOGLE_FORM_URL_HERE', '_blank');`

**File 3:** `/app/frontend/src/pages/Home.jsx`
- Line ~430: `const formUrl = 'YOUR_GOOGLE_FORM_URL_HERE';`

### **Step 3: Update Contact Information** (if needed)

Current settings:
- **Phone:** +91 8999100590 / +91 7709596817
- **Email:** interiorsbynakshatra@gmail.com
- **Instagram:** @nakshatra.interior
- **Service Area:** PAN Maharashtra

If any of these need to change, search for them in the code and replace.

### **Step 4: Deploy Your Website**

📖 **Follow:** [DEPLOYMENT_GUIDE.md](./DEPLOYMENT_GUIDE.md)

1. Create GitHub account
2. Upload code to GitHub
3. Create Render account
4. Deploy from GitHub
5. Your website goes live!

---

## 📂 Project Structure

```
/app/
├── frontend/                          # Frontend React app
│   ├── public/
│   │   └── index.html                # Main HTML (title updated)
│   ├── src/
│   │   ├── components/               # Reusable components
│   │   │   ├── Navbar.jsx           # Navigation bar
│   │   │   ├── Footer.jsx           # Footer
│   │   │   ├── WhatsAppButton.jsx   # Floating WhatsApp
│   │   │   └── ConsultationPopup.jsx # Popup form
│   │   ├── pages/                    # Website pages
│   │   │   ├── Home.jsx             # Landing page
│   │   │   ├── About.jsx            # About page
│   │   │   ├── Portfolio.jsx        # Portfolio grid ⭐ NEW
│   │   │   ├── ProjectDetail.jsx    # Project details ⭐ NEW
│   │   │   ├── GetQuote.jsx         # Get quote page
│   │   │   ├── Testimonials.jsx     # Testimonials
│   │   │   └── Contact.jsx          # Contact page
│   │   ├── data/
│   │   │   └── mockProjects.js      # 📸 YOUR PROJECTS HERE ⭐
│   │   ├── App.js                    # Main app
│   │   └── index.css                 # Global styles
│   └── package.json                  # Dependencies
├── HOW_TO_ADD_PHOTOS.md             # 📖 Photo guide
├── DEPLOYMENT_GUIDE.md              # 📖 Deployment guide
└── README.md                         # 📖 This file
```

---

## 🛠️ Tech Stack

- **Frontend:** React 19
- **Styling:** Tailwind CSS
- **UI Components:** Shadcn UI
- **Icons:** Lucide React
- **Routing:** React Router DOM
- **Toasts:** Sonner
- **Deployment:** Render (recommended)

---

## 🎨 Design Guidelines

### **Brand Colors:**
- **Pine Green:** `#047C74` - Primary accent, buttons
- **Chalky:** `#E7D49E` - Light backgrounds, cards
- **Brandy Punch:** `#C68D28` - Secondary accent, hover states

### **Fonts:**
- **Main:** Poppins (Google Fonts)
- **Weights:** 400, 600, 700, 800

### **Design Principles:**
- Clean, minimal, airy
- Ample whitespace
- Mobile-first responsive
- Smooth animations and transitions

---

## 📱 Testing Your Website

### **Locally (Before Deployment):**

The website should already be running at:
```
http://localhost:3000
```

Test these:
- ✅ All pages load
- ✅ Navigation works
- ✅ Portfolio projects open correctly
- ✅ WhatsApp button works
- ✅ Contact form submits
- ✅ Popup appears after 10 seconds
- ✅ Mobile responsive

### **After Deployment:**

1. Open your live URL
2. Test on different devices:
   - Desktop computer
   - Mobile phone
   - Tablet
3. Test all features
4. Share with friends for feedback

---

## 🔧 Making Changes

### **Quick Edits:**

1. Find the file you want to edit
2. Make your changes
3. Save the file
4. Website auto-reloads (if running locally)
5. Commit to GitHub (if deployed)

### **Common Edits:**

**Change Phone Number:**
- Search for: `8999100590`
- Replace all occurrences

**Change Email:**
- Search for: `interiorsbynakshatra@gmail.com`
- Replace all occurrences

**Change Social Media:**
- Search for: `@nakshatra.interior`
- Replace with your handle

**Add/Remove Projects:**
- Edit: `/app/frontend/src/data/mockProjects.js`
- Follow format in existing projects

---

## 📞 Support & Help

### **Need Help?**

1. **Read the guides first:**
   - [How to Add Photos](./HOW_TO_ADD_PHOTOS.md)
   - [Deployment Guide](./DEPLOYMENT_GUIDE.md)

2. **Common issues:**
   - Photos not showing → Check URLs are public
   - Page not loading → Check browser console (F12)
   - Can't deploy → Check GitHub connection

3. **Still stuck?**
   - Check file syntax (commas, quotes)
   - Compare with working examples
   - Try copying a working project and modifying it

---

## 📈 Next Steps After Launch

1. **SEO Optimization:**
   - Submit to Google Search Console
   - Create sitemap.xml
   - Add meta descriptions

2. **Analytics:**
   - Add Google Analytics
   - Track visitor behavior
   - Monitor conversions

3. **Marketing:**
   - Share on social media
   - Add to Google My Business
   - Update Instagram bio
   - Include in email signature

4. **Content Updates:**
   - Add new projects regularly
   - Update testimonials
   - Refresh photos

---

## ✅ Pre-Launch Checklist

Before making your website public:

- [ ] Replaced all dummy projects with real ones
- [ ] Added 8-10 photos per project
- [ ] Updated Google Form URLs
- [ ] Verified WhatsApp number works
- [ ] Tested on mobile device
- [ ] Checked all pages load
- [ ] Verified all links work
- [ ] Updated contact information
- [ ] Added real testimonials
- [ ] Tested consultation popup
- [ ] Verified footer information
- [ ] Checked portfolio page
- [ ] Tested project detail pages

---

## 🎉 Success!

Your website is professional, modern, and ready to generate leads for Nakshatra Interiors!

**What You Have:**
- ✅ Professional 7-page website
- ✅ Portfolio with project galleries
- ✅ Lead capture via WhatsApp & forms
- ✅ Mobile-responsive design
- ✅ Your actual branding & logo
- ✅ Easy to update and maintain

**Share Your Website:**
```
🌐 Website: nakshtrainterior.com
📱 WhatsApp: +91 8999100590
📧 Email: interiorsbynakshatra@gmail.com
📸 Instagram: @nakshatra.interior
```

---

## 📝 Version History

**Version 1.0** - December 2025
- Initial website launch
- 7 pages implemented
- Portfolio system with detail pages
- 6 dummy projects included
- WhatsApp integration
- Consultation popup
- Mobile-responsive
- Brand colors & logo integrated

---

## 📄 License

© 2025 Nakshatra Interiors. All rights reserved.

---

**Built with ❤️ for Nakshatra Interiors**

*"Adding aesthetics to life"*
