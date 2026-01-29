<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="Abdulazizov Abdukarim" content="width=device-width, initial-scale=1.0">
    <title>my profile | @Abdulazizov Abdukarim</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* GitHub Dark Mode Color Palette */
        :root {
            --gh-bg: #0d1117;
            --gh-card: #161b22;
            --gh-border: #30363d;
            --gh-text: #c9d1d9;
            --gh-gray: #8b949e;
            --gh-green: #238636;
            --gh-green-hover: #2ea043;
            --gh-link: #58a6ff;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            background-color: var(--gh-bg);
            color: var(--gh-text);
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
            padding: 40px 20px;
            line-height: 1.5;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 280px 1fr;
            gap: 30px;
        }

        /* 1. LEFT COLUMN: PROFILE INFO */
        .sidebar { text-align: left; }

        .avatar-container {
            position: relative;
            margin-bottom: 20px;
        }

        .avatar {
            width: 100%;
            border-radius: 50%;
            border: 1px solid var(--gh-border);
        }

        .status-badge {
            position: absolute;
            bottom: 30px;
            right: 0;
            background: var(--gh-card);
            border: 1px solid var(--gh-border);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 12px;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .status-dot {
            width: 8px;
            height: 8px;
            background: var(--gh-green);
            border-radius: 50%;
        }

        h1 { font-size: 26px; font-weight: 600; margin-top: 10px; color: white; }
        .username { font-size: 20px; color: var(--gh-gray); font-weight: 300; margin-bottom: 20px; }
        .bio { font-size: 16px; margin-bottom: 20px; }

        .edit-btn {
            display: block;
            width: 100%;
            padding: 8px;
            background: var(--gh-card);
            border: 1px solid var(--gh-border);
            color: var(--gh-text);
            border-radius: 6px;
            text-align: center;
            text-decoration: none;
            font-size: 14px;
            font-weight: 500;
            margin-bottom: 20px;
        }

        .edit-btn:hover { background: #30363d; border-color: #8b949e; }

        /* 2. RIGHT COLUMN: ACCOUNTS GRID */
        .main-content { padding-top: 20px; }

        .nav-tabs {
            display: flex;
            gap: 20px;
            border-bottom: 1px solid var(--gh-border);
            margin-bottom: 20px;
            padding-bottom: 10px;
        }

        .tab { font-size: 14px; color: var(--gh-text); text-decoration: none; display: flex; align-items: center; gap: 8px; }
        .tab.active { font-weight: 600; border-bottom: 2px solid #f78166; padding-bottom: 12px; margin-bottom: -12px; }

        .accounts-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 16px;
        }

        .account-card {
            background: var(--gh-card);
            border: 1px solid var(--gh-border);
            border-radius: 6px;
            padding: 16px;
            text-decoration: none;
            color: var(--gh-text);
            transition: 0.2s;
        }

        .account-card:hover { border-color: var(--gh-gray); }

        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 8px;
        }

        .card-title { color: var(--gh-link); font-weight: 600; font-size: 14px; }
        .public-badge {
            font-size: 12px;
            color: var(--gh-gray);
            border: 1px solid var(--gh-border);
            padding: 2px 8px;
            border-radius: 12px;
        }

        .card-desc { font-size: 12px; color: var(--gh-gray); margin-bottom: 12px; }

        .card-footer { font-size: 12px; display: flex; align-items: center; gap: 15px; color: var(--gh-gray); }
        .lang-dot { width: 12px; height: 12px; border-radius: 50%; }

        /* Contribution Graph Mockup */
        .contribution-box {
            margin-top: 30px;
            border: 1px solid var(--gh-border);
            border-radius: 6px;
            padding: 20px;
        }

        .graph-title { font-size: 14px; margin-bottom: 10px; }
        .graph-cells { display: flex; gap: 3px; }
        .cell { width: 11px; height: 11px; border-radius: 2px; background: #161b22; border: 1px solid rgba(27,31,35,0.06); }
        .cell.low { background: #0e4429; }
        .cell.mid { background: #006d32; }
        .cell.high { background: #26a641; }
        .cell.ultra { background: #39d353; }

        /* Responsive */
        @media (max-width: 768px) {
            .container { grid-template-columns: 1fr; }
            .sidebar { text-align: center; }
            .accounts-grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="sidebar">
            <div class="avatar-container">
                <img src="https://github.com/identicons/jasonlong.png" alt="Avatar" class="avatar">
                <div class="status-badge">
                    <div class="status-dot"></div>
                    <span>Focusing</span>
                </div>
            </div>
            <h1>Abdulazizov Abdukarim</h1>
            <div class="username">kali.linux_404</div>
            <div class="bio">python,kali linux,deux,jv,css,hacker🚀</div>

            <a href="#" class="edit-btn">sudo access --root</a>

            <div style="font-size: 14px; color: var(--gh-text);">
                <p style="margin-bottom: 8px;"><i class="fas fa-map-marker-alt" style="width: 20px;"></i> Tashkent, Uzbekistan</p>
                <p style="margin-bottom: 8px;"><i class="fas fa-link" style="width: 20px;"></i> <a href="https://www.instagram.com/kali.linux_404?igsh=N3owbjFmY2w5dWJz&utm_source=qr" style="color: var(--gh-text); text-decoration: none;">portfolio.me</a></p>
                <p style="margin-bottom: 8px;"><i class="fab fa-twitter" style="width: 20px;"></i> @kali.linux_404</p>
            </div>
        </div>

        <div class="main-content">
            <div class="nav-tabs">
                <a href="#" class="tab active"><i class="fas fa-book-open"></i> ~/root</a>
                <a href="#" class="tab"><i class="fas fa-code-branch"></i> get_accesss</a>
                <a href="#" class="tab"><i class="fas fa-star"></i> Stars</a>
            </div>

            <p style="font-size: 14px; margin-bottom: 15px;">Active Sessions</p>

            <div class="accounts-grid">
                <a href="https://t.me/abdukarim_704" class="account-card">
                    <div class="card-header">
                        <span class="card-title">Telegram</span>
                        <span class="public-badge">Public</span>
                    </div>
                    <p class="card-desc">Telegram.com</p>
                    <div class="card-footer">
                        <span class="lang-dot" style="background: #0088cc;"></span> Telegram
                        <span><i class="far fa-star"></i> 124</span>
                    </div>
                </a>

                <a href="https://instagram.com/username" class="account-card">
                    <div class="card-header">
                        <span class="card-title">Insta_Portfolio</span>
                        <span class="public-badge">Public</span>
                    </div>
                    <p class="card-desc">Instagram.com</p>
                    <div class="card-footer">
                        <span class="lang-dot" style="background: #e1306c;"></span> Instagram
                        <span><i class="far fa-star"></i> 89</span>
                    </div>
                </a>

                <a href="tel:+998 904022888" class="account-card">
                    <div class="card-header">
                        <span class="card-title">Phon number</span>
                        <span class="public-badge">Public</span>
                    </div>
                    <p class="card-desc">phone number +998904022888</p>
                    <div class="card-footer">
                        <span class="lang-dot" style="background: #2ecc71;"></span> Phone
                        <span><i class="fas fa-shield-alt"></i> Verified</span>
                    </div>
                </a>

                <a href="https://facebook.com/username" class="account-card">
                    <div class="card-header">
                        <span class="card-title">Facebook</span>
                        <span class="public-badge">Public</span>
                    </div>
                    <p class="card-desc">facebook.com</p>
                    <div class="card-footer">
                        <span class="https://www.facebook.com/usman.kurbanaliev" style="background: #1877f2;"></span> Facebook
                        <span><i class="far fa-star"></i> 45</span>
                    </div>
                </a>
            </div>

            <div class="contribution-box">
                <p class="graph-title">4,234 contributions in the last year</p>
                <div class="graph-cells" id="graph">
                    </div>
            </div>
        </div>
    </div>

    <script>
        // GitHub "yashil kvadratlar" grafigini yaratish
        const graph = document.getElementById('graph');
        for (let i = 0; i < 50; i++) {
            const cell = document.createElement('div');
            cell.className = 'cell';
            const rand = Math.random();
            if (rand > 0.8) cell.classList.add('ultra');
            else if (rand > 0.6) cell.classList.add('high');
            else if (rand > 0.4) cell.classList.add('mid');
            else if (rand > 0.2) cell.classList.add('low');
            graph.appendChild(cell);
        }
    </script>

</body>
</html>

