# DSA Sensei

A secure deployment of the DSA Sensei application.

## Security Note
This project uses GitHub Actions to securely inject API keys during the deployment process. The `config.js` file is generated dynamically on the GitHub runner and is never stored in the repository.

## Setup Instructions

1.  **Create a new GitHub Repository.**
2.  **Add Secrets:** Go to `Settings` > `Secrets and variables` > `Actions` and add the following repository secrets:
    *   `GROQ_API_KEY`: Your Groq API key.
    *   `SUPABASE_URL`: Your Supabase Project URL.
    *   `SUPABASE_ANON_KEY`: Your Supabase Anon/Public Key.
    *   `TEACHER_PASS`: Your desired teacher password (default is `dsasensei2025`).
3.  **Push the code:** Push these files to the `main` branch.
4.  **Enable GitHub Pages:** Go to `Settings` > `Pages` and ensure "Build and deployment" is set to "GitHub Actions".
