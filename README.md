# Spotify OAuth Callback Page

This project provides a simple **callback page** for handling Spotify OAuth redirects.  
When Spotify redirects the user after login and authorization, this page displays the full URL including the authorization code or access token.

## 📄 What is this page?

- A minimal HTML file (`callback.html`) that shows the full redirect URL.  
- Useful for testing and debugging Spotify OAuth flows.  
- Helps you manually copy the authorization code or token from the URL.

## 🚀 How it works

1. Configure your Spotify Developer App with a **Redirect URI** pointing to this page, e.g.:
2. After login, Spotify redirects the browser to this page with query parameters:
3. The page displays the full URL so you can see the returned code/token.

⚠️ Notes
This page is for testing and development.
In production, you should handle the authorization code server‑side and exchange it for an access token using Spotify’s Web API.
Tokens expire after ~1 hour; for long‑term use, implement a refresh token flow.
