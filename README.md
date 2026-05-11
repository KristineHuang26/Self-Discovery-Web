# Self Profile Page Generator

A web app that helps users create personalized self-profile pages based on identity, memory, personality, and visual aesthetic preferences.

The project is designed to turn a simple self-reflection routine into a shareable digital profile page. Users can create their own profile, choose an aesthetic theme, and generate links for either social sharing or professional showcase use.

## Features

- Interactive self-profile creation flow
- Personalized profile page generation
- Multiple aesthetic theme options
- Saved profiles using a database-backed system
- Public social sharing link for inviting others to create their own profile
- Professional read-only showcase link for portfolio, LinkedIn, CV, or email signature use
- Mobile-friendly public profile pages

## Sharing System

Each saved profile generates two types of public links:

### Social Share Link

Designed for visibility and growth. This version allows others to view the profile and includes a call-to-action encouraging them to create their own.

Example:

    ```text
    /share/:id# Self Profile Page Generator

### Professional Showcase Link

The professional showcase link is designed for clean, read-only presentation. This version focuses on the finished profile only and avoids exposing the creation/editing interface.

Use Case: LinkedIn, CV, personal portfolio, email signature, job applications, or professional self-presentation.

## How It Works

User creates a profile
↓
User saves or publishes the profile
↓
The profile is stored in the database
↓
The backend generates or returns a unique profile ID
↓
The app creates two public links using that ID
↓
Other people can open the links from any device

## Recommended Routes

/                 Home or landing page
/create           Profile creation flow
/editor/:id       Profile editing page
/share/:id        Public social sharing page
/p/:id            Professional read-only showcase page
/api/profiles/:id Backend API endpoint for loading saved profiles

## Tech Stack

React
Node.js / Express
PostgreSQL
Tailwind CSS

## Local Development

### Install dependencies:

npm install
npm run dev

Depending on the deployment setup, the project may require environment variables for the database connection and server configuration.

