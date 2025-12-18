# Project: IELTS Coaching Center, Akure
# Folder structure:
ielts-coaching-center-akure/
├─ package.json
├─ vite.config.js
├─ tailwind.config.js
├─ postcss.config.js
├─ public/
│   ├─ logo.png
│   └─ placeholder.jpg
├─ src/
│   ├─ main.jsx
│   ├─ App.jsx
│   ├─ index.css
│   ├─ components/
│   │   ├─ Navbar.jsx
│   │   ├─ Footer.jsx
│   │   ├─ Hero.jsx
│   │   ├─ Stats.jsx
│   │   ├─ CoursesCard.jsx
│   │   ├─ TestimonialCard.jsx
│   │   ├─ ScrollToTop.jsx
│   │   └─ DarkModeToggle.jsx
│   ├─ pages/
│   │   ├─ Home.jsx
│   │   ├─ About.jsx
│   │   ├─ Courses.jsx
│   │   ├─ Services.jsx
│   │   ├─ SuccessStories.jsx
│   │   ├─ Blog.jsx
│   │   └─ Contact.jsx
│   └─ assets/
│       └─ images/

# package.json
{
  "name": "ielts-coaching-center-akure",
  "version": "1.0.0",
  "private": true,
  "dependencies": {
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "react-router-dom": "^6.16.0",
    "framer-motion": "^10.12.16",
    "lucide-react": "^0.268.0"
  },
  "devDependencies": {
    "vite": "^5.0.0",
    "tailwindcss": "^4.3.2",
    "autoprefixer": "^10.4.0",
    "postcss": "^8.4.0"
  },
  "scripts": {
    "dev": "vite",
    "build": "vite build",
    "preview": "vite preview"
  }
}

# vite.config.js
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
export default defineConfig({ plugins: [react()] })

# tailwind.config.js
export default { content: ['./index.html', './src/**/*.{js,jsx}'], theme: { extend: {} }, plugins: [] }

# postcss.config.js
export default { plugins: { tailwindcss: {}, autoprefixer: {} } }

# src/main.jsx
import React from 'react'
import ReactDOM from 'react-dom/client'
import App from './App'
import './index.css'
ReactDOM.createRoot(document.getElementById('root')).render(<React.StrictMode><App /></React.StrictMode>)

