# Deploy to Render

## Steps to Deploy

1. **Push your code to GitHub:**
   ```bash
   git add .
   git commit -m "Initial commit with Swagger API"
   git push -u origin main
   ```

2. **Go to Render Dashboard:**
   - Visit https://render.com
   - Sign in or create an account

3. **Create a New Web Service:**
   - Click "New +" → "Web Service"
   - Connect your GitHub repository: `kruz-rana/Swagger_api`
   - Configure the service:
     - **Name:** swagger-api (or your preferred name)
     - **Environment:** Node
     - **Build Command:** `npm install`
     - **Start Command:** `npm start`
     - **Plan:** Free

4. **Deploy:**
   - Click "Create Web Service"
   - Render will automatically deploy your app
   - Your API will be live at: `https://your-app-name.onrender.com`

5. **Access Swagger Docs:**
   - Once deployed, visit: `https://your-app-name.onrender.com/api-docs`

## Notes

- Free tier services may spin down after inactivity (takes ~30 seconds to wake up)
- The `render.yaml` file is included for automatic configuration
- Environment variable `RENDER_EXTERNAL_URL` is automatically set by Render
