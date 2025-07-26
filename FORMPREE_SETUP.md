# Formspree Setup Guide

## 📧 **Step-by-Step Formspree Integration**

### **Step 1: Create Formspree Account**

1. **Go to [formspree.io](https://formspree.io)**
2. **Sign up** for a free account
3. **Verify your email** address

### **Step 2: Create a New Form**

1. **Click "New Form"** in your dashboard
2. **Name it**: "Tartarus Group Contact"
3. **Copy the form endpoint** - it will look like:
   ```
   https://formspree.io/f/xaybzwab
   ```

### **Step 3: Update the Website Code**

**Replace `YOUR_FORM_ID` in `index.html`:**

Find this line:
```html
<form class="contact-form" id="contactForm" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

Replace `YOUR_FORM_ID` with your actual form ID (e.g., `xaybzwab`):
```html
<form class="contact-form" id="contactForm" action="https://formspree.io/f/xaybzwab" method="POST">
```

### **Step 4: Configure Formspree Settings**

1. **Go to your form settings** in Formspree dashboard
2. **Set up email notifications**:
   - Add your email: `contact@tartarusgroup.com`
   - Choose notification frequency
3. **Configure spam protection** (optional)
4. **Set up redirect URLs** (optional):
   - Success: `https://tartarusgroup.com/?status=success`
   - Error: `https://tartarusgroup.com/?status=error`

### **Step 5: Test the Form**

1. **Deploy your website** to GitHub Pages
2. **Test the contact form** by submitting a message
3. **Check your email** for the notification
4. **Verify the form data** in Formspree dashboard

## 🔧 **Features Included**

### **✅ Form Validation**
- Required field validation
- Email format validation
- Client-side error messages

### **✅ User Experience**
- Loading state during submission
- Success/error notifications
- Form reset after successful submission

### **✅ Spam Protection**
- Formspree's built-in spam filtering
- Honeypot protection
- Rate limiting

### **✅ Email Notifications**
- Instant email notifications
- Form data in organized format
- Customizable email templates

## 📊 **Formspree Plans**

### **Free Plan** (Recommended to start)
- ✅ 50 submissions per month
- ✅ Email notifications
- ✅ Spam protection
- ✅ Basic analytics

### **Paid Plans** (If you need more)
- **Starter**: $8/month - 1,000 submissions
- **Growth**: $25/month - 5,000 submissions
- **Business**: $50/month - 25,000 submissions

## 🚀 **Next Steps**

1. **Create your Formspree account**
2. **Get your form endpoint**
3. **Update the HTML with your form ID**
4. **Deploy to GitHub Pages**
5. **Test the form**

The form is now ready to capture leads and inquiries from your website! 🎉 