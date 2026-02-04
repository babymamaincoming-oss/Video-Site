# Video Site

A simple, elegant video site with an embedded YouTube video.

## Custom Domain Setup

This site is configured to use a custom domain instead of the default GitHub Pages URL.

### How to Configure Your Custom Domain

1. **Update the CNAME file**: Replace `www.example.com` in the `CNAME` file with your actual domain name (e.g., `videos.yourdomain.com` or `www.yourdomain.com`)

2. **Configure DNS Settings**: In your domain registrar's DNS settings, add one of the following:
   
   **For a subdomain (recommended):**
   - Add a CNAME record pointing to `babymamaincoming-oss.github.io`
   - Example: `www` or `videos` → `babymamaincoming-oss.github.io`
   
   **For an apex domain (root domain):**
   - Add A records pointing to GitHub's IP addresses:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Add AAAA records (optional, for IPv6):
     - 2606:50c0:8000::153
     - 2606:50c0:8001::153
     - 2606:50c0:8002::153
     - 2606:50c0:8003::153

3. **Enable HTTPS**: After DNS propagates (may take up to 48 hours), enable HTTPS in your GitHub repository settings under Pages → Enforce HTTPS

### Testing Your Domain

After DNS propagation, your site will be accessible at your custom domain instead of the GitHub Pages URL.

You can check DNS propagation status at: https://www.whatsmydns.net/

## Development

This is a simple static HTML site. To make changes, edit `index.html` and commit your changes.
