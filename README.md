# 🚨 Disaster Prep Quiz

**Are you ready for an emergency? Take the 5-minute quiz and find out.**

Affiliate-driven disaster preparedness quiz designed to go viral and generate income through Amazon Associates and insurance lead generation.

## 🎯 Project Status

### ✅ MVP Complete (Week 1)
- [x] 20-question quiz across 5 categories (Water, Food, Shelter, Communications, Medical)
- [x] Scoring algorithm (0-100% with 5 readiness levels)
- [x] Gap analysis by category
- [x] Product recommendations (50+ products with Amazon links)
- [x] Responsive single-page app
- [x] Email capture form
- [x] Social sharing buttons
- [x] GitHub Pages deployment

### 🚧 In Progress
- [ ] Amazon Associates account setup
- [ ] Replace placeholder affiliate tag (`YOUR-AFFILIATE-ID`) with real tag
- [ ] Email service integration (Mailchimp/ConvertKit)
- [ ] Custom domain setup (suggested: preparedquiz.com)
- [ ] Analytics integration

### 📋 Launch Checklist (Week 2)
- [ ] Test all affiliate links
- [ ] Create social sharing graphics
- [ ] Write launch posts for Reddit (r/preppers, r/homestead, r/Survival)
- [ ] Set up email autoresponder with free checklist PDF
- [ ] Facebook ads test budget ($50)
- [ ] Partner outreach (prep bloggers/YouTubers)

## 🌐 Live URL

**Demo:** https://fullstackkevinvandriel.github.io/DisasterPrepQuiz/disaster-prep.html

## 📁 Key Files

- `disaster-prep.html` - Main quiz interface (single-page app)
- `disaster-prep-quiz.json` - Quiz data (questions, products, scoring)

## 💰 Revenue Model

### Affiliate Opportunities
- **Amazon Associates:** 4-8% commission on emergency supplies
  - Average commission per quiz-taker: $5-$10 (assumes 2-3 product purchases)
- **Insurance comparison leads:** $20-$50 per quote submitted
- **Prep brand affiliates:** 10-20% commission on specialty products

### Target Metrics
- Month 1: $500 (100 quiz-takers, 2% buy rate)
- Month 3: $1,500 (300 quiz-takers)
- Month 6: $2,500 (500 quiz-takers)
- **September spike:** 5-10x during National Preparedness Month

## 🎯 Marketing Strategy

### Launch Channels
1. **Reddit:** r/preppers (800K members), r/homestead, r/Survival
2. **Facebook groups:** Preparedness, homesteading
3. **NextDoor:** "Is your neighborhood prepared?"
4. **Pinterest:** Preparedness checklists (huge audience)

### SEO Targets
- "emergency preparedness checklist 2026"
- "are you ready for an emergency quiz"
- "disaster preparedness test"

### Viral Hooks
- "Only 23% of Americans are prepared for a 3-day emergency"
- "Take the 5-minute quiz everyone's sharing"
- Social proof: "47,392 people have taken this quiz"

## 🛠️ Setup Instructions

### 1. Amazon Associates
1. Sign up at https://affiliate-program.amazon.com/
2. Get your affiliate tag (e.g., `yourname-20`)
3. Replace `YOUR-AFFILIATE-ID` in `disaster-prep.html` (line ~435)

### 2. Email Service Integration
Current placeholder: `console.log('Email submitted:', email)`

**Option A: Mailchimp**
```javascript
fetch('https://YOUR-MAILCHIMP-SERVER.us1.list-manage.com/subscribe/post-json?u=XXX&id=YYY', {
    method: 'POST',
    body: JSON.stringify({ EMAIL: email }),
    mode: 'no-cors'
});
```

**Option B: ConvertKit**
```javascript
fetch('https://api.convertkit.com/v3/forms/YOUR-FORM-ID/subscribe', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email: email, api_key: 'YOUR-API-KEY' })
});
```

### 3. Custom Domain (Optional)
1. Register domain (e.g., preparedquiz.com)
2. Add CNAME record: `www` → `fullstackkevinvandriel.github.io`
3. Update GitHub Pages settings with custom domain

## 📊 Product Database

50+ products across categories:
- **Water:** Storage containers, filters, purification tablets
- **Food:** Emergency food buckets, MREs, freeze-dried meals
- **Shelter:** Blankets, tarps, sleeping bags, generators
- **Communications:** Emergency radios, solar chargers, power banks
- **Medical:** First aid kits, prescription storage, training courses
- **Documents:** Fireproof bags, insurance (lead gen opportunity)

All products include:
- Amazon affiliate links
- Price estimates
- Expected commission ($0.50 - $15 per item)

## 🚀 Quick Deploy

```bash
# Clone and deploy
git clone https://github.com/FullStackKevinVanDriel/DisasterPrepQuiz.git
cd DisasterPrepQuiz

# Update affiliate tag in disaster-prep.html
sed -i '' 's/YOUR-AFFILIATE-ID/yourname-20/g' disaster-prep.html

# Commit and push
git add disaster-prep.html
git commit -m "Add Amazon affiliate tag"
git push

# GitHub Pages will auto-deploy in ~2 minutes
```

## 🎨 Branding

- **Icon:** 🚨 (emergency siren)
- **Colors:** Purple gradient (#667eea → #764ba2)
- **CTA Color:** Red (#ff6b6b)
- **Vibe:** Urgent but friendly, practical not fear-mongering

## 📈 Future Enhancements

- Add quiz keyword system (reuse QuizMyself engine for multiple quiz topics)
- Insurance lead generation form integration
- PDF checklist generator (email lead magnet)
- State-specific disaster prep (earthquakes, hurricanes, wildfires)
- WordPress plugin version for bloggers
- Mobile app

## 🔗 Related Projects

- **QuizMyself:** Core quiz engine used as foundation
- **Transit Route Planner:** WordPress plugin with similar license/payment model

## 📄 License

MIT - Feel free to fork and customize

---

**Built by Kevin VanDriel** | Vandromeda | February 2026
