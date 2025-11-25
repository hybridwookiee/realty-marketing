# Collaboration Guide

## Repository Information
- **GitHub URL:** https://github.com/hybridwookiee/realty-marketing
- **Default Branch:** `main`

## Adding a Collaborator

### Option 1: Using GitHub CLI (Recommended)
```bash
gh repo invite <username> --repo hybridwookiee/realty-marketing
```

### Option 2: Using GitHub Web Interface
1. Go to https://github.com/hybridwookiee/realty-marketing
2. Click on **Settings** (top right)
3. Click on **Collaborators** in the left sidebar
4. Click **Add people**
5. Enter the collaborator's GitHub username or email
6. Select their permission level:
   - **Read**: Can view and clone
   - **Write**: Can push changes
   - **Admin**: Full access including settings
7. Click **Add [username] to this repository**

## For Collaborators: Getting Started

### Clone the Repository
```bash
git clone https://github.com/hybridwookiee/realty-marketing.git
cd realty-marketing
```

### Making Changes
1. Create a new branch for your work:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes and commit:
   ```bash
   git add .
   git commit -m "Description of your changes"
   ```

3. Push your branch:
   ```bash
   git push origin feature/your-feature-name
   ```

4. Create a Pull Request on GitHub to merge into `main`

### Syncing with Latest Changes
```bash
git checkout main
git pull origin main
```

## Best Practices
- Always work on a feature branch, not directly on `main`
- Write clear commit messages
- Pull latest changes before starting new work
- Create Pull Requests for review before merging

