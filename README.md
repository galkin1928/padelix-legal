# Legal Documents for PadelAudioCounter

This folder contains the legal documents for the PadelAudioCounter mobile application.

## 📄 Files

- **index.html** - Landing page with links to legal documents
- **terms.html** - Terms of Use
- **privacy.html** - Privacy Policy

## 🌐 Live Preview

To preview these files locally:

```bash
cd /Users/alex/dev/PadelAudioCounter/docs
python3 -m http.server 8000
```

Then open: http://localhost:8000

## ⚠️ Before Publishing

Replace the following placeholders in all HTML files:

1. **Email**: `[email protected]` → Your actual support email
2. **Developer Name**: `[Your Name/Company Name]` → Your actual name/company

Quick replace command:
```bash
# Replace email
sed -i '' 's/support@padelaudiocounter\.com/youremail@example.com/g' *.html

# Replace developer name
sed -i '' 's/\[Your Name\/Company Name\]/Your Actual Name/g' *.html
```

## 🚀 Deployment

See `../HOSTING_OPTIONS.md` for detailed deployment instructions.

**Recommended:** GitHub Pages for free, professional hosting.

## 📱 Usage in App

After deployment, use these URLs in your `PaywallView.swift`:

```swift
Link("Terms of Use", destination: URL(string: "https://your-domain.com/terms.html")!)
Link("Privacy Policy", destination: URL(string: "https://your-domain.com/privacy.html")!)
```

## ✅ Checklist

- [ ] Replace placeholder email and developer name
- [ ] Test all pages locally
- [ ] Deploy to hosting service
- [ ] Verify links work from mobile device
- [ ] Update URLs in app code
- [ ] Submit to App Store
