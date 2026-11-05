# S SQUARE STUDIO | Portfolio

A modern, responsive, and dynamic portfolio website for **Sumanan**, a professional Video Editor & Colorist. Built with Next.js, this application showcases cinematic video editing, color grading, and sound design projects, complete with an interactive admin panel for content management.

## 🚀 Features

- **Dynamic Portfolio Grid:** View recent works categorized by project type (Travel Films, Product Promos, etc.).
- **Video Showreels:** Interactive video modals powered by `react-player` for seamless viewing without leaving the page.
- **Client Reviews:** A built-in review system where clients can submit their feedback and ratings.
- **Admin Dashboard:** A secured backend panel to upload new projects and approve/manage client reviews.
- **Modern UI/UX:** Dark-themed, cinematic design using Tailwind CSS, backdrop filters, and smooth animations with Framer Motion.
- **Direct Contact:** Quick WhatsApp and email integrations for easy client communication.

## 🛠️ Tech Stack

- **Framework:** [Next.js](https://nextjs.org/) (App Router)
- **Language:** TypeScript
- **Styling:** CSS Modules & Tailwind CSS
- **Backend/Database:** [Supabase](https://supabase.com/) (PostgreSQL & Auth)
- **Animations:** [Framer Motion](https://www.framer.com/motion/)
- **Icons:** `lucide-react`, `react-icons`
- **Video Player:** `react-player`

## 📦 Getting Started

### Prerequisites
Make sure you have [Node.js](https://nodejs.org/) installed on your machine.

### Installation

1. **Clone the repository (or navigate to the project directory):**
   ```bash
   cd sspp
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Set up Environment Variables:**
   Create a `.env.local` file in the root directory and add your Supabase credentials:
   ```env
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   ```
   *(Note: You will need a Supabase project set up with `projects` and `reviews` tables as defined in the `supabase-setup.sql` file.)*

4. **Run the development server:**
   ```bash
   npm run dev
   ```

5. **Open the App:**
   Open [http://localhost:3000](http://localhost:3000) with your browser to see the live portfolio.

## 🗄️ Database Schema

This project relies on Supabase. A setup file (`supabase-setup.sql`) is included to quickly initialize the necessary tables:
- `projects`: Stores video portfolio data (title, category, video URL, thumbnail).
- `reviews`: Stores client testimonials (name, text, rating, approval status).

## 🔒 Admin Access

To access the admin panel for uploading projects and managing reviews, navigate to `/login` to authenticate, which will redirect you to the `/admin` dashboard.

## 📄 License

This project is proprietary and created for **S Square Studio**. All video contents and branding are copyright of their respective owners.
