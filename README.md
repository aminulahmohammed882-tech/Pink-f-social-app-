# Pink-f-social-app-
Good app that unit the world 🌎 together 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pink F Social App</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Arial, sans-serif;
        }
        
        body {
            background-color: #f0f2f5;
            color: #1c1e21;
            line-height: 1.6;
            padding: 60px 0;
            max-width: 100%;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 500px;
            margin: 0 auto;
            padding: 15px;
        }
        
        /* Header */
        .header {
            background-color: #ffffff;
            padding: 15px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            position: fixed;
            top: 0;
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 100;
        }
        
        .logo {
            width: 40px;
            height: 40px;
            background-color: #ff4081;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 20px;
            font-weight: bold;
        }
        
        .app-name {
            color: #ff4081;
            font-size: 20px;
            font-weight: bold;
        }
        
        .header-icons {
            display: flex;
            gap: 15px;
        }
        
        /* Instructions */
        .instructions {
            background: white;
            padding: 20px;
            border-radius: 10px;
            margin-bottom: 20px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .instructions h3 {
            color: #ff4081;
            margin-bottom: 15px;
            text-align: center;
        }
        
        .steps {
            padding-left: 20px;
            margin-bottom: 15px;
        }
        
        .steps li {
            margin-bottom: 10px;
        }
        
        .note {
            background: #f0f2f5;
            padding: 12px;
            border-radius: 8px;
            font-size: 14px;
            margin-top: 15px;
        }
        
        .button {
            display: block;
            background: #ff4081;
            color: white;
            text-align: center;
            padding: 12px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 15px;
        }
        
        /* Create Post */
        .create-post {
            background-color: #ffffff;
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 15px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .post-input {
            display: flex;
            align-items: center;
            gap: 10px;
            padding-bottom: 15px;
            border-bottom: 1px solid #e4e6eb;
        }
        
        .user-image {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: linear-gradient(45deg, #ff9a9e, #fad0c4);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
        }
        
        .post-input input {
            flex: 1;
            padding: 12px 15px;
            border-radius: 20px;
            border: none;
            background-color: #f0f2f5;
            font-size: 16px;
        }
        
        .post-actions {
            display: flex;
            justify-content: space-around;
            margin-top: 15px;
        }
        
        .post-action {
            display: flex;
            align-items: center;
            gap: 5px;
            padding: 8px;
            color: #65676b;
        }
        
        /* News Feed */
        .news-feed {
            background-color: #ffffff;
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 15px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
        }
        
        .post-header {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 15px;
        }
        
        .post-info h3 {
            font-size: 16px;
        }
        
        .post-info span {
            font-size: 12px;
            color: #65676b;
        }
        
        .post-content {
            margin-bottom: 15px;
        }
        
        .post-content p {
            margin-bottom: 10px;
        }
        
        .post-image {
            width: 100%;
            height: 200px;
            background: linear-gradient(45deg, #ff9a9e, #fad0c4);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            margin-top: 10px;
        }
        
        .post-stats {
            display: flex;
            justify-content: space-between;
            padding: 10px 0;
            border-bottom: 1px solid #e4e6eb;
            margin-bottom: 10px;
            font-size: 14px;
            color: #65676b;
        }
        
        .post-buttons {
            display: flex;
            justify-content: space-around;
        }
        
        .post-button {
            display: flex;
            align-items: center;
            gap: 5px;
            padding: 8px;
            color: #65676b;
        }
        
        /* Bottom Navigation */
        .bottom-nav {
            position: fixed;
            bottom: 0;
            width: 100%;
            background: #fff;
            display: flex;
            justify-content: space-around;
            padding: 12px;
            border-top: 1px solid #ddd;
        }
        
        .nav-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            color: #65676b;
            font-size: 12px;
        }
        
        .nav-item.active {
            color: #ff4081;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <div class="header">
        <div class="logo">f</div>
        <div class="app-name">PinkF Social</div>
        <div class="header-icons">
            <span>🔍</span>
            <span>💬</span>
        </div>
    </div>

    <div class="container">
        <div class="instructions">
            <h3>How to Save This App</h3>
            <ol class="steps">
                <li>Tap & hold on the code to select all</li>
                <li>Copy the entire code</li>
                <li>Open a notes app and paste</li>
                <li>Save the note as "pinkf.html"</li>
                <li>Use an HTML viewer app to open it</li>
            </ol>
            <div class="note">
                <strong>Quick Method:</strong> Copy the code and paste into an online HTML editor like https://html-online.com
            </div>
            <a href="https://play.google.com/store/search?q=html%20viewer&c=apps" class="button">Get HTML Viewer App</a>
        </div>
        
        <!-- Create Post -->
        <div class="create-post">
            <div class="post-input">
                <div class="user-image">J</div>
                <input type="text" placeholder="What's on your mind?">
            </div>
            <div class="post-actions">
                <div class="post-action">
                    <span style="color: #f3425f;">📹</span>
                    <span>Live Video</span>
                </div>
                <div class="post-action">
                    <span style="color: #45bd62;">🖼️</span>
                    <span>Photo/Video</span>
                </div>
                <div class="post-action">
                    <span style="color: #f7b928;">😊</span>
                    <span>Feeling/Activity</span>
                </div>
            </div>
        </div>

        <!-- News Feed -->
        <div class="news-feed">
            <div class="post-header">
                <div class="user-image">S</div>
                <div class="post-info">
                    <h3>Sarah Johnson</h3>
                    <span>Yesterday at 3:45 PM · 🌎</span>
                </div>
            </div>
            <div class="post-content">
                <p>Just finished my morning hike! The view was absolutely breathtaking today. 🏞️</p>
                <div class="post-image">Mountain View</div>
            </div>
            <div class="post-stats">
                <div class="likes">👍 245</div>
                <div class="comments-shares">48 comments · 12 shares</div>
            </div>
            <div class="post-buttons">
                <div class="post-button">👍 Like</div>
                <div class="post-button">💬 Comment</div>
                <div class="post-button">↗️ Share</div>
            </div>
        </div>

        <!-- Post 2 -->
        <div class="news-feed">
            <div class="post-header">
                <div class="user-image">M</div>
                <div class="post-info">
                    <h3>Michael Thompson</h3>
                    <span>Today at 10:15 AM · 🌎</span>
                </div>
            </div>
            <div class="post-content">
                <p>Check out this amazing recipe I tried last night! Perfect for dinner parties.</p>
                <div class="post-image">Food Photo</div>
            </div>
            <div class="post-stats">
                <div class="likes">👍 189</div>
                <div class="comments-shares">32 comments · 5 shares</div>
            </div>
            <div class="post-buttons">
                <div class="post-button">👍 Like</div>
                <div class="post-button">💬 Comment</div>
                <div class="post-button">↗️ Share</div>
            </div>
        </div>
    </div>

    <!-- Bottom Navigation -->
    <div class="bottom-nav">
        <div class="nav-item active">
            <span>🏠</span>
            <span>Home</span>
        </div>
        <div class="nav-item">
            <span>👥</span>
            <span>Friends</span>
        </div>
        <div class="nav-item">
            <span>📺</span>
            <span>Watch</span>
        </div>
        <div class="nav-item">
            <span>🔔</span>
            <span>Notifications</span>
        </div>
        <div class="nav-item">
            <span>☰</span>
            <span>Menu</span>
        </div>
    </div>

    <script>
        // Simple interaction for demonstration
        document.addEventListener('DOMContentLoaded', function() {
            // Like button functionality
            const likeButtons = document.querySelectorAll('.post-button');
            likeButtons.forEach(button => {
                button.addEventListener('click', function() {
                    if (this.innerHTML.includes('Like')) {
                        this.innerHTML = '👍 Liked';
                        this.style.color = '#ff4081';
                    } else if (this.innerHTML.includes('Liked')) {
                        this.innerHTML = '👍 Like';
                        this.style.color = '#65676b';
                    }
                });
            });
            
            // Bottom nav interaction
            const navItems = document.querySelectorAll('.nav-item');
            navItems.forEach(item => {
                item.addEventListener('click', function() {
                    navItems.forEach(i => i.classList.remove('active'));
                    this.classList.add('active');
                });
            });
            
            // Post input focus
            const postInput = document.querySelector('.post-input input');
            postInput.addEventListener('focus', function() {
                alert("In a real app, this would open a full post creation screen!");
            });
        });
    </script>
</body>
</html>
