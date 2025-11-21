# ⚡ **NETLIFY - QUICK REFERENCE**

## 🎯 **3-STEP DEPLOYMENT**

```
1. PUSH TO GITHUB
   └─→ Use #github-push tool OR git push

2. CONNECT TO NETLIFY
   └─→ app.netlify.com → Import from GitHub

3. ADD CUSTOM DOMAIN
   └─→ Domain settings → Add www.supergrc.com
```

---

## 📁 **KEY FILES**

| File | Purpose | Location |
|------|---------|----------|
| `netlify.toml` | Main config | `/netlify.toml` |
| `_redirects` | SPA routing | `/public/_redirects` |
| `logo-full.svg` | Logo file | `/public/logo-full.svg` |

---

## ⚙️ **BUILD SETTINGS**

```toml
Build command:     npm run build
Publish directory: dist
Node version:      18
```

*Auto-detected from netlify.toml - no manual config needed!*

---

## 🌐 **DNS CONFIGURATION**

### **Option 1: Netlify DNS** (Recommended)
Update nameservers at your registrar:
```
dns1.p01.nsone.net
dns2.p01.nsone.net
dns3.p01.nsone.net
dns4.p01.nsone.net
```

### **Option 2: External DNS**
Add these records:
```
Type    Name    Value
A       @       75.2.60.5
AAAA    @       2600:4040:5002:8::6f
CNAME   www     [your-site].netlify.app
```

---

## ✅ **VERIFICATION CHECKLIST**

After deployment:
```
[ ] Site loads at https://[name].netlify.app
[ ] All pages work
[ ] Logo displays
[ ] Mobile responsive
[ ] SSL enabled (green padlock)
[ ] No console errors (F12)
[ ] Custom domain configured
[ ] Force HTTPS enabled
```

---

## 🐛 **QUICK FIXES**

**Build fails:**
```
→ Check build log in Netlify
→ Clear cache and redeploy
→ Verify Node version 18
```

**Blank page:**
```
→ Open console (F12) for errors
→ Check publish directory is 'dist'
→ Verify _redirects file exists
```

**Images broken:**
```
→ Verify /public/logo-full.svg exists
→ Check paths start with /
→ Clear browser cache (Ctrl+Shift+R)
```

**Domain not working:**
```
→ Verify DNS records
→ Wait 24-48 hours for propagation
→ Check https://dnschecker.org
```

---

## 📊 **WHAT'S INCLUDED**

✅ Global CDN  
✅ Free SSL  
✅ Auto deployments  
✅ Deploy previews  
✅ Instant rollbacks  
✅ 100GB bandwidth/month  
✅ DDoS protection  
✅ Security headers  
✅ Cache optimization  

---

## 🔗 **USEFUL LINKS**

- **Dashboard:** https://app.netlify.com/
- **Docs:** https://docs.netlify.com/
- **Forum:** https://answers.netlify.com/
- **Status:** https://www.netlifystatus.com/

---

## 🚀 **DEPLOY COMMAND**

If using Netlify CLI:
```bash
netlify deploy --prod
```

---

## ⏱️ **TIMELINE**

| Task | Time |
|------|------|
| Push to GitHub | 2 min |
| Initial deploy | 3 min |
| SSL setup | 5 min |
| DNS propagation | 24-48 hrs |

---

**Total active time: ~10 minutes**  
**Full DNS: 24-48 hours**

---

*Quick reference for Super GRC Netlify deployment*