# src/index.css
@tailwind base;
@tailwind components;
@tailwind utilities;
html { scroll-behavior: smooth; }
body { background-color: #f9fafb; color: #1f2937; }

# src/App.jsx
import { BrowserRouter as Router, Routes, Route } from 'react-router-dom';
import Navbar from './components/Navbar';
import Footer from './components/Footer';
import ScrollToTop from './components/ScrollToTop';
import DarkModeToggle from './components/DarkModeToggle';
import Home from './pages/Home';
import About from './pages/About';
import Courses from './pages/Courses';
import Services from './pages/Services';
import SuccessStories from './pages/SuccessStories';
import Blog from './pages/Blog';
import Contact from './pages/Contact';
function App() { return (<Router><DarkModeToggle /><Navbar /><ScrollToTop /><Routes><Route path="/" element={<Home />} /><Route path="/about" element={<About />} /><Route path="/courses" element={<Courses />} /><Route path="/services" element={<Services />} /><Route path="/success-stories" element={<SuccessStories />} /><Route path="/blog" element={<Blog />} /><Route path="/contact" element={<Contact />} /></Routes><Footer /></Router>); }
export default App;

# src/components/Navbar.jsx
import { useState } from 'react';
import { Link } from 'react-router-dom';
const Navbar = () => { const [open,setOpen]=useState(false); return (<nav className="bg-white dark:bg-gray-900 shadow fixed w-full z-50"><div className="container mx-auto px-4 py-4 flex justify-between items-center"><Link to="/" className="font-bold text-xl text-blue-600">IELTS Coaching Akure</Link><div className="hidden md:flex gap-6"><Link to="/">Home</Link><Link to="/about">About</Link><Link to="/courses">Courses</Link><Link to="/services">Services</Link><Link to="/success-stories">Success Stories</Link><Link to="/blog">Blog</Link><Link to="/contact" className="bg-green-500 px-4 py-2 rounded-lg text-white hover:bg-green-600">Contact</Link></div><div className="md:hidden flex items-center gap-2"><button onClick={()=>setOpen(!open)}>{open?'✖':'☰'}</button></div></div>{open&&(<div className="md:hidden bg-white dark:bg-gray-900 flex flex-col px-4 py-2 gap-2"><Link to="/" onClick={()=>setOpen(false)}>Home</Link><Link to="/about" onClick={()=>setOpen(false)}>About</Link><Link to="/courses" onClick={()=>setOpen(false)}>Courses</Link><Link to="/services" onClick={()=>setOpen(false)}>Services</Link><Link to="/success-stories" onClick={()=>setOpen(false)}>Success Stories</Link><Link to="/blog" onClick={()=>setOpen(false)}>Blog</Link><Link to="/contact" className="bg-green-500 px-4 py-2 rounded-lg text-white" onClick={()=>setOpen(false)}>Contact</Link></div>)}</nav>); }
export default Navbar;

# src/components/Footer.jsx
const Footer=()=>{return(<footer className="bg-blue-600 text-white py-8 mt-12"><div className="container mx-auto text-center"><p className="mb-2">IELTS Coaching Center, Akure</p><p className="mb-4">Phone: +234 800 123 4567 | Email: info@ieltsakure.com</p><p>&copy; {new Date().getFullYear()} IELTS Coaching Akure. All rights reserved.</p></div></footer>);}
export default Footer;

# src/components/Hero.jsx
import { motion } from 'framer-motion';
const Hero=()=>{return(<section className="bg-blue-600 text-white py-32 px-4 text-center"><motion.h1 className="text-4xl md:text-6xl font-bold mb-4" initial={{opacity:0,y:-50}} animate={{opacity:1,y:0}} transition={{duration:1}}>Ace Your IELTS Exam with Confidence</motion.h1><p className="text-lg md:text-2xl mb-8">Expert IELTS coaching in Akure with proven success rates</p><div className="flex justify-center gap-4"><a href="/contact" className="bg-green-500 px-6 py-3 rounded-lg font-semibold hover:bg-green-600">Enroll Now</a><a href="/contact" className="bg-white text-blue-600 px-6 py-3 rounded-lg font-semibold hover:bg-gray-100">Free Consultation</a></div></section>);}
export default Hero;

# src/components/Stats.jsx
const Stats=()=>{return(<section className="py-16 bg-gray-100 text-center"><div className="container mx-auto grid md:grid-cols-3 gap-8"><div><h2 className="text-4xl font-bold text-blue-600">95%</h2><p>Success Rate</p></div><div><h2 className="text-4xl font-bold text-blue-600">500+</h2><p>Students Trained</p></div><div><h2 className="text-4xl font-bold text-blue-600">Certified</h2><p>IELTS Tutors</p></div></div></section>);}
export default Stats;

# src/components/CoursesCard.jsx
const CoursesCard=({title,description,duration,price})=>{return(<div className="bg-white shadow-lg rounded-lg p-6 hover:shadow-xl transition"><h3 className="text-xl font-bold mb-2">{title}</h3><p className="mb-2">{description}</p><p className="mb-2">Duration: {duration}</p><p className="mb-4">Price: {price}</p><a href="/contact" className="bg-green-500 px-4 py-2 rounded-lg text-white hover:bg-green-600">Enroll Now</a></div>);}
export default CoursesCard;

# src/components/TestimonialCard.jsx
const TestimonialCard=({name,band,review})=>{return(<div className="bg-white shadow-md rounded-lg p-6"><p className="mb-2">"{review}"</p><h4 className="font-bold">{name}</h4><span>Band {band}</span></div>);}
export default TestimonialCard;

# src/components/ScrollToTop.jsx
import { useEffect } from 'react';
import { useLocation } from 'react-router-dom';
const ScrollToTop=()=>{const {pathname}=useLocation();useEffect(()=>{window.scrollTo(0,0);},[pathname]);return null;}
export default ScrollToTop;

# src/components/DarkModeToggle.jsx
import { useState,useEffect } from 'react';
import { Sun,Moon } from 'lucide-react';
const DarkModeToggle=()=>{const [dark,setDark]=useState(false);useEffect(()=>{dark?document.documentElement.classList.add('dark'):document.documentElement.classList.remove('dark');},[dark]);return(<button onClick={()=>setDark(!dark)} className="fixed top-4 right-4 p-2 bg-gray-200 dark:bg-gray-700 rounded-full z-50">{dark?<Sun />:<Moon />}</button>);}
export default DarkModeToggle;

# src/pages/Home.jsx
import Hero from '../components/Hero';
import Stats from '../components/Stats';
const Home=()=>{return(<><Hero /><Stats /></>);}
export default Home;

# src/pages/About.jsx
const About=()=>{return(<section className="py-16 px-4 max-w-5xl mx-auto"><h2 className="text-3xl font-bold mb-4 text-center">About IELTS Coaching Center, Akure</h2><p className="mb-4 text-center">We provide expert IELTS coaching for Academic and General Training students. Our certified tutors have helped hundreds of students achieve their dream band scores.</p></section>);}
export default About;

# src/pages/Courses.jsx
import CoursesCard from '../components/CoursesCard';
const Courses=()=>{return(<section className="py-16 px-4 max-w-5xl mx-auto"><h2 className="text-3xl font-bold mb-8 text-center">Our Courses</h2><div className="grid md:grid-cols-2 gap-8"><CoursesCard title="IELTS Academic" description="Comprehensive Academic IELTS prep" duration="8 weeks" price="₦150,000"/><CoursesCard title="IELTS General Training" description="Focused General IELTS prep" duration="6 weeks" price="₦120,000"/><CoursesCard title="One-on-One Coaching" description="Personalized coaching with expert tutor" duration="Flexible" price="₦200,000"/><CoursesCard title="Weekend Classes" description="Intensive weekend sessions" duration="4 weeks" price="₦80,000"/><CoursesCard title="Online Classes" description="Remote coaching via Zoom" duration="8 weeks" price="₦100,000"/></div></section>);}
export default Courses;

# src/pages/Services.jsx
const Services=()=>{return(<section className="py-16 px-4 max-w-5xl mx-auto"><h2 className="text-3xl font-bold mb-8 text-center">IELTS Services</h2><ul className="list-disc list-inside space-y-2 text-lg"><li>Speaking Test Preparation</li><li>Writing Task 1 & 2 Coaching</li><li>Listening Practice</li><li>Reading Strategies</li><li>Mock Exams</li><li>Band Score Improvement Program</li></ul></section>);}
export default Services;

# src/pages/SuccessStories.jsx
import TestimonialCard from '../components/TestimonialCard';
const SuccessStories=()=>{return(<section className="py-16 px-4 max-w-5xl mx-auto"><h2 className="text-3xl font-bold mb-8 text-center">Success Stories</h2><div className="grid md:grid-cols-2 gap-8"><TestimonialCard name="Amaka" band="8.5" review="I achieved my target band thanks to the expert coaching!"/><TestimonialCard name="Chidi" band="7.5" review="Highly recommended for anyone preparing for IELTS."/></div></section>);}
export default SuccessStories;

# src/pages/Blog.jsx
const Blog=()=>{return(<section className="py-16 px-4 max-w-5xl mx-auto"><h2 className="text-3xl font-bold mb-8 text-center">Blog & Resources</h2><ul className="list-disc list-inside space-y-2"><li>Top IELTS Writing Tips</li><li>Listening Practice Strategies</li><li>Reading Techniques for High Scores</li><li>Exam Updates & Resources</li></ul></section>);}
export default Blog;

# src/pages/Contact.jsx
const Contact=()=>{return(<section className="py-16 bg-gray-50"><div className="container mx-auto max-w-xl px-4"><h2 className="text-3xl font-bold mb-6 text-center">Contact Us</h2><form className="flex flex-col gap-4"><input type="text" placeholder="Name" className="p-3 border rounded"/><input type="email" placeholder="Email" className="p-3 border rounded"/><input type="tel" placeholder="Phone" className="p-3 border rounded"/><textarea placeholder="Message" className="p-3 border rounded"></textarea><button type="submit" className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-700">Send Message</button></form><div className="mt-6 text-center"><a href="https://wa.me/2348001234567" className="bg-green-500 text-white px-6 py-3 rounded hover:bg-green-600">Chat on WhatsApp</a></div></div></section>);}
export default Contact;
