# Animepfp-2
/* Google Fonts Import */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    background-color: #f7f9fc;
    color: #333;
}

/* Header & Navbar styling */
header {
    background-color: #1a1a2e;
    color: white;
    padding: 15px 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 4px 10px rgba(0,0,0,0.1);
}

.navbarContainer {
    width: 85%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 24px;
    font-weight: 700;
    color: #fff;
    text-decoration: none;
    text-transform: uppercase;
}

.logo span {
    color: #e94560;
}

.nav-links {
    list-style: none;
    display: flex;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    color: #e0e0e0;
    text-decoration: none;
    font-weight: 500;
    transition: 0.3s;
}

.nav-links a:hover, .nav-links a.active {
    color: #e94560;
}

.search-box {
    display: flex;
    align-items: center;
    background: #16213e;
    padding: 6px 12px;
    border-radius: 20px;
}

.search-box input {
    background: none;
    border: none;
    outline: none;
    color: white;
    padding-right: 5px;
}

.search-box i {
    color: #e94560;
    cursor: pointer;
}

/* Layout Structure */
.main-container {
    width: 85%;
    margin: 40px auto;
    display: grid;
    grid-template-columns: 70% 28%;
    gap: 2%;
}

/* Blog Cards Section */
.blog-posts h2 {
    margin-bottom: 20px;
    font-size: 28px;
    color: #1a1a2e;
}

.posts-grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 30px;
}

.post-card {
    background: white;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    display: flex;
    transition: transform 0.3s;
}

.post-card:hover {
    transform: translateY(-5px);
}

.post-img {
    position: relative;
    width: 40%;
    min-height: 200px;
}

.post-img img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.category-tag {
    position: absolute;
    top: 10px;
    left: 10px;
    background: #e94560;
    color: white;
    padding: 4px 10px;
    font-size: 12px;
    border-radius: 4px;
    font-weight: 600;
}

.post-content {
    padding: 20px;
    width: 60%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.post-content h3 {
    font-size: 20px;
    color: #1a1a2e;
    margin-bottom: 10px;
}

.post-content p {
    color: #666;
    font-size: 14px;
    line-height: 1.6;
    margin-bottom: 15px;
}

.post-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.post-footer .date {
    font-size: 13px;
    color: #999;
}

.read-btn {
    color: #e94560;
    text-decoration: none;
    font-weight: 600;
    font-size: 14px;
    transition: 0.2s;
}

.read-btn:hover {
    letter-spacing: 0.5px;
}

/* Sidebar Widgets */
.sidebar .widget {
    background: white;
    padding: 20px;
    border-radius: 12px;
    margin-bottom: 30px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
}

.widget h3 {
    border-bottom: 2px solid #e94560;
    padding-bottom: 8px;
    margin-bottom: 15px;
    font-size: 18px;
    color: #1a1a2e;
}

.widget p {
    font-size: 14px;
    color: #666;
    line-height: 1.6;
}

.category-widget ul {
    list-style: none;
}

.category-widget ul li {
    margin-bottom: 10px;
}

.category-widget ul li a {
    text-decoration: none;
    color: #444;
    font-size: 14px;
    display: flex;
    justify-content: space-between;
    transition: 0.2s;
}

.category-widget ul li a:hover {
    color: #e94560;
    padding-left: 5px;
}

/* Footer */
footer {
    background: #1a1a2e;
    color: #a0a0a0;
    text-align: center;
    padding: 20px 0;
    margin-top: 40px;
    font-size: 14px;
}

/* Responsive Design for Mobile Devices */
@media (max-width: 900px) {
    .main-container {
        grid-template-columns: 1fr;
    }
    .post-card {
        flex-direction: column;
    }
    .post-img {
        width: 100%;
        height: 200px;
    }
    .post-content {
        width: 100%;
    }
    .navbarContainer {
        flex-direction: column;
        gap: 15px;
    }
}
