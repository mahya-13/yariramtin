<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رامتین محمدیاری</title>
    <style>
        body {
            font-family: Tahoma, sans-serif;
            background-color: #fff0f5; /* رنگ صورتی خیلی ملایم */
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden; /* برای اینکه قلب‌ها از صفحه بیرون نزنند */
        }
        .profile-card {
            background: white;
            padding: 30px;
            border: 2px solid #ffb6c1;
            border-radius: 20px;
            text-align: center;
            width: 90%;
            max-width: 350px;
            z-index: 10; /* برای اینکه کارت روی قلب‌ها باشد */
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        h1 { font-size: 22px; color: #d63384; }
        p { font-size: 14px; color: #666; }
        .info-list { text-align: right; display: inline-block; width: 100%; }
        .info-item {
            font-size: 14px;
            margin: 10px 0;
            padding: 8px;
            background: #fff5f7;
            border-radius: 8px;
        }
        
        /* استایل دکمه قلب */
        .heart-button {
            background: #ff4d6d;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 25px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 15px;
            transition: transform 0.2s;
        }
        .heart-button:active { transform: scale(0.9); }

        /* استایل قلب‌های پرنده */
        .floating-heart {
            position: absolute;
            color: #ff4d6d;
            font-size: 20px;
            user-select: none;
            pointer-events: none;
            animation: growAndFade 3s forwards;
            z-index: 1;
        }

        @keyframes growAndFade {
            0% { transform: scale(0.5); opacity: 1; }
            100% { transform: scale(5); opacity: 0; }
        }

        .footer { margin-top: 20px; font-size: 12px; color: #aaa; }
    </style>
</head>
<body>

    <div class="profile-card">
        <h1>رامتین محمدیاری</h1>
        <p>رامتین محمدیاری بابای خوشگل و جذاب من انشالله 120 سال زنده باشه</p>

        <div class="info-list">
            <div class="info-item">✨ مهارت: تربیت به درستی</div>
            <div class="info-item">💖 معشوقه: فاطمه السادات محسنی</div>
            <div class="info-item">⚠️ عامل اذیت: محیا محمدیاری</div>
        </div>

        <!-- دکمه جادویی -->
        <button class="heart-button" onclick="createHeart()">روی من کلیک کن ❤️</button>

        <div class="footer">کد نویسی با عشق ✨</div>
    </div>

    <script>
        function createHeart() {
            // ساختن یک المنت قلب
            const heart = document.createElement('div');
            heart.classList.add('floating-heart');
            heart.innerHTML = '❤️';
            
            // تعیین موقعیت تصادفی قلب در صفحه
            const x = Math.random() * window.innerWidth;
            const y = Math.random() * window.innerHeight;
            
            heart.style.left = x + 'px';
            heart.style.top = y + 'px';
            
            // اضافه کردن قلب به صفحه
            document.body.appendChild(heart);
            
            // پاک کردن قلب از حافظه بعد از اتمام انیمیشن
            setTimeout(() => {
                heart.remove();
            }, 3000);
        }
    </script>

</body>
</html>
