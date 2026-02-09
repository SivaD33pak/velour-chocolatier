# Velour Chocolatier Website Deployment Guide

This guide outlines the steps to deploy the Velour Chocolatier website to **Vercel**.

## Prerequisites

- A [Vercel](https://vercel.com/) account.
- The project pushed to a Git repository (GitHub, GitLab, or Bitbucket).

## Deployment Steps

1.  **Log in to Vercel**: Go to your Vercel dashboard.
2.  **Add New Project**: Click on "Add New..." and select "Project".
3.  **Import Git Repository**: Select the `Velour` repository you just pushed.
4.  **Configure Project**:
    *   **Framework Preset**: Select "Other" (since this is a simple HTML/Static project).
    *   **Root Directory**: Click "Edit" next to Root Directory and select `src`.
        *   *Note*: This is crucial because your HTML files reside in the `src` folder.
5.  **Deploy**: Click "Deploy".

## Post-Deployment

- Vercel will build and assign a domain (e.g., `velour-chocolatier.vercel.app`).
- Verify that `cleanUrls` are working (e.g., verify you can visit pages without `.html` extension if supported by your links).

## Local Development

To run the project locally:

```bash
cd src
npx serve
```
