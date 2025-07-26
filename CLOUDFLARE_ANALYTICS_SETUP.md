# Cloudflare & Analytics Setup Guide

## ☁️ **Cloudflare Setup**

### **Step 1: Add Domain to Cloudflare**

1. **Go to [cloudflare.com](https://cloudflare.com)**
2. **Sign up/Login** to your account
3. **Click "Add a Site"**
4. **Enter**: `tartarusgroup.com`
5. **Select "Free" plan**
6. **Click "Continue"**

### **Step 2: Update Nameservers**

Cloudflare will provide 2 nameservers like:
```
nina.ns.cloudflare.com
rick.ns.cloudflare.com
```

**Update these at your domain registrar:**
1. **Login** to your domain registrar (where you bought tartarusgroup.com)
2. **Find DNS/Nameserver settings**
3. **Replace existing nameservers** with Cloudflare's
4. **Save changes**

### **Step 3: Configure DNS Records**

Once nameservers are updated (can take 24-48 hours), in Cloudflare DNS:

**CNAME Record:**
- **Name**: `tartarusgroup.com`
- **Target**: `bgarber42.github.io`
- **Proxy status**: ✅ **Proxied** (orange cloud)

**A Records** (for apex domain):
- **Name**: `@`
- **Target**: `185.199.108.153`
- **Proxy status**: ✅ **Proxied**

- **Name**: `@`
- **Target**: `185.199.109.153`
- **Proxy status**: ✅ **Proxied**

- **Name**: `@`
- **Target**: `185.199.110.153`
- **Proxy status**: ✅ **Proxied**

- **Name**: `@`
- **Target**: `185.199.111.153`
- **Proxy status**: ✅ **Proxied**

### **Step 4: SSL/TLS Settings**

In Cloudflare SSL/TLS settings:
1. **Encryption mode**: "Full"
2. **Always Use HTTPS**: ✅ **On**
3. **Minimum TLS Version**: 1.2

### **Step 5: Performance Settings**

**Speed > Optimization:**
- ✅ **Auto Minify**: JavaScript, CSS, HTML
- ✅ **Brotli**: On
- ✅ **Early Hints**: On

**Caching > Configuration:**
- ✅ **Browser Cache TTL**: 4 hours
- ✅ **Always Online**: On

---

## 📊 **Google Analytics Setup**

### **Step 1: Create Google Analytics Account**

1. **Go to [analytics.google.com](https://analytics.google.com)**
2. **Click "Start measuring"**
3. **Create account**: "Tartarus Group"
4. **Create property**: "Tartarus Group Website"
5. **Enter website URL**: `https://tartarusgroup.com`
6. **Complete setup**

### **Step 2: Get Measurement ID**

1. **Go to Admin** (gear icon)
2. **Property Settings**
3. **Copy Measurement ID** (starts with "G-")

### **Step 3: Update Website Code**

**Replace `GA_MEASUREMENT_ID` in `index.html`:**

Find this line:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
```

Replace `GA_MEASUREMENT_ID` with your actual ID (e.g., `G-ABC123DEF4`):
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-ABC123DEF4"></script>
```

Also update this line:
```html
gtag('config', 'G-ABC123DEF4');
```

### **Step 4: Deploy Updated Code**

```bash
git add .
git commit -m "Add Google Analytics tracking"
git push
```

---

## 🎯 **Benefits You'll Get**

### **Cloudflare Benefits:**
- ✅ **Faster loading** worldwide (CDN)
- ✅ **Free SSL certificate** (instant)
- ✅ **DDoS protection**
- ✅ **Caching** for better performance
- ✅ **Analytics** included

### **Google Analytics Benefits:**
- ✅ **Visitor insights** (traffic, sources)
- ✅ **Page performance** data
- ✅ **User behavior** analysis
- ✅ **Conversion tracking**
- ✅ **Real-time data**

---

## 🚀 **Next Steps After Setup**

1. **Wait for DNS propagation** (24-48 hours)
2. **Test HTTPS**: `https://tartarusgroup.com`
3. **Verify analytics** are tracking
4. **Monitor performance** improvements
5. **Set up conversion goals** in Analytics

Your website will be faster, more secure, and you'll have valuable insights into your visitors! 🎉 