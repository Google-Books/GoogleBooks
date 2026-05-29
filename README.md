                                                                                                         <!DOCTYPE html>

<html lang="fa" dir="rtl">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Google Books - Premium Portal</title>

    <style>

        :root {

            --tg-dark-bg: #17212b;

            --laser-blue: #00f0ff;

            --laser-glow: rgba(0, 240, 255, 0.45);

            --btn-blue: #2481cc;

            --btn-shadow: rgba(11, 44, 71, 0.95);

            --card-radius: 35px;

            --transition-smooth: all 0.5s cubic-bezier(0.16, 1, 0.3, 1);

        }

        * { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Segoe UI', system-ui, -apple-system, sans-serif; }

        body { background-color: var(--tg-dark-bg); color: #ffffff; display: flex; flex-direction: column; align-items: center; justify-content: flex-start; min-height: 100vh; padding: 160px 24px 60px 24px; position: relative; overflow-x: hidden; -webkit-font-smoothing: antialiased; }

        .telegram-btn { position: fixed; top: 30px; left: 50%; transform: translateX(-50%); z-index: 10000; background: linear-gradient(135deg, #00f0ff, #0066ff); color: #ffffff; text-decoration: none; padding: 13px 38px; border-radius: 20px; font-size: 15px; font-weight: 700; display: flex; align-items: center; justify-content: center; gap: 12px; border: 1px solid rgba(255, 255, 255, 0.25); box-shadow: 0 8px 25px var(--laser-glow), inset 0 1px 2px rgba(255, 255, 255, 0.4); transition: var(--transition-smooth); white-space: nowrap; }

        .telegram-btn:hover { transform: translateX(-50%) translateY(-3px); box-shadow: 0 12px 35px rgba(0, 240, 255, 0.7); filter: brightness(1.1); }

        .telegram-icon { width: 22px; height: 22px; fill: #ffffff; transition: var(--transition-smooth); }

        .telegram-btn:hover .telegram-icon { transform: scale(1.1); }

        .main-title { font-size: 3rem; font-weight: 900; text-align: center; margin-bottom: 70px; line-height: 1.2; letter-spacing: -1px; background: linear-gradient(180deg, #ffffff 0%, #b0c4de 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; text-shadow: 0 4px 20px rgba(0, 0, 0, 0.5); }

        .cards-container { display: grid; grid-template-columns: repeat(3, minmax(260px, 340px)); gap: 50px; width: 100%; max-width: 1200px; justify-content: center; }

        .card-wrapper { display: flex; flex-direction: column; align-items: center; width: 100%; background: rgba(255, 255, 255, 0.03); border: 1px solid rgba(255, 255, 255, 0.06); padding: 22px; border-radius: calc(var(--card-radius) + 10px); box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3); transition: var(--transition-smooth); }

        .card-wrapper:hover { transform: translateY(-8px); background: rgba(255, 255, 255, 0.05); border-color: rgba(255, 255, 255, 0.12); box-shadow: 0 25px 50px rgba(0, 0, 0, 0.5); }

        .card-img-box { width: 100%; aspect-ratio: 1 / 1; background-color: #ffffff; border-radius: var(--card-radius); padding: 20px; display: flex; align-items: center; justify-content: center; margin-bottom: 22px; box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3); transition: var(--transition-smooth); }

        .card-img { max-width: 100%; max-height: 100%; object-fit: contain; transition: var(--transition-smooth); }

        .card-wrapper:hover .card-img { transform: scale(1.05); }

        .card-btn { width: 100%; background-color: var(--btn-blue); color: #ffffff; text-decoration: none; text-align: center; padding: 14px 20px; border-radius: 16px; font-size: 15px; font-weight: 600; box-shadow: 0 10px 22px var(--btn-shadow); border: 1px solid rgba(255, 255, 255, 0.08); transition: var(--transition-smooth); }

        .card-btn:hover { background-color: #2b96eb; box-shadow: 0 12px 28px rgba(36, 129, 204, 0.5); transform: translateY(-1px); }

        .attribution { display: none; }

        @media (max-width: 950px) { .cards-container { grid-template-columns: repeat(2, minmax(240px, 320px)); gap: 40px; } .main-title { font-size: 2.5rem; } }

        @media (max-width: 600px) {

            body { padding-top: 130px; padding-left: 12px; padding-right: 12px; }

.main-title { font-size: 1.8rem; margin-bottom: 45px; }

            .cards-container { grid-template-columns: repeat(2, 1fr); gap: 12px; }

            .card-wrapper { padding: 10px; border-radius: 25px; }

            .card-img-box { border-radius: 20px; padding: 10px; margin-bottom: 12px; }

            .card-btn { font-size: 11px; padding: 11px 4px; border-radius: 12px; box-shadow: 0 6px 14px var(--btn-shadow); }

            .telegram-btn { padding: 11px 24px; font-size: 13px; top: 20px; border-radius: 14px; box-shadow: 0 6px 18px var(--laser-glow); }

        }

    </style>

</head>

<body>



    <!-- دکمه شناور تلگرام متصل به لینک درخواستی شما -->

    <a href="https://books-photoes.webflow.io/old-home" class="telegram-btn">

        <span>Our Telegram channels</span>

        <!-- آیکون رسمی، ترمیم‌شده و کاملاً متقارن هواپیمای کاغذی تلگرام از Flaticon -->

        <svg class="telegram-icon" viewBox="0 0 24 24">

            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8c-.15 1.58-.8 5.42-1.13 7.19-.14.75-.42 1-.68 1.03-.58.05-1.02-.38-1.58-.75-.88-.58-1.38-.94-2.23-1.5-1-.65-.35-1.01.22-1.59.15-.15 2.71-2.48 2.76-2.69.01-.03.01-.14-.07-.2-.08-.06-.19-.04-.27-.02-.11.02-1.93 1.23-5.46 3.62-.51.35-.98.52-1.4.51-.46-.01-1.35-.26-2.01-.48-.81-.27-1.46-.42-1.4-.88.03-.24.38-.49 1.04-.74 4.07-1.77 6.79-2.94 8.15-3.5 3.89-1.61 4.7-1.89 5.23-1.9.11 0 .37.03.54.17.14.12.18.28.2.45-.02.07-.02.13-.03.2z"/>

        </svg>

    </a>



    <h1 class="main-title">Welcome To<br>Google Books!</h1>



    <div class="cards-container">

        <!-- کارت اول: کتاب‌های رایگان (با لینک تصویر کاملاً سالم و فیکس‌شده) -->

        <div class="card-wrapper">

            <div class="card-img-box">

                <img src="https://trilliardaire.sirv.com/FreeBooks.png" alt="Free Books" class="card-img" crossorigin="anonymous">

            </div>

            <a href="#" class="card-btn">Free Books</a>

        </div>



        <!-- کارت دوم: کتاب‌های صوتی رایگان (با لینک تصویر کاملاً بازسازی شده و بدون کوتاه‌شدگی) -->

        <div class="card-wrapper">

            <div class="card-img-box">

                <img src="https://trilliardaire.sirv.com/%DA%A9%D8%AA%D8%A7%D8%A8%20%D9%87%D8%A7%DB%8C%20%DA%AF%D9%88%DA%AF%D9%84/audio.avif" alt="Free Audio Books" class="card-img" crossorigin="anonymous">

            </div>

            <a href="https://audiobookbay.lu" target="_blank" class="card-btn">Free Audio Books</a>

        </div>



        <!-- کارت سوم: بهترین کتاب‌های سال ۲۰۲۶ (با لینک تصویر کاملاً بازسازی شده و بدون کوتاه‌شدگی) -->

        <div class="card-wrapper">

            <div class="card-img-box">

                <img src="https://trilliardaire.sirv.com/%DA%A9%D8%AA%D8%A7%D8%A8%20%D9%87%D8%A7%DB%8C%20%DA%AF%D9%88%DA%AF%D9%84/b_best%202026.avif" alt="The Best Books of 2026" class="card-img" crossorigin="anonymous">

            </div>

            <a href="https://books-photoes.webflow.io/" class="card-btn">The Best Books of 2026</a>

        </div>

    </div>



<!-- خط کپی‌رایت فلات‌آیکون درخواستی شما -->

    <div class="attribution">

        <a href="https://www.flaticon.com/free-icons/telegram" title="telegram icons">Telegram icons created by See Icons - Flaticon</a>

    </div>



    <!-- Social Bar Ad -->

    <script src="https://speedingdeadlyplays.com/b3/e9/4d/b3e94d023432c8cb40b981d7804166a2.js"></script>



</body>

</html>



    <!-- خط کپی‌رایت فلات‌آیکون درخواستی شما -->

    <div class="attribution">

        <a href="https://www.flaticon.com/free-icons/telegram" title="telegram icons">Telegram icons created by See Icons - Flaticon</a>

    </div>



</body>

</html>
