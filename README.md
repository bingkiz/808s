/* 基础样式重置 */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    line-height: 1.6;
}

/* 导航栏样式 */
nav {
    background-color: #333;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: white;
    font-size: 1.5rem;
    font-weight: bold;
}

.nav-links {
    display: flex;
    list-style: none;
}

.nav-links li a {
    color: white;
    text-decoration: none;
    padding: 0.5rem 1rem;
}

.nav-links li a:hover {
    color: #ddd;
}

/* 首页英雄区域样式 */
.hero {
    height: 100vh;
    background-color: #f4f4f4;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 2rem;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

/* 章节通用样式 */
.section {
    padding: 5rem 2rem;
    max-width: 1200px;
    margin: 0 auto;
}

.section h2 {
    text-align: center;
    margin-bottom: 2rem;
}

/* 产品网格样式 */
.products-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    padding: 2rem 0;
}

.product-card {
    background: white;
    padding: 1rem;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    transition: transform 0.3s ease;
}

.product-card:hover {
    transform: translateY(-5px);
}

.product-card img {
    width: 100%;
    height: 300px; /* 固定高度 */
    object-fit: cover; /* 保持图片比例 */
    border-radius: 4px;
    margin-bottom: 1rem;
}

.product-card h3 {
    color: #333;
    margin: 0.5rem 0;
    font-size: 1.2rem;
}

.product-card p {
    color: #666;
    font-size: 0.9rem;
}

/* 联系方式样式 */
.contact-info {
    text-align: center;
}

.social-links {
    margin-top: 2rem;
}

.social-links a {
    margin: 0 1rem;
    color: #333;
    text-decoration: none;
}

/* 页脚样式 */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1rem;
    margin-top: 2rem;
}

/* 响应式设计 */
@media (max-width: 768px) {
    .nav-links {
        display: none; /* 在移动端需要添加汉堡菜单 */
    }
    
    .hero-content h1 {
        font-size: 2rem;
    }
} 
