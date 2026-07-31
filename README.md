<!-- Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Exo+2:wght@300;400;500;600;700&family=Orbitron:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<!-- Font Awesome -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<!-- React & ReactDOM -->
<script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>

<!-- Babel -->
<script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>

<style>
    :root {
        --primary: #0D1B2A;
        --secondary: #1B263B;
        --accent: #E63946;
        --accent-secondary: #F77F00;
        --success: #2ECC71;
        --background: #FFFFFF;
        --text-primary: #1A1A2E;
        --text-secondary: #4A4A68;
        --card-bg: #F8F9FA;
        --border: #E1E5E9;
    }

    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    body {
        font-family: 'Exo 2', sans-serif;
        color: var(--text-primary);
        background: var(--background);
        overflow-x: hidden;
    }

    h1, h2, h3, h4, h5, h6 {
        font-family: 'Orbitron', sans-serif;
    }

    /* Scrollbar */
    ::-webkit-scrollbar {
        width: 8px;
    }

    ::-webkit-scrollbar-track {
        background: var(--card-bg);
    }

    ::-webkit-scrollbar-thumb {
        background: var(--accent);
        border-radius: 4px;
    }

    /* Animations */
    @keyframes float {
        0%, 100% { transform: translateY(0); }
        50% { transform: translateY(-10px); }
    }

    @keyframes pulse {
        0%, 100% { transform: scale(1); opacity: 1; }
        50% { transform: scale(1.1); opacity: 0.8; }
    }

    @keyframes slideIn {
        from { opacity: 0; transform: translateY(20px); }
        to { opacity: 1; transform: translateY(0); }
    }

    @keyframes glow {
        0%, 100% { box-shadow: 0 0 20px rgba(230, 57, 70, 0.3); }
        50% { box-shadow: 0 0 40px rgba(230, 57, 70, 0.6); }
    }

    @keyframes scan {
        0% { top: 0; }
        50% { top: calc(100% - 4px); }
        100% { top: 0; }
    }

    /* Navbar */
    .navbar {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        z-index: 1000;
        background: rgba(13, 27, 42, 0.95);
        backdrop-filter: blur(10px);
        padding: 1rem 2rem;
        transition: all 0.3s ease;
    }

    .navbar-container {
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .logo {
        display: flex;
        align-items: center;
        gap: 10px;
        color: white;
        text-decoration: none;
    }

    .logo-icon {
        font-size: 2rem;
        color: var(--accent);
        animation: float 3s ease-in-out infinite;
    }

    .logo-text {
        font-family: 'Orbitron', sans-serif;
        font-size: 1.5rem;
        font-weight: 700;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }

    .nav-links {
        display: flex;
        gap: 2rem;
        list-style: none;
    }

    .nav-links a {
        color: white;
        text-decoration: none;
        font-weight: 500;
        transition: color 0.3s;
        position: relative;
    }

    .nav-links a::after {
        content: '';
        position: absolute;
        bottom: -5px;
        left: 0;
        width: 0;
        height: 2px;
        background: var(--accent);
        transition: width 0.3s;
    }

    .nav-links a:hover {
        color: var(--accent);
    }

    .nav-links a:hover::after {
        width: 100%;
    }

    .mobile-menu-btn {
        display: none;
        color: white;
        font-size: 1.5rem;
        cursor: pointer;
    }

    /* Hero Section */
    .hero {
        min-height: 100vh;
        background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 120px 2rem 80px;
        position: relative;
        overflow: hidden;
    }

    .hero::before {
        content: '';
        position: absolute;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.03'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        opacity: 0.5;
    }

    .hero-content {
        max-width: 900px;
        text-align: center;
        position: relative;
        z-index: 1;
    }

    .hero h1 {
        font-size: 3.5rem;
        color: white;
        margin-bottom: 1.5rem;
        line-height: 1.2;
        animation: slideIn 0.8s ease-out;
    }

    .hero h1 span {
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }

    .hero p {
        font-size: 1.25rem;
        color: rgba(255, 255, 255, 0.8);
        margin-bottom: 2.5rem;
        animation: slideIn 0.8s ease-out 0.2s both;
    }

    .search-container {
        display: flex;
        gap: 1rem;
        max-width: 600px;
        margin: 0 auto 2rem;
        animation: slideIn 0.8s ease-out 0.4s both;
    }

    .search-input {
        flex: 1;
        padding: 1rem 1.5rem;
        border: none;
        border-radius: 50px;
        font-size: 1rem;
        font-family: 'Exo 2', sans-serif;
        box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
        outline: none;
        transition: all 0.3s;
    }

    .search-input:focus {
        transform: scale(1.02);
        box-shadow: 0 15px 50px rgba(0, 0, 0, 0.3);
    }

    .search-btn {
        padding: 1rem 2rem;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        border: none;
        border-radius: 50px;
        color: white;
        font-size: 1rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        font-family: 'Orbitron', sans-serif;
    }

    .search-btn:hover {
        transform: scale(1.05);
        animation: glow 1.5s ease-in-out infinite;
    }

    .cta-buttons {
        display: flex;
        gap: 1rem;
        justify-content: center;
        animation: slideIn 0.8s ease-out 0.6s both;
    }

    .btn-primary {
        padding: 1rem 2.5rem;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        border: none;
        border-radius: 50px;
        color: white;
        font-size: 1.1rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        font-family: 'Orbitron', sans-serif;
        text-decoration: none;
    }

    .btn-primary:hover {
        transform: translateY(-3px);
        box-shadow: 0 15px 40px rgba(230, 57, 70, 0.4);
    }

    .btn-secondary {
        padding: 1rem 2.5rem;
        background: transparent;
        border: 2px solid white;
        border-radius: 50px;
        color: white;
        font-size: 1.1rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        font-family: 'Orbitron', sans-serif;
        text-decoration: none;
    }

    .btn-secondary:hover {
        background: white;
        color: var(--primary);
    }

    /* Floating Elements */
    .floating-parts {
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        pointer-events: none;
        overflow: hidden;
    }

    .floating-icon {
        position: absolute;
        font-size: 3rem;
        color: rgba(255, 255, 255, 0.1);
        animation: float 6s ease-in-out infinite;
    }

    /* Features Section */
    .features {
        padding: 80px 2rem;
        background: var(--background);
    }

    .container {
        max-width: 1200px;
        margin: 0 auto;
    }

    .section-header {
        text-align: center;
        margin-bottom: 60px;
    }

    .section-header h2 {
        font-size: 2.5rem;
        color: var(--primary);
        margin-bottom: 1rem;
    }

    .section-header p {
        font-size: 1.1rem;
        color: var(--text-secondary);
        max-width: 600px;
        margin: 0 auto;
    }

    .features-grid {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 2rem;
    }

    .feature-card {
        background: var(--card-bg);
        padding: 2rem;
        border-radius: 20px;
        text-align: center;
        transition: all 0.3s;
        border: 1px solid var(--border);
    }

    .feature-card:hover {
        transform: translateY(-8px);
        box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
        border-color: var(--accent);
    }

    .feature-icon {
        width: 80px;
        height: 80px;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        border-radius: 20px;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 auto 1.5rem;
        font-size: 2rem;
        color: white;
    }

    .feature-card h3 {
        font-size: 1.3rem;
        color: var(--primary);
        margin-bottom: 1rem;
    }

    .feature-card p {
        color: var(--text-secondary);
        line-height: 1.6;
    }

    /* How It Works */
    .how-it-works {
        padding: 80px 2rem;
        background: linear-gradient(180deg, var(--card-bg) 0%, var(--background) 100%);
    }

    .steps {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 3rem;
        position: relative;
    }

    .steps::before {
        content: '';
        position: absolute;
        top: 60px;
        left: 15%;
        right: 15%;
        height: 3px;
        background: linear-gradient(90deg, var(--accent), var(--accent-secondary));
        z-index: 0;
    }

    .step {
        text-align: center;
        position: relative;
        z-index: 1;
    }

    .step-number {
        width: 80px;
        height: 80px;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 auto 1.5rem;
        font-family: 'Orbitron', sans-serif;
        font-size: 1.8rem;
        font-weight: 700;
        color: white;
        box-shadow: 0 10px 30px rgba(230, 57, 70, 0.3);
    }

    .step h3 {
        font-size: 1.4rem;
        color: var(--primary);
        margin-bottom: 1rem;
    }

    .step p {
        color: var(--text-secondary);
        line-height: 1.6;
    }

    /* Price Comparison */
    .price-comparison {
        padding: 80px 2rem;
        background: var(--background);
    }

    .filters {
        display: flex;
        gap: 1rem;
        margin-bottom: 2rem;
        flex-wrap: wrap;
    }

    .filter-btn {
        padding: 0.75rem 1.5rem;
        background: var(--card-bg);
        border: 2px solid var(--border);
        border-radius: 30px;
        font-family: 'Exo 2', sans-serif;
        font-size: 0.9rem;
        font-weight: 500;
        cursor: pointer;
        transition: all 0.3s;
        color: var(--text-secondary);
    }

    .filter-btn:hover, .filter-btn.active {
        background: var(--accent);
        border-color: var(--accent);
        color: white;
    }

    .sort-select {
        padding: 0.75rem 1.5rem;
        background: var(--card-bg);
        border: 2px solid var(--border);
        border-radius: 30px;
        font-family: 'Exo 2', sans-serif;
        font-size: 0.9rem;
        cursor: pointer;
        outline: none;
        color: var(--text-secondary);
    }

    .price-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
        gap: 2rem;
    }

    .price-card {
        background: var(--card-bg);
        border-radius: 20px;
        overflow: hidden;
        border: 1px solid var(--border);
        transition: all 0.3s;
    }

    .price-card:hover {
        transform: translateY(-8px);
        box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
    }

    .price-card-header {
        background: linear-gradient(135deg, var(--primary), var(--secondary));
        padding: 1.5rem;
        color: white;
    }

    .part-image {
        width: 100%;
        height: 150px;
        background: white;
        border-radius: 15px;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 4rem;
        color: var(--text-secondary);
        margin-bottom: 1rem;
    }

    .price-card-header h3 {
        font-size: 1.2rem;
        margin-bottom: 0.5rem;
    }

    .part-number {
        font-size: 0.85rem;
        opacity: 0.8;
    }

    .price-card-body {
        padding: 1.5rem;
    }

    .shop-prices {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    .shop-price {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem;
        background: white;
        border-radius: 12px;
        border: 1px solid var(--border);
        transition: all 0.3s;
    }

    .shop-price:hover {
        border-color: var(--accent);
        transform: translateX(5px);
    }

    .shop-info {
        display: flex;
        align-items: center;
        gap: 0.75rem;
    }

    .shop-icon {
        width: 40px;
        height: 40px;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        border-radius: 10px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-weight: 600;
    }

    .shop-name {
        font-weight: 600;
        color: var(--primary);
    }

    .shop-distance {
        font-size: 0.8rem;
        color: var(--text-secondary);
    }

    .price-value {
        text-align: right;
    }

    .price-amount {
        font-size: 1.3rem;
        font-weight: 700;
        color: var(--primary);
    }

    .price-original {
        font-size: 0.85rem;
        color: var(--text-secondary);
        text-decoration: line-through;
    }

    .savings-badge {
        display: inline-block;
        padding: 0.25rem 0.75rem;
        background: var(--success);
        color: white;
        border-radius: 20px;
        font-size: 0.75rem;
        font-weight: 600;
        margin-top: 0.5rem;
    }

    /* Scanner Modal */
    .scanner-modal {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: rgba(0, 0, 0, 0.9);
        z-index: 2000;
        display: flex;
        align-items: center;
        justify-content: center;
        opacity: 0;
        visibility: hidden;
        transition: all 0.3s;
    }

    .scanner-modal.active {
        opacity: 1;
        visibility: visible;
    }

    .scanner-content {
        background: var(--background);
        border-radius: 30px;
        width: 90%;
        max-width: 500px;
        overflow: hidden;
        transform: scale(0.8);
        transition: all 0.3s;
    }

    .scanner-modal.active .scanner-content {
        transform: scale(1);
    }

    .scanner-header {
        background: linear-gradient(135deg, var(--primary), var(--secondary));
        padding: 1.5rem;
        color: white;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .scanner-header h3 {
        font-size: 1.3rem;
    }

    .close-btn {
        background: none;
        border: none;
        color: white;
        font-size: 1.5rem;
        cursor: pointer;
        transition: transform 0.3s;
    }

    .close-btn:hover {
        transform: rotate(90deg);
    }

    .scanner-body {
        padding: 2rem;
        text-align: center;
    }

    .scanner-area {
        width: 250px;
        height: 250px;
        margin: 0 auto 2rem;
        border: 3px solid var(--accent);
        border-radius: 20px;
        position: relative;
        overflow: hidden;
        background: var(--primary);
    }

    .scanner-line {
        position: absolute;
        left: 10px;
        right: 10px;
        height: 4px;
        background: var(--accent);
        box-shadow: 0 0 20px var(--accent);
        animation: scan 2s ease-in-out infinite;
    }

    .scanner-icon {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        font-size: 5rem;
        color: rgba(255, 255, 255, 0.3);
        animation: pulse 2s ease-in-out infinite;
    }

    .scan-categories {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 1rem;
    }

    .scan-category {
        padding: 1rem;
        background: var(--card-bg);
        border-radius: 15px;
        cursor: pointer;
        transition: all 0.3s;
        border: 2px solid transparent;
    }

    .scan-category:hover, .scan-category.active {
        border-color: var(--accent);
        background: white;
    }

    .scan-category i {
        font-size: 1.5rem;
        color: var(--accent);
        margin-bottom: 0.5rem;
    }

    .scan-category span {
        display: block;
        font-size: 0.75rem;
        color: var(--text-secondary);
    }

    /* Nearby Shops */
    .nearby-shops {
        padding: 80px 2rem;
        background: var(--card-bg);
    }

    .shops-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
        gap: 2rem;
    }

    .shop-card {
        background: white;
        border-radius: 20px;
        padding: 1.5rem;
        border: 1px solid var(--border);
        transition: all 0.3s;
    }

    .shop-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
    }

    .shop-card-header {
        display: flex;
        gap: 1rem;
        margin-bottom: 1rem;
    }

    .shop-logo {
        width: 60px;
        height: 60px;
        background: linear-gradient(135deg, var(--accent), var(--accent-secondary));
        border-radius: 15px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-size: 1.5rem;
        font-weight: 700;
    }

    .shop-card-title h4 {
        font-size: 1.1rem;
        color: var(--primary);
        margin-bottom: 0.25rem;
    }

    .shop-card-title .distance {
        font-size: 0.85rem;
        color: var(--text-secondary);
    }

    .shop-rating {
        display: flex;
        gap: 0.25rem;
        margin-bottom: 1rem;
    }

    .shop-rating i {
        color: #FFD700;
        font-size: 0.9rem;
    }

    .shop-rating span {
        margin-left: 0.5rem;
        color: var(--text-secondary);
        font-size: 0.9rem;
    }

    .shop-details {
        display: flex;
        flex-direction: column;
        gap: 0.75rem;
        margin-bottom: 1rem;
    }

    .shop-detail {
        display: flex;
        align-items: center;
        gap: 0.75rem;
        font-size: 0.9rem;
        color: var(--text-secondary);
    }

    .shop-detail i {
        color: var(--accent);
        width: 20px;
    }

    .shop-card-footer {
        display: flex;
        gap: 1rem;
    }

    .shop-card-footer button {
        flex: 1;
        padding: 0.75rem;
        border-radius: 10px;
        font-family: 'Exo 2', sans-serif;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
    }

    .btn-contact {
        background: var(--accent);
        border: none;
        color: white;
    }

    .btn-contact:hover {
        background: var(--accent-secondary);
    }

    .btn-view {
        background: transparent;
        border: 2px solid var(--primary);
        color: var(--primary);
    }

    .btn-view:hover {
        background: var(--primary);
        color: white;
    }

    /* Footer */
    footer {
        background: var(--primary);
        color: white;
        padding: 60px 2rem 30px;
    }

    .footer-content {
        max-width: 1200px;
        margin: 0 auto;
        display: grid;
        grid-template-columns: 2fr 1fr 1fr 1fr;
        gap: 3rem;
    }

    .footer-brand .logo {
        margin-bottom: 1rem;
    }

    .footer-brand p {
        color: rgba(255, 255, 255, 0.7);
        line-height: 1.6;
        margin-bottom: 1.5rem;
    }

    .social-links {
        display: flex;
        gap: 1rem;
    }

    .social-links a {
        width: 40px;
        height: 40px;
        background: rgba(255, 255, 255, 0.1);
        border-radius: 10px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        transition: all 0.3s;
    }

    .social-links a:hover {
        background: var(--accent);
        transform: translateY(-3px);
    }

    .footer-links h4 {
        font-size: 1.1rem;
        margin-bottom: 1.5rem;
        color: white;
    }

    .footer-links ul {
        list-style: none;
    }

    .footer-links li {
        margin-bottom: 0.75rem;
    }

    .footer-links a {
        color: rgba(255, 255, 255, 0.7);
        text-decoration: none;
        transition: color 0.3s;
    }

    .footer-links a:hover {
        color: var(--accent);
    }

    .newsletter {
        display: flex;
        gap: 0.5rem;
    }

    .newsletter input {
        flex: 1;
        padding: 0.75rem 1rem;
        border: none;
        border-radius: 10px;
        font-family: 'Exo 2', sans-serif;
    }

    .newsletter button {
        padding: 0.75rem 1.25rem;
        background: var(--accent);
        border: none;
        border-radius: 10px;
        color: white;
        cursor: pointer;
        transition: all 0.3s;
    }

    .newsletter button:hover {
        background: var(--accent-secondary);
    }

    .footer-bottom {
        max-width: 1200px;
        margin: 40px auto 0;
        padding-top: 30px;
        border-top: 1px solid rgba(255, 255, 255, 0.1);
        text-align: center;
        color: rgba(255, 255, 255, 0.6);
        font-size: 0.9rem;
    }

    /* Mobile Responsive */
    @media (max-width: 1024px) {
        .features-grid {
            grid-template-columns: repeat(2, 1fr);
        }
        
        .footer-content {
            grid-template-columns: repeat(2, 1fr);
        }
    }

    @media (max-width: 768px) {
        .nav-links {
            display: none;
        }
        
        .mobile-menu-btn {
            display: block;
        }
        
        .hero h1 {
            font-size: 2.5rem;
        }
        
        .hero p {
            font-size: 1rem;
        }
        
        .search-container {
            flex-direction: column;
        }
        
        .cta-buttons {
            flex-direction: column;
            align-items: center;
        }
        
        .features-grid {
            grid-template-columns: 1fr;
        }
        
        .steps {
            grid-template-columns: 1fr;
            gap: 2rem;
        }
        
        .steps::before {
            display: none;
        }
        
        .section-header h2 {
            font-size: 1.8rem;
        }
        
        .price-grid {
            grid-template-columns: 1fr;
        }
        
        .shops-grid {
            grid-template-columns: 1fr;
        }
        
        .footer-content {
            grid-template-columns: 1fr;
            text-align: center;
        }
        
        .social-links {
            justify-content: center;
        }
        
        .scan-categories {
            grid-template-columns: repeat(2, 1fr);
        }
    }

    /* Mobile Menu */
    .mobile-menu {
        position: fixed;
        top: 0;
        right: -100%;
        width: 80%;
        max-width: 300px;
        height: 100vh;
        background: var(--primary);
        z-index: 1500;
        padding: 80px 2rem 2rem;
        transition: right 0.3s ease;
    }

    .mobile-menu.active {
        right: 0;
    }

    .mobile-menu-overlay {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: rgba(0, 0, 0, 0.5);
        z-index: 1400;
        opacity: 0;
        visibility: hidden;
        transition: all 0.3s;
    }

    .mobile-menu-overlay.active {
        opacity: 1;
        visibility: visible;
    }

    .mobile-menu ul {
        list-style: none;
    }

    .mobile-menu li {
        margin-bottom: 1.5rem;
    }

    .mobile-menu a {
        color: white;
        text-decoration: none;
        font-size: 1.2rem;
        font-weight: 500;
        transition: color 0.3s;
    }

    .mobile-menu a:hover {
        color: var(--accent);
    }
</style>
