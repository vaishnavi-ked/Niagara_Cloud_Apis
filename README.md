# Niagara Cloud Dashboard

This is a Node.js/Express dashboard for visualizing smart building data from the Niagara Cloud API.

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [npm](https://www.npmjs.com/)
- API credentials for Niagara Cloud (see `.env` setup below)

## Setup

1. **Clone the repository**

   ```sh
   git clone <your-repo-url>
   cd <project-directory>
   ```

2. **Install dependencies**

   ```sh
   npm install
   ```

3. **Configure environment variables**

   - Copy `dashboard.env` to `.env` (or edit `dashboard.env` directly).
   - Fill in your Niagara Cloud API credentials:
     ```
     CLIENT_ID=your_client_id
     CLIENT_SECRET=your_client_secret
     CUSTOMER_ID=your_customer_id
     SYSTEM_GUID=your_system_guid
     PING_TOKEN_URL=https://your-token-url
     ```

4. **Run the server**

   ```sh
   npm start
   ```
   Or for development with auto-reload:
   ```sh
   npm run dev
   ```

5. **Open the dashboard**

   - Visit [http://localhost:3000/dashboard](http://localhost:3000/dashboard) in your browser.

## Project Structure

- `server.js` - Main Express server and API logic
- `views/` - EJS templates for dashboard and other pages
- `public/` - Static assets (CSS, JS, images)
- `dashboard.env` - Environment variables (API credentials)

## Notes

- The dashboard auto-refreshes data every 10 seconds.
- Make sure your API credentials are valid and have access to the required endpoints.

---

For any issues, please contact the project maintainer.
