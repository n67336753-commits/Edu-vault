<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exam Archive — Premium JEE & NEET Academic Resources</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">

    <style>
        /* ==========================================================================
           Exam Archive — Structural Luxury Design Language Sheet
           ========================================================================== */

        :root {
            --bg-warm-grey: #f5f4f0;
            --color-taupe: #d7d3c9;
            --color-charcoal: #1c1c1a;
            --color-muted-brown: #5c5852;
            --color-off-white: #fafafa;
            --color-glass-border: rgba(28, 28, 26, 0.08);
            --font-serif: 'Cormorant Garamond', Georgia, serif;
            --font-sans: 'Plus Jakarta Sans', system-ui, sans-serif;
            --grid-line-color: rgba(28, 28, 26, 0.05);
            --transition-smooth: all 0.6s cubic-bezier(0.16, 1, 0.3, 1);
        }

        /* Global System Resets & Architecture */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
            background-color: var(--bg-warm-grey);
            color: var(--color-charcoal);
            font-family: var(--font-sans);
            font-size: 16px;
            -webkit-font-smoothing: antialiased;
        }

        body {
            overflow-x: hidden;
            position: relative;
        }

        /* Static Structural Aesthetic Background Grid lines */
        .grid-line-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 99;
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            padding: 0 10vw;
        }

        .grid-line-overlay .line {
            border-right: 1px solid var(--grid-line-color);
            height: 100%;
        }

        .grid-line-overlay .line:first-child {
            border-left: 1px solid var(--grid-line-color);
        }

        /* Reusable Layout Systems */
        .section-padding {
            padding: 8rem 10vw;
        }

        .border-top-grid {
            border-top: 1px solid rgba(28, 28, 26, 0.1);
        }

        /* Typographic Hierarchy Styling */
        .serif-italic {
            font-family: var(--font-serif);
            font-style: italic;
            font-weight: 400;
        }

        .section-index {
            display: block;
            font-family: var(--font-sans);
            font-size: 0.85rem;
            font-weight: 500;
            letter-spacing: 0.15em;
            color: var(--color-muted-brown);
            margin-bottom: 1rem;
        }

        .section-title-editorial {
            font-family: var(--font-serif);
            font-size: 3.5rem;
            font-weight: 300;
            line-height: 1.1;
            letter-spacing: -0.02em;
            margin-bottom: 2rem;
        }

        /* Refined Studio Navigation Bar */
        .nav-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 10vw;
            z-index: 1000;
            background: rgba(245, 244, 240, 0.8);
            backdrop-filter: blur(15px);
            border-bottom: 1px solid var(--color-glass-border);
        }

        .nav-brand {
            font-family: var(--font-sans);
            font-weight: 600;
            font-size: 1.1rem;
            letter-spacing: 0.2em;
        }

        .nav-links {
            display: flex;
            gap: 2.5rem;
        }

        .nav-link {
            text-decoration: none;
            color: var(--color-charcoal);
            font-size: 0.85rem;
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            position: relative;
            padding: 0.3rem 0;
            transition: var(--transition-smooth);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 1px;
            background-color: var(--color-charcoal);
            transition: var(--transition-smooth);
        }

        .nav-link:hover::after, .nav-link.active::after {
            width: 100%;
        }

        .mobile-nav-toggle {
            display: none;
            background: none;
            border: none;
            cursor: pointer;
            flex-direction: column;
            gap: 6px;
        }

        .mobile-nav-toggle span {
            width: 24px;
            height: 1px;
            background-color: var(--color-charcoal);
        }

        /* Hero Screen Presentation Layout */
        .hero-section {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 0 10vw;
            position: relative;
            overflow: hidden;
            gap: 4rem;
        }

        .hero-content {
            flex: 1.2;
            z-index: 10;
            margin-top: 4rem;
        }

        .eyebrow-text {
            font-family: var(--font-sans);
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 0.25em;
            color: var(--color-muted-brown);
            display: block;
            margin-bottom: 1.5rem;
        }

        .hero-title {
            font-family: var(--font-serif);
            font-size: 5.5rem;
            font-weight: 300;
            line-height: 1.05;
            letter-spacing: -0.03em;
            margin-bottom: 2rem;
        }

        .hero-tagline {
            font-size: 1.15rem;
            line-height: 1.7;
            color: var(--color-muted-brown);
            max-width: 540px;
            margin-bottom: 3rem;
            font-weight: 300;
        }

        .hero-actions {
            display: flex;
            gap: 1.5rem;
        }

        /* Structural Layout Buttons */
        .btn {
            display: inline-block;
            padding: 1.1rem 2.2rem;
            font-family: var(--font-sans);
            font-size: 0.85rem;
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            text-decoration: none;
            border: 1px solid var(--color-charcoal);
            cursor: pointer;
            transition: var(--transition-smooth);
        }

        .btn-primary {
            background-color: var(--color-charcoal);
            color: var(--bg-warm-grey);
        }

        .btn-primary:hover {
            background-color: transparent;
            color: var(--color-charcoal);
        }

        .btn-secondary {
            background-color: transparent;
            color: var(--color-charcoal);
        }

        .btn-secondary:hover {
            background-color: var(--color-charcoal);
            color: var(--bg-warm-grey);
        }

        /* Layered Interactive Parallax 3D Card Module */
        .hero-graphic-container {
            flex: 0.8;
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            perspective: 1200px;
            height: 100%;
        }

        .perspective-box {
            width: 280px;
            height: 380px;
            position: relative;
            transform-style: preserve-3d;
            transform: rotateY(-20deg) rotateX(15deg);
            transition: transform 0.1s linear;
        }

        .book-layer {
            position: absolute;
            width: 100%;
            height: 100%;
            box-shadow: 0 30px 60px rgba(0,0,0,0.1);
            transform-style: preserve-3d;
            backface-visibility: hidden;
        }

        .layer-back {
            background: #c7c3b9;
            transform: translateZ(-20px);
            border: 1px solid rgba(0,0,0,0.1);
        }

        .layer-middle {
            background: #e6e2d8;
            transform: translateZ(-10px);
            border: 1px solid rgba(0,0,0,0.05);
        }

        .layer-front {
            background: var(--color-off-white);
            border: 1px solid #1c1c1a;
            padding: 2.5rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            transform: translateZ(0px);
        }

        .paper-header {
            font-size: 0.7rem;
            letter-spacing: 0.3em;
            font-weight: 600;
            border-bottom: 1px solid var(--color-charcoal);
            padding-bottom: 0.5rem;
        }

        .paper-title {
            font-family: var(--font-serif);
            font-size: 2.2rem;
            line-height: 1.1;
            font-weight: 400;
        }

        .paper-footer {
            font-size: 0.65rem;
            letter-spacing: 0.15em;
            color: var(--color-muted-brown);
        }

        /* Universal Search Architecture Group */
        .search-section {
            background: var(--color-taupe);
        }

        .section-header-minimal {
            margin-bottom: 3rem;
        }

        .section-header-minimal h2 {
            font-family: var(--font-serif);
            font-size: 2.5rem;
            font-weight: 300;
        }

        .search-wrapper {
            position: relative;
            border-bottom: 1px solid var(--color-charcoal);
            display: flex;
            align-items: center;
        }

        #universal-search-input {
            width: 100%;
            background: transparent;
            border: none;
            padding: 1.5rem 0;
            font-family: var(--font-serif);
            font-size: 2rem;
            color: var(--color-charcoal);
            font-style: italic;
        }

        #universal-search-input:focus {
            outline: none;
        }

        .search-icon {
            font-size: 1.5rem;
            position: absolute;
            right: 0;
        }

        /* Asymmetric Dual Dashboard System Layout */
        .asymmetric-grid {
            display: grid;
            grid-template-columns: 1fr 1.3fr;
            gap: 8vw;
            align-items: start;
        }

        .asymmetric-grid.reverse {
            grid-template-columns: 1.3fr 1fr;
        }

        .section-info {
            position: sticky;
            top: 8rem;
        }

        .section-desc {
            font-size: 1.05rem;
            line-height: 1.7;
            color: var(--color-muted-brown);
            margin-bottom: 3rem;
            font-weight: 300;
        }

        /* Refined Form Dropdowns Control Infrastructure */
        .filter-group {
            margin-bottom: 2rem;
        }

        .filter-label {
            display: block;
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            margin-bottom: 0.6rem;
            font-weight: 600;
            color: var(--color-charcoal);
        }

        .luxury-select {
            width: 100%;
            padding: 1rem;
            background: transparent;
            border: 1px solid rgba(28, 28, 26, 0.2);
            font-family: var(--font-sans);
            font-size: 0.9rem;
            color: var(--color-charcoal);
            cursor: pointer;
            appearance: none;
            background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='10' height='10' viewBox='0 0 10 10'><path d='M0 3l5 5 5-5z' fill='%231c1c1a'/></svg>");
            background-repeat: no-repeat;
            background-position: right 1rem center;
            transition: var(--transition-smooth);
        }

        .luxury-select:focus {
            outline: none;
            border-color: var(--color-charcoal);
        }

        /* Custom Radio Group Buttons */
        .custom-radio-group {
            display: flex;
            gap: 0.5rem;
        }

        .radio-btn {
            background: transparent;
            border: 1px solid rgba(28, 28, 26, 0.2);
            padding: 0.8rem 1.5rem;
            font-family: var(--font-sans);
            font-size: 0.85rem;
            cursor: pointer;
            transition: var(--transition-smooth);
        }

        .radio-btn.active, .radio-btn:hover {
            background: var(--color-charcoal);
            color: var(--bg-warm-grey);
            border-color: var(--color-charcoal);
        }

        /* Archive List Content Layout Cards */
        .archive-list {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .paper-card-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 2rem;
            background: var(--color-off-white);
            border: 1px solid var(--color-glass-border);
            transition: var(--transition-smooth);
        }

        .paper-card-row:hover {
            transform: translateY(-4px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.04);
            border-color: var(--color-charcoal);
        }

        .card-meta-details {
            display: flex;
            flex-direction: column;
            gap: 0.4rem;
        }

        .meta-year-tag {
            font-family: var(--font-serif);
            font-size: 1.6rem;
            font-weight: 400;
        }

        .meta-sub-labels {
            font-size: 0.8rem;
            color: var(--color-muted-brown);
            font-weight: 400;
        }

        .meta-sub-labels span {
            margin-right: 0.8rem;
        }

        .card-action-links {
            display: flex;
            gap: 1rem;
        }

        .btn-inline {
            background: transparent;
            border: none;
            font-family: var(--font-sans);
            font-size: 0.75rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            cursor: pointer;
            padding: 0.5rem 0;
            border-bottom: 1px solid var(--color-charcoal);
            text-decoration: none;
            color: var(--color-charcoal);
            transition: var(--transition-smooth);
        }

        .btn-inline:hover {
            opacity: 0.6;
        }

        /* Strategic Counters Statistics Grid Layout */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 4rem;
            text-align: center;
        }

        .stat-item {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .stat-number {
            font-family: var(--font-serif);
            font-size: 4.5rem;
            font-weight: 300;
        }

        .stat-label {
            font-size: 0.85rem;
            text-transform: uppercase;
            letter-spacing: 0.15em;
            color: var(--color-muted-brown);
        }

        /* Continuous Elegant Typography Institutional Marquee */
        .institutions-section {
            overflow: hidden;
            background: var(--color-charcoal);
            color: var(--bg-warm-grey);
            padding: 4rem 0;
        }

        .marquee-wrapper {
            display: flex;
            width: 100%;
        }

        .marquee-content {
            display: flex;
            white-space: nowrap;
            gap: 4rem;
            animation: marquee-scroll 25s linear infinite;
            font-family: var(--font-serif);
            font-size: 4rem;
            font-weight: 300;
            letter-spacing: 0.05em;
        }

        .marquee-content span {
            display: flex;
            align-items: center;
        }

        @keyframes marquee-scroll {
            0% { transform: translateX(0%); }
            100% { transform: translateX(-50%); }
        }

        /* Testimonials Editorial Framework Layout */
        .testimonials-editorial-layout {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 6rem;
            margin-top: 4rem;
        }

        .testimonial-card {
            border-left: 1px solid var(--color-charcoal);
            padding-left: 2.5rem;
        }

        .layout-offset-down {
            margin-top: 4rem;
        }

        .quote-text {
            font-family: var(--font-serif);
            font-size: 1.6rem;
            line-height: 1.5;
            font-weight: 300;
            margin-bottom: 1.5rem;
        }

        .quote-author {
            font-style: normal;
            font-family: var(--font-sans);
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            color: var(--color-muted-brown);
        }

        /* Admin Dashboard Pipeline Ingestion Screen UI */
        .admin-wrapper-card {
            background: var(--color-off-white);
            border: 1px solid var(--color-charcoal);
            padding: 4rem;
        }

        .admin-header {
            margin-bottom: 3rem;
            border-bottom: 1px solid var(--color-glass-border);
            padding-bottom: 1.5rem;
        }

        .admin-header h2 {
            font-family: var(--font-serif);
            font-size: 2.5rem;
            font-weight: 300;
            margin-bottom: 0.5rem;
        }

        .admin-header p {
            font-size: 0.9rem;
            color: var(--color-muted-brown);
        }

        .admin-form-layout {
            display: flex;
            flex-direction: column;
            gap: 2.5rem;
        }

        .form-main-inputs {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 2rem;
        }

        .form-main-inputs .full-width {
            grid-column: span 2;
        }

        .form-group-luxury {
            display: flex;
            flex-direction: column;
            gap: 0.6rem;
        }

        .form-group-luxury label {
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 0.1rem;
            font-weight: 600;
        }

        .luxury-select-input, .luxury-text-input {
            width: 100%;
            padding: 1.1rem;
            background: var(--bg-warm-grey);
            border: 1px solid var(--color-glass-border);
            font-family: var(--font-sans);
            font-size: 0.9rem;
            color: var(--color-charcoal);
            transition: var(--transition-smooth);
        }

        .luxury-select-input:focus, .luxury-text-input:focus {
            outline: none;
            border-color: var(--color-charcoal);
            background: #fff;
        }

        /* File Drag & Drop Target Interface */
        .drag-drop-zone {
            border: 1px dashed var(--color-charcoal);
            background: var(--bg-warm-grey);
            padding: 4rem;
            text-align: center;
            cursor: pointer;
            transition: var(--transition-smooth);
        }

        .drag-drop-zone.drag-over {
            background: var(--color-taupe);
            transform: scale(0.99);
        }

        .upload-cloud-icon {
            font-size: 2rem;
            display: block;
            margin-bottom: 1rem;
        }

        .drop-zone-text {
            font-size: 0.9rem;
            color: var(--color-muted-brown);
        }

        .browse-link {
            text-decoration: underline;
            color: var(--color-charcoal);
            font-weight: 500;
        }

        .file-details-visible {
            margin-top: 1rem;
            font-size: 0.85rem;
            font-weight: 600;
            color: var(--color-charcoal);
            background: rgba(0,0,0,0.04);
            padding: 0.5rem 1rem;
            display: inline-block;
        }

        .file-details-hidden {
            display: none;
        }

        .submit-upload-btn {
            align-self: flex-start;
        }

        /* Luxury Footprint Identity Block Area */
        .luxury-footer {
            background: #111;
            color: #999;
            padding: 6rem 10vw 3rem 10vw;
            font-family: var(--font-sans);
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 2fr repeat(2, 1fr);
            gap: 4rem;
            padding-bottom: 4rem;
            border-bottom: 1px solid rgba(255,255,255,0.05);
        }

        .footer-brand-column {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .footer-logo {
            color: #fff;
            font-weight: 600;
            letter-spacing: 0.2em;
            font-size: 1.2rem;
        }

        .footer-essence {
            font-size: 0.9rem;
            line-height: 1.6;
            max-width: 320px;
            font-weight: 300;
        }

        .footer-links-column {
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }

        .footer-links-column .column-title {
            color: #fff;
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 0.15em;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }

        .footer-links-column a {
            color: #888;
            text-decoration: none;
            font-size: 0.85rem;
            transition: var(--transition-smooth);
        }

        .footer-links-column a:hover {
            color: #fff;
        }

        .footer-bottom-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 2rem;
            font-size: 0.8rem;
        }

        .social-links {
            display: flex;
            gap: 2rem;
        }

        .social-link {
            color: #888;
            text-decoration: none;
            transition: var(--transition-smooth);
        }

        .social-link:hover {
            color: #fff;
        }

        /* Micro-interaction Notification Toast */
        #notification-toast {
            position: fixed;
            bottom: 2rem;
            right: 2rem;
            background: var(--color-charcoal);
            color: var(--color-off-white);
            padding: 1rem 2rem;
            font-size: 0.85rem;
            letter-spacing: 0.05em;
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
            z-index: 10000;
            transform: translateY(150%);
            transition: transform 0.5s cubic-bezier(0.16, 1, 0.3, 1);
        }

        #notification-toast.visible {
            transform: translateY(0);
        }

        /* ==========================================================================
           Responsive Adaptations (Mobile-First / Breakpoint Engineering)
           ========================================================================== */

        @media(max-width: 1024px) {
            .hero-title { font-size: 4rem; }
            .asymmetric-grid, .asymmetric-grid.reverse {
                grid-template-columns: 1fr;
                gap: 4rem;
            }
            .section-info { position: relative; top: 0; }
            .stats-grid { gap: 2rem; }
        }

        @media(max-width: 768px) {
            .section-padding { padding: 4rem 6vw; }
            .grid-line-overlay { display: none; }
            .hero-section { flex-direction: column-reverse; padding-top: 8rem; text-align: center; gap: 2rem;}
            .hero-tagline { margin-left: auto; margin-right: auto; }
            .hero-actions { justify-content: center; }
            .nav-links {
                display: none;
                position: absolute; top: 100%; left: 0; width: 100%;
                background: var(--bg-warm-grey); flex-direction: column;
                padding: 2rem; gap: 1.5rem; border-bottom: 1px solid var(--color-glass-border);
            }
            .nav-links.mobile-open { display: flex; }
            .mobile-nav-toggle { display: flex; }
            .stats-grid { grid-template-columns: 1fr; }
            .testimonials-editorial-layout { grid-template-columns: 1fr; gap: 3rem; }
            .layout-offset-down { margin-top: 0; }
            .form-main-inputs { grid-template-columns: 1fr; }
            .form-main-inputs .full-width { grid-column: span 1; }
            .admin-wrapper-card { padding: 2rem 1.5rem; }
            .footer-grid { grid-template-columns: 1fr; gap: 3rem; }
        }
    </style>
</head>
<body>

    <div class="grid-line-overlay">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
    </div>

    <nav class="nav-container">
        <div class="nav-brand">EXAM ARCHIVE</div>
        <div class="nav-links">
            <a href="#hero" class="nav-link active">Home</a>
            <a href="#jee-main" class="nav-link">JEE Main</a>
            <a href="#jee-advanced" class="nav-link">JEE Advanced</a>
            <a href="#neet" class="nav-link">NEET</a>
            <a href="#admin-upload" class="nav-link admin-trigger-btn">Upload</a>
            <a href="#institutions" class="nav-link">About</a>
        </div>
        <button class="mobile-nav-toggle" aria-label="Toggle menu">
            <span></span><span></span>
        </button>
    </nav>

    <header id="hero" class="hero-section">
        <div class="hero-content">
            <div class="editorial-header">
                <span class="eyebrow-text">The Academic Repository</span>
                <h1 class="hero-title">Exam Archive<br><span class="serif-italic">JEE & NEET PYQs</span></h1>
            </div>
            <p class="hero-tagline">Making preparation accessible through beautifully organized academic resources. Designed for clarity, curated for performance.</p>
            <div class="hero-actions">
                <a href="#search-section" class="btn btn-primary">Explore Archive</a>
                <a href="#jee-main" class="btn btn-secondary">Browse Series</a>
            </div>
        </div>

        <div class="hero-graphic-container">
            <div class="perspective-box" id="interactive-book">
                <div class="book-layer layer-back"></div>
                <div class="book-layer layer-middle"></div>
                <div class="book-layer layer-front">
                    <div class="paper-header">CONFIDENTIAL</div>
                    <div class="paper-title">ARCHIVE 2002 — 2026</div>
                    <div class="paper-footer">NATIONAL TESTING REPOSITORY</div>
                </div>
            </div>
        </div>
    </header>

    <section id="search-section" class="search-section section-padding">
        <div class="section-header-minimal">
            <span class="section-index">01</span>
            <h2>Universal Search</h2>
        </div>
        <div class="search-wrapper">
            <input type="text" id="universal-search-input" placeholder="Search by year, exam, subject or keyword (e.g., 2024 Physics)..." aria-label="Search across papers">
            <span class="search-icon">🔍</span>
        </div>
    </section>

    <section id="jee-main" class="exam-section section-padding">
        <div class="asymmetric-grid">
            <div class="section-info">
                <span class="section-index">02</span>
                <h2 class="section-title-editorial">JEE Main<br><span class="serif-italic">Archive Portfolio</span></h2>
                <p class="section-desc">Comprehensive structural cataloging of JEE Main examinations from 2002 to the present era. Refined and sorted for seamless indexing.</p>
                
                <div class="filter-group">
                    <label class="filter-label">Filter by Academic Year</label>
                    <select id="jee-main-year" class="luxury-select">
                        <option value="all">All Available Years</option>
                        <option value="2025">2025 Papers</option>
                        <option value="2024">2024 Papers</option>
                        <option value="2023">2023 Papers</option>
                        <option value="2022">2022 Papers</option>
                        <option value="2020">2020 Papers</option>
                        <option value="2019">2019 Papers</option>
                        <option value="2012">2012 Papers</option>
                        <option value="2002">2002 Papers</option>
                    </select>
                </div>
                <div class="filter-group">
                    <label class="filter-label">Session Assignment</label>
                    <select id="jee-main-session" class="luxury-select">
                        <option value="all">All Sessions</option>
                        <option value="session-1">Session I (January)</option>
                        <option value="session-2">Session II (April)</option>
                    </select>
                </div>
            </div>
            
            <div class="papers-display-panel">
                <div class="archive-list" id="jee-main-list">
                    </div>
            </div>
        </div>
    </section>

    <section id="jee-advanced" class="exam-section section-padding border-top-grid">
        <div class="asymmetric-grid reverse">
            <div class="papers-display-panel">
                <div class="archive-list" id="jee-advanced-list">
                    </div>
            </div>
            <div class="section-info">
                <span class="section-index">03</span>
                <h2 class="section-title-editorial">JEE Advanced<br><span class="serif-italic">Deep Synthesis</span></h2>
                <p class="section-desc">Splitting analytical frameworks into Paper 1 and Paper 2 archives. Complete integrated solutions catalogs available for download.</p>
                
                <div class="filter-group">
                    <label class="filter-label">Select Paper Type</label>
                    <div class="custom-radio-group">
                        <button class="radio-btn active" data-paper-type="all">All</button>
                        <button class="radio-btn" data-paper-type="Paper 1">Paper 1</button>
                        <button class="radio-btn" data-paper-type="Paper 2">Paper 2</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="neet" class="exam-section section-padding border-top-grid">
        <div class="asymmetric-grid">
            <div class="section-info">
                <span class="section-index">04</span>
                <h2 class="section-title-editorial">NEET National<br><span class="serif-italic">Medical Registry</span></h2>
                <p class="section-desc">Year-wise structured question paper vaults combined with state-specific language localization criteria.</p>
                
                <div class="filter-group">
                    <label class="filter-label">Language / Translation Profile</label>
                    <select id="neet-language" class="luxury-select">
                        <option value="all">All Languages Available</option>
                        <option value="English">English</option>
                        <option value="Hindi">Hindi / हिंदी</option>
                        <option value="Bengali">Bengali</option>
                    </select>
                </div>
            </div>
            <div class="papers-display-panel">
                <div class="archive-list" id="neet-list">
                    </div>
            </div>
        </div>
    </section>

    <section class="statistics-section section-padding border-top-grid">
        <div class="stats-grid">
            <div class="stat-item">
                <span class="stat-number" data-target="1450">0</span>
                <span class="stat-label">Total Curated Papers</span>
            </div>
            <div class="stat-item">
                <span class="stat-number" data-target="920">0</span>
                <span class="stat-label">Verified Solutions</span>
            </div>
            <div class="stat-item">
                <span class="stat-number" data-target="320">0</span>
                <span class="stat-label">K+ Global Downloads</span>
            </div>
        </div>
    </section>

    <section id="institutions" class="institutions-section section-padding">
        <div class="marquee-wrapper">
            <div class="marquee-content">
                <span>IIT</span><span>•</span>
                <span>NIT</span><span>•</span>
                <span>AIIMS</span><span>•</span>
                <span>NCERT</span><span>•</span>
                <span>IIT</span><span>•</span>
                <span>NIT</span><span>•</span>
                <span>AIIMS</span><span>•</span>
                <span>NCERT</span><span>•</span>
            </div>
        </div>
    </section>

    <section class="testimonials-section section-padding border-top-grid">
        <div class="section-header-minimal">
            <span class="section-index">05</span>
            <h2>Scholarly Review</h2>
        </div>
        <div class="testimonials-editorial-layout">
            <blockquote class="testimonial-card">
                <p class="quote-text">“The minimalist structure provided by Exam Archive is unparalleled. I wasted zero time browsing clunky forums. Everything loads elegantly like a digital magazine portfolio.”</p>
                <cite class="quote-author">— Aravind K., IIT Bombay (Rank 42)</cite>
            </blockquote>
            <blockquote class="testimonial-card layout-offset-down">
                <p class="quote-text">“The presence of precise language filers and clean PDF previews created an optimal flow for my NEET revision patterns. Truly a premium repository.”</p>
                <cite class="quote-author">— Meera J., AIIMS New Delhi</cite>
            </blockquote>
        </div>
    </section>

    <section id="admin-upload" class="admin-section section-padding border-top-grid">
        <div class="admin-wrapper-card glass-panel">
            <div class="admin-header">
                <h2>Repository Ingestion Dashboard</h2>
                <p>Curator Access — Structure & publish architectural document archives directly into database structures.</p>
            </div>
            
            <form id="upload-form" class="admin-form-layout" onsubmit="event.preventDefault();">
                <div class="form-main-inputs">
                    <div class="form-group-luxury">
                        <label>Examination Framework</label>
                        <select id="upload-exam" class="luxury-select-input" required>
                            <option value="">Select Target Platform...</option>
                            <option value="JEE Main">JEE Main</option>
                            <option value="JEE Advanced">JEE Advanced</option>
                            <option value="NEET">NEET</option>
                        </select>
                    </div>
                    <div class="form-group-luxury">
                        <label>Academic Year</label>
                        <input type="number" id="upload-year" min="2000" max="2027" placeholder="e.g., 2026" class="luxury-text-input" required>
                    </div>
                    <div class="form-group-luxury">
                        <label>Session / Variant Label</label>
                        <input type="text" id="upload-session" placeholder="e.g., Session 1 / Paper 2" class="luxury-text-input" required>
                    </div>
                    <div class="form-group-luxury">
                        <label>Language Classification</label>
                        <input type="text" id="upload-language" placeholder="e.g., English, Hindi" class="luxury-text-input" required>
                    </div>
                    <div class="form-group-luxury full-width">
                        <label>Subject Domain Metadata Tags</label>
                        <input type="text" id="upload-subject" placeholder="e.g., Physics, Chemistry, Mathematics Full Length" class="luxury-text-input" required>
                    </div>
                </div>

                <div id="drop-zone" class="drag-drop-zone">
                    <div class="drop-zone-content">
                        <span class="upload-cloud-icon">🗂️</span>
                        <p class="drop-zone-text">Drag and drop verified paper PDF file or <span class="browse-link">click here to browse files</span></p>
                        <input type="file" id="file-input" accept="application/pdf" hidden>
                        <div id="file-details" class="file-details-hidden"></div>
                    </div>
                </div>

                <button type="submit" class="btn btn-primary submit-upload-btn">Initialize Pipeline Verification</button>
            </form>
        </div>
    </section>

    <footer class="luxury-footer">
        <div class="footer-grid">
            <div class="footer-brand-column">
                <span class="footer-logo">EXAM ARCHIVE</span>
                <p class="footer-essence">An editorial curation of historical competitive testing blueprints for premium preparation execution.</p>
            </div>
            <div class="footer-links-column">
                <span class="column-title">Frameworks</span>
                <a href="#jee-main">JEE Main Core</a>
                <a href="#jee-advanced">JEE Advanced Matrix</a>
                <a href="#neet">NEET Repository</a>
            </div>
            <div class="footer-links-column">
                <span class="column-title">Legal & Identity</span>
                <a href="#">Privacy Protocol</a>
                <a href="#">Terms of Use</a>
                <a href="#">Archival Integrity</a>
            </div>
        </div>
        <div class="footer-bottom-bar">
            <p class="copyright-text">&copy; 2026 Exam Archive Studio. Built with clean typographic precision.</p>
            <div class="social-links">
                <a href="#" class="social-link">Instagram</a>
                <a href="#" class="social-link">LinkedIn</a>
                <a href="#" class="social-link">GitHub</a>
            </div>
        </div>
    </footer>

    <div id="notification-toast" class="notification-toast-hidden"></div>

    <script>
        /**
         * Exam Archive — Premium Identity Platform Interaction Lifecycle Scripts
         */

        const ARCHIVE_REGISTRY = [
            { id: 1, exam: "JEE Main", year: 2025, session: "session-1", language: "English", subject: "Full Length Set A", type: "Paper 1" },
            { id: 2, exam: "JEE Main", year: 2024, session: "session-2", language: "English", subject: "Physics & Chemistry Depth", type: "Paper 1" },
            { id: 3, exam: "JEE Main", year: 2023, session: "session-1", language: "Hindi", subject: "Mathematics Linear Pack", type: "Paper 2" },
            { id: 4, exam: "JEE Advanced", year: 2025, session: "all", language: "English", subject: "Advanced Physics Systems", type: "Paper 1" },
            { id: 5, exam: "JEE Advanced", year: 2024, session: "all", language: "English", subject: "Comprehensive Paper 2 Cluster", type: "Paper 2" },
            { id: 6, exam: "NEET", year: 2025, session: "all", language: "English", subject: "Biological Sciences Portfolio", type: "Paper 1" },
            { id: 7, exam: "NEET", year: 2024, session: "all", language: "Hindi", subject: "All-India Structural Variant B", type: "Paper 1" },
            { id: 8, exam: "NEET", year: 2022, session: "all", language: "Bengali", subject: "Regional Vernacular Booklet", type: "Paper 1" },
            { id: 9, exam: "JEE Main", year: 2012, session: "session-1", language: "English", subject: "AIEEE Legacy Archive", type: "Paper 1" },
            { id: 10, exam: "JEE Main", year: 2002, session: "session-1", language: "English", subject: "Inaugural Framework Architecture", type: "Paper 1" }
        ];

        document.addEventListener("DOMContentLoaded", () => {
            renderExams();
            initializeSearchEngines();
            setupInteractions3D();
            setupAdminIngestionEngine();
            setupScrollAnimations();
            setupMobileMenu();
        });

        function renderExams(filterCriteria = null) {
            const panels = {
                "JEE Main": document.getElementById("jee-main-list"),
                "JEE Advanced": document.getElementById("jee-advanced-list"),
                "NEET": document.getElementById("neet-list")
            };

            Object.values(panels).forEach(p => { if(p) p.innerHTML = ""; });

            ARCHIVE_REGISTRY.forEach(paper => {
                if (filterCriteria) {
                    if (filterCriteria.type === "search") {
                        const q = filterCriteria.query.toLowerCase();
                        const match = paper.exam.toLowerCase().includes(q) || 
                                      paper.year.toString().includes(q) || 
                                      paper.subject.toLowerCase().includes(q) || 
                                      paper.language.toLowerCase().includes(q);
                        if (!match) return;
                    } else {
                        if (paper.exam === "JEE Main") {
                            const yFilter = document.getElementById("jee-main-year").value;
                            const sFilter = document.getElementById("jee-main-session").value;
                            if (yFilter !== "all" && paper.year.toString() !== yFilter) return;
                            if (sFilter !== "all" && paper.session !== sFilter) return;
                        }
                        if (paper.exam === "JEE Advanced") {
                            const activeRadio = document.querySelector(".radio-btn.active");
                            const pType = activeRadio ? activeRadio.getAttribute("data-paper-type") : "all";
                            if (pType !== "all" && paper.type !== pType) return;
                        }
                        if (paper.exam === "NEET") {
                            const lFilter = document.getElementById("neet-language").value;
                            if (lFilter !== "all" && paper.language !== lFilter) return;
                        }
                    }
                }

                const card = document.createElement("div");
                card.className = "paper-card-row";
                card.innerHTML = `
                    <div class="card-meta-details">
                        <span class="meta-year-tag">${paper.exam} — ${paper.year}</span>
                        <div class="meta-sub-labels">
                            <span>Domain: ${paper.subject}</span>
                            <span>•</span>
                            <span>Lang: ${paper.language}</span>
                            ${paper.session !== 'all' ? `<span>•</span><span>${paper.session.replace('-', ' ')}</span>` : ''}
                        </div>
                    </div>
                    <div class="card-action-links">
                        <a href="#" class="btn-inline view-pdf-action" data-id="${paper.id}">Preview Map</a>
                        <a href="#" class="btn-inline download-pdf-action" data-id="${paper.id}">Download Archive</a>
                    </div>
                `;

                if (panels[paper.exam]) {
                    panels[paper.exam].appendChild(card);
                }
            });

            Object.entries(panels).forEach(([key, element]) => {
                if (element && element.children.length === 0) {
                    element.innerHTML = `<p style="font-family: var(--font-serif); font-style: italic; color: var(--color-muted-brown); padding: 2rem 0;">No matching archival assets indexed for this matrix configuration.</p>`;
                }
            });

            attachCardActionListeners();
        }

        function initializeSearchEngines() {
            const searchInput = document.getElementById("universal-search-input");
            searchInput.addEventListener("input", (e) => {
                const val = e.target.value;
                if (val.trim() !== "") {
                    renderExams({ type: "search", query: val });
                } else {
                    renderExams();
                }
            });

            ["jee-main-year", "jee-main-session", "neet-language"].forEach(id => {
                const element = document.getElementById(id);
                if (element) element.addEventListener("change", () => renderExams({ type: "dropdown" }));
            });

            const radioButtons = document.querySelectorAll(".radio-btn");
            radioButtons.forEach(btn => {
                btn.addEventListener("click", (e) => {
                    radioButtons.forEach(b => b.classList.remove("active"));
                    e.target.classList.add("active");
                    renderExams({ type: "radio" });
                });
            });
        }

        function triggerToastNotification(message) {
            const toast = document.getElementById("notification-toast");
            toast.textContent = message;
            toast.classList.add("visible");
            setTimeout(() => {
                toast.classList.remove("visible");
            }, 4000);
        }

        function attachCardActionListeners() {
            document.querySelectorAll(".view-pdf-action").forEach(btn => {
                btn.onclick = (e) => {
                    e.preventDefault();
                    triggerToastNotification("Initializing Sandboxed Cloud PDF View Frame Preview...");
                };
            });
            document.querySelectorAll(".download-pdf-action").forEach(btn => {
                btn.onclick = (e) => {
                    e.preventDefault();
                    triggerToastNotification("Archival Asset Successfully Syntsembled & Dispatched to Pipeline.");
                };
            });
        }

        function setupInteractions3D() {
            const book = document.getElementById("interactive-book");
            const container = document.querySelector(".hero-graphic-container");
            if (!container || !book) return;

            container.addEventListener("mousemove", (e) => {
                const rect = container.getBoundingClientRect();
                const x = e.clientX - rect.left - (rect.width / 2);
                const y = e.clientY - rect.top - (rect.height / 2);
                
                const tiltX = (y / (rect.height / 2)) * -25;
                const tiltY = (x / (rect.width / 2)) * 25;

                book.style.transform = `rotateY(${tiltY}deg) rotateX(${tiltX}deg)`;
            });

            container.addEventListener("mouseleave", () => {
                book.style.transform = `rotateY(-20deg) rotateX(15deg)`;
            });
        }

        function setupScrollAnimations() {
            window.addEventListener("scroll", () => {
                const scrolled = window.pageYOffset;
                const book = document.getElementById("interactive-book");
                if (book) {
                    const rotationOffset = -20 + (scrolled * 0.08);
                    const openZ = Math.min(scrolled * 0.1, 40);
                    book.style.transform = `rotateY(${rotationOffset}deg) rotateX(15deg) translateZ(${openZ}px)`;
                }
            });

            const statsSection = document.querySelector(".statistics-section");
            if (!statsSection) return;

            let metricsTriggered = false;
            const observer = new IntersectionObserver((entries) => {
                if(entries[0].isIntersecting && !metricsTriggered) {
                    metricsTriggered = true;
                    document.querySelectorAll(".stat-number").forEach(num => {
                        const target = parseInt(num.getAttribute("data-target"), 10);
                        let current = 0;
                        const increment = Math.ceil(target / 40);
                        const timer = setInterval(() => {
                            current += increment;
                            if(current >= target) {
                                num.textContent = target;
                                clearInterval(timer);
                            } else {
                                num.textContent = current;
                            }
                        }, 25);
                    });
                }
            }, { threshold: 0.3 });

            observer.observe(statsSection);
        }

        function setupAdminIngestionEngine() {
            const dropZone = document.getElementById("drop-zone");
            const fileInput = document.getElementById("file-input");
            const fileDetails = document.getElementById("file-details");
            const uploadForm = document.getElementById("upload-form");

            if (!dropZone || !fileInput) return;

            dropZone.addEventListener("click", () => fileInput.click());

            dropZone.addEventListener("dragover", (e) => {
                e.preventDefault();
                dropZone.classList.add("drag-over");
            });

            ["dragleave", "drop"].forEach(evt => {
                dropZone.addEventListener(evt, () => dropZone.classList.remove("drag-over"));
            });

            dropZone.addEventListener("drop", (e) => {
                e.preventDefault();
                if(e.dataTransfer.files.length) {
                    fileInput.files = e.dataTransfer.files;
                    handleFileVerification(e.dataTransfer.files[0]);
                }
            });

            fileInput.addEventListener("change", () => {
                if(fileInput.files.length) handleFileVerification(fileInput.files[0]);
            });

            function handleFileVerification(file) {
                if(file.type !== "application/pdf") {
                    triggerToastNotification("Security Error: Target payload format must be a standard valid document PDF.");
                    fileInput.value = "";
                    fileDetails.className = "file-details-hidden";
                    return;
                }
                fileDetails.className = "file-details-visible";
                fileDetails.textContent = `Target Payload Confirmed: ${file.name} [${(file.size/(1024*1024)).toFixed(2)} MB]`;
            }

            if (uploadForm) {
                uploadForm.addEventListener("submit", (e) => {
                    e.preventDefault();
                    if(!fileInput.files.length) {
                        triggerToastNotification("Validation Warning: No historical archive PDF bounded to payload stream.");
                        return;
                    }

                    const mockPayload = {
                        id: ARCHIVE_REGISTRY.length + 1,
                        exam: document.getElementById("upload-exam").value,
                        year: parseInt(document.getElementById("upload-year").value, 10),
                        session: document.getElementById("upload-session").value || "all",
                        language: document.getElementById("upload-language").value,
                        subject: document.getElementById("upload-subject").value,
                        type: "Paper 1"
                    };

                    ARCHIVE_REGISTRY.unshift(mockPayload);
                    renderExams();
                    triggerToastNotification(`Archival Object Stream Injected Successfully into ${mockPayload.exam} Clusters.`);
                    
                    uploadForm.reset();
                    fileDetails.className = "file-details-hidden";
                });
            }
        }

        function setupMobileMenu() {
            const toggle = document.querySelector(".mobile-nav-toggle");
            const links = document.querySelector(".nav-links");
            if (!toggle || !links) return;

            toggle.addEventListener("click", () => {
                links.classList.toggle("mobile-open");
            });

            document.querySelectorAll(".nav-link").forEach(l => {
                l.addEventListener("click", () => links.classList.remove("mobile-open"));
            });
        }
    </script>
</body>
</html>
