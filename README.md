<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ZENTRIXA | Master Words. Master the World.</title>
    <meta name="description"
        content="ZENTRIXA - AI-powered English vocabulary learning platform. O'zbekcha-inglizcha lug'at, 15 ta test savollari, A1 dan C1 dagacha 5 ta darajalar. IELTS so'zlar generatsiyasi va AI Teacher integratsiyasi.">
    <meta name="keywords"
        content="english vocabulary, английский язык, узбекский, learn english, lug'at, test, A1, A2, B1, B2, C1, ZENTRIXA, o'zbekcha-inglizcha lug'at, test, A1 dan C1 dagacha 5 ta darajalar. IELTS so'zlar generatsiyasi va AI Teacher integratsiyasi. xatolarni to'g'irla qilindi.">
    <meta name="author" content="ZENTRIXA">
    <meta name="robots" content="index, follow">

    <!-- Open Graph Tags -->
    <meta property="og:title" content="ZENTRIXA | Master Words. Master the World.">
    <meta property="og:description"
        content="AI-powered English vocabulary learning platform with interactive quizzes and flashcards for all levels">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://www.zentrixa.com">
    <meta property="og:image" content="https://www.zentrixa.com/images/og-image.jpg">

    <!-- Twitter Card Tags -->
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:title" content="ZENTRIXA | Master Words. Master the World.">
    <meta name="twitter:description"
        content="Learn English vocabulary with AI-powered quizzes and interactive flashcards">
    <meta name="twitter:image" content="https://www.zentrixa.com/images/twitter-image.jpg">

    <!-- Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag() { dataLayer.push(arguments); }
        gtag('js', new Date());
        gtag('config', 'GA_MEASUREMENT_ID');
    </script>

    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background: #0B1120;
            color: white;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 50px;
            background: #111827;
        }

        .navbar nav {
            display: flex;
            gap: 20px;
            align-items: center;
            justify-content: center;
            flex: 1;
        }

        .logo {
            color: #06B6D4;
        }

        nav a {
            color: white;
            text-decoration: none;
            cursor: pointer;
            font-size: 1.1em;
            padding: 10px 20px;
            border-radius: 8px;
            transition: all 0.3s ease;
            background: linear-gradient(135deg, #1E293B 0%, #475569 100%);
            font-weight: 500;
            box-shadow: 0 4px 10px rgba(6, 182, 212, 0.2);
        }

        nav a:hover {
            background: linear-gradient(135deg, #06B6D4 0%, #0891b2 100%);
            color: white !important;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(6, 182, 212, 0.5);
        }

        .test-link {
            background: linear-gradient(135deg, #2563EB 0%, #06B6D4 100%) !important;
            color: white !important;
            font-weight: bold;
            box-shadow: 0 4px 15px rgba(6, 182, 212, 0.4) !important;
            position: relative;
            z-index: 10;
        }

        .test-link:hover {
            background: linear-gradient(135deg, #1d4ed8 0%, #0891b2 100%) !important;
            box-shadow: 0 6px 25px rgba(6, 182, 212, 0.8) !important;
            transform: translateY(-3px) scale(1.05);
        }

        @keyframes pulse {
            0%,
            100% {
                box-shadow: 0 4px 15px rgba(6, 182, 212, 0.4);
            }
            50% {
                box-shadow: 0 6px 25px rgba(6, 182, 212, 0.8);
            }
        }

        .hero {
            height: 200px;
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("images/quiz-banner.jpg");
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 28px;
            font-weight: bold;
            border-radius: 15px;
            margin-bottom: 20px;
        }

        .hero h2 {
            font-size: 24px;
            margin: 0;
            margin-bottom: 8px;
        }

        .hero p {
            font-size: 12px;
            font-weight: normal;
            margin: 0;
            margin-bottom: 15px;
        }

        .hero button {
            padding: 8px 18px;
            font-size: 13px;
            background: #2563EB;
            border: none;
            color: white;
            border-radius: 8px;
            cursor: pointer;
        }

        .auth-section {
            display: flex;
            justify-content: center;
            padding: 60px 20px;
        }

        .auth-container {
            background: #1E293B;
            padding: 40px;
            border-radius: 12px;
            width: 350px;
        }

        .auth-container input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: none;
            border-radius: 6px;
            box-sizing: border-box;
        }

        .auth-container button {
            width: 100%;
            padding: 10px;
            background: #06B6D4;
            border: none;
            border-radius: 6px;
            color: white;
            cursor: pointer;
            font-size: 1em;
        }

        .auth-container button:hover {
            background: #0891b2;
        }

        .auth-container span {
            color: #06B6D4;
            cursor: pointer;
        }

        /* Vocabulary Styles */
        .vocab-section {
            padding: 50px 20px;
            background: #0B1120;
            display: none;
        }

        .vocab-container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .vocab-container h2 {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 40px;
            color: #06B6D4;
        }

        .level-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .level-btn {
            padding: 12px 25px;
            background: #1E293B;
            border: 2px solid #475569;
            color: white;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1em;
            transition: all 0.3s ease;
        }

        .level-btn:hover {
            background: #2563EB;
            border-color: #2563EB;
        }

        .level-btn.active {
            background: #06B6D4;
            border-color: #06B6D4;
        }

        .words-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }

        .word-card {
            background: #1E293B;
            padding: 25px;
            border-radius: 12px;
            border-left: 4px solid #06B6D4;
            cursor: pointer;
            transition: all 0.3s ease;
            min-height: 150px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }

        .word-card:hover {
            background: #2D3E50;
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(6, 182, 212, 0.2);
        }

        .word-card.flipped {
            background: linear-gradient(135deg, #2563EB 0%, #06B6D4 100%);
        }

        .word-uz {
            font-size: 1.8em;
            font-weight: bold;
            margin-bottom: 10px;
            color: #06B6D4;
        }

        .word-en {
            font-size: 1.2em;
            color: #94A3B8;
            display: none;
        }

        .word-card.flipped .word-uz {
            display: none;
        }

        .word-card.flipped .word-en {
            display: block;
            color: white;
        }

        .word-hint {
            font-size: 0.8em;
            color: #64748B;
            margin-top: 10px;
        }

        /* Quiz Styles */
        .quiz-section {
            padding: 50px 20px;
            background: #0B1120;
            display: none;
        }

        .quiz-container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 20px;
        }

        .quiz-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 30px;
        }

        .quiz-header h2 {
            color: #06B6D4;
            font-size: 2.5em;
        }

        .quiz-timer {
            font-size: 2em;
            color: #06B6D4;
            font-weight: bold;
            padding: 15px 30px;
            background: #1E293B;
            border-radius: 8px;
            border: 2px solid #06B6D4;
        }

        .quiz-timer.warning {
            color: #f97316;
        }

        .quiz-timer.danger {
            color: #ef4444;
        }

        .question-card {
            background: #1E293B;
            padding: 40px;
            border-radius: 12px;
            margin-bottom: 30px;
            border-left: 6px solid #06B6D4;
            box-shadow: 0 8px 20px rgba(6, 182, 212, 0.15);
        }

        .question-text {
            font-size: 1.6em;
            margin-bottom: 30px;
            color: white;
            font-weight: 500;
            line-height: 1.5;
        }

        .options {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .option {
            padding: 18px 20px;
            background: #0F172A;
            border: 2px solid #475569;
            border-radius: 8px;
            cursor: pointer;
            color: white;
            transition: all 0.3s ease;
            font-size: 1.1em;
        }

        .option:hover {
            background: #1E293B;
            border-color: #06B6D4;
        }

        .option input[type="radio"] {
            margin-right: 10px;
            cursor: pointer;
        }

        .quiz-controls {
            display: flex;
            gap: 10px;
            margin-top: 30px;
        }

        .submit-btn,
        .back-btn {
            padding: 12px 25px;
            border: none;
            border-radius: 8px;
            font-size: 1em;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .submit-btn {
            background: #06B6D4;
            color: white;
            flex: 1;
        }

        .submit-btn:hover {
            background: #0891b2;
        }

        .back-btn {
            background: #1E293B;
            color: white;
            border: 2px solid #475569;
        }

        .back-btn:hover {
            background: #2D3E50;
        }

        .quiz-result {
            text-align: center;
            padding: 40px;
            background: linear-gradient(135deg, #2563EB 0%, #06B6D4 100%);
            border-radius: 12px;
            margin-bottom: 30px;
        }

        .result-score {
            font-size: 5em;
            font-weight: bold;
            margin-bottom: 15px;
        }

        .result-message {
            font-size: 1.8em;
            margin-bottom: 20px;
            font-weight: 500;
        }

        .leaderboard {
            background: #1E293B;
            padding: 20px;
            border-radius: 12px;
            margin-top: 30px;
        }

        .leaderboard h3 {
            color: #06B6D4;
            margin-top: 0;
            font-size: 1.8em;
        }

        .leaderboard-item {
            display: flex;
            justify-content: space-between;
            padding: 15px 0;
            border-bottom: 1px solid #475569;
            font-size: 1.2em;
        }

        .leaderboard-item:last-child {
            border-bottom: none;
        }

        .leaderboard-rank {
            color: #06B6D4;
            font-weight: bold;
        }

        .quiz-level-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .quiz-level-buttons button {
            font-size: 1.2em;
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            animation: fadeIn 0.3s ease;
        }

        .modal-content {
            background: linear-gradient(135deg, #1E293B 0%, #2563EB 100%);
            margin: 10% auto;
            padding: 40px;
            border-radius: 15px;
            width: 90%;
            max-width: 600px;
            box-shadow: 0 15px 35px rgba(6, 182, 212, 0.3);
            border: 2px solid #06B6D4;
            animation: slideIn 0.3s ease;
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 25px;
        }

        .modal-title {
            color: #06B6D4;
            font-size: 2em;
            font-weight: bold;
            margin: 0;
        }

        .close-btn {
            color: #94A3B8;
            font-size: 2em;
            font-weight: bold;
            cursor: pointer;
            transition: color 0.3s ease;
            background: none;
            border: none;
        }

        .quiz-question {
            background: linear-gradient(135deg, #06B6D4 0%, #2563EB 100%);
            color: rgb(255, 255, 255);
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 20px;
            font-size: 1.2em;
            line-height: 1.6;
            border-left: 5px solid #1e40af;
        }

        .word-display {
            background: rgba(0, 0, 0, 0.3);
            padding: 25px;
            border-radius: 10px;
            margin-bottom: 20px;
            border-left: 4px solid #06B6D4;
        }

        .word-text {
            color: white;
            font-size: 1.3em;
            line-height: 1.6;
            white-space: pre-line;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes slideIn {
            from { 
                opacity: 0;
                transform: translateY(-50px);
            }
            to { 
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* ============ RESPONSIVE DESIGN ============ */

        /* Tablets (768px and below) */
        @media (max-width: 768px) {
            .navbar {
                padding: 15px 20px;
            }

            .navbar nav {
                gap: 10px;
            }

            nav a {
                font-size: 0.9em;
                padding: 8px 12px;
            }

            .logo {
                font-size: 1.2em;
            }

            .hero {
                height: 150px;
                margin-bottom: 15px;
            }

            .hero h2 {
                font-size: 18px;
                margin-bottom: 5px;
            }

            .hero p {
                font-size: 10px;
                margin-bottom: 10px;
            }

            .hero button {
                padding: 6px 12px;
                font-size: 11px;
            }

            .vocab-container {
                max-width: 95%;
            }

            .vocab-container h2 {
                font-size: 1.8em;
            }

            .level-buttons {
                gap: 8px;
            }

            .level-btn {
                padding: 8px 12px;
                font-size: 0.85em;
            }

            .words-grid {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
                gap: 12px;
            }

            .word-card {
                padding: 15px;
                min-height: 100px;
            }

            .word-uz {
                font-size: 1.3em;
                margin-bottom: 5px;
            }

            .word-en {
                font-size: 0.9em;
            }

            .quiz-container {
                max-width: 95%;
                padding: 10px;
            }

            .question-card {
                padding: 20px;
                margin-bottom: 15px;
            }

            .question-text {
                font-size: 1.2em;
                margin-bottom: 15px;
            }

            .option {
                padding: 12px 15px;
                font-size: 0.95em;
            }

            .quiz-header h2 {
                font-size: 1.5em;
            }

            .quiz-timer {
                font-size: 1.3em;
                padding: 10px 15px;
            }

            .result-score {
                font-size: 3em;
            }

            .result-message {
                font-size: 1.3em;
            }

            .leaderboard h3 {
                font-size: 1.3em;
            }

            .leaderboard-item {
                padding: 10px 0;
                font-size: 0.95em;
            }

            .quiz-level-buttons button {
                font-size: 0.95em;
                padding: 10px 15px;
            }

            .auth-container {
                width: 90%;
                max-width: 300px;
            }

            .auth-container input {
                padding: 8px;
                font-size: 0.95em;
            }

            .auth-container button {
                padding: 8px;
                font-size: 0.9em;
            }
        }

        /* Phones (480px and below) */
        @media (max-width: 480px) {
            .navbar {
                padding: 10px 15px;
                flex-direction: column;
                gap: 10px;
            }

            .navbar nav {
                gap: 5px;
                width: 100%;
            }

            nav a {
                font-size: 0.8em;
                padding: 6px 8px;
                flex: 1;
                text-align: center;
            }

            .logo {
                font-size: 1em;
                margin-bottom: 5px;
            }

            .hero {
                height: 120px;
                border-radius: 10px;
                margin-bottom: 10px;
            }

            .hero h2 {
                font-size: 14px;
                margin-bottom: 3px;
            }

            .hero p {
                font-size: 8px;
                margin-bottom: 8px;
            }

            .hero button {
                padding: 5px 10px;
                font-size: 10px;
            }

            .vocab-container {
                max-width: 100%;
            }

            .vocab-container h2 {
                font-size: 1.3em;
                margin-bottom: 15px;
            }

            .level-buttons {
                gap: 5px;
                margin-bottom: 15px;
            }

            .level-btn {
                padding: 6px 8px;
                font-size: 0.75em;
            }

            .words-grid {
                grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
                gap: 8px;
            }

            .word-card {
                padding: 12px;
                min-height: 80px;
                border-left: 3px solid #06B6D4;
            }

            .word-uz {
                font-size: 1em;
                margin-bottom: 3px;
            }

            .word-en {
                font-size: 0.75em;
            }

            .word-hint {
                font-size: 0.7em;
            }

            .quiz-container {
                max-width: 100%;
                padding: 8px;
            }

            .quiz-header {
                flex-direction: column;
                gap: 10px;
            }

            .question-card {
                padding: 15px;
                margin-bottom: 10px;
                border-left: 4px solid #06B6D4;
            }

            .question-text {
                font-size: 1em;
                margin-bottom: 12px;
            }

            .option {
                padding: 10px 12px;
                font-size: 0.85em;
                margin-bottom: 5px;
            }

            .quiz-header h2 {
                font-size: 1.2em;
            }

            .quiz-timer {
                font-size: 1.1em;
                padding: 8px 12px;
                border: 1px solid #06B6D4;
            }

            .quiz-controls {
                flex-direction: column;
                gap: 8px;
            }

            .submit-btn,
            .back-btn {
                padding: 10px 15px;
                font-size: 0.9em;
            }

            .result-score {
                font-size: 2.5em;
            }

            .result-message {
                font-size: 1em;
            }

            .quiz-result {
                padding: 20px;
                margin-bottom: 15px;
            }

            .leaderboard {
                padding: 15px;
            }

            .leaderboard h3 {
                font-size: 1.1em;
            }

            .leaderboard-item {
                padding: 8px 0;
                font-size: 0.85em;
            }

            .quiz-level-buttons {
                gap: 8px;
                margin-bottom: 20px;
            }

            .quiz-level-buttons button {
                font-size: 0.85em;
                padding: 8px 12px;
                flex: 1;
            }

            .auth-container {
                width: 95%;
                padding: 20px;
            }

            .auth-container input {
                padding: 6px;
                font-size: 0.9em;
            }

            .auth-container button {
                padding: 8px;
                font-size: 0.85em;
            }

            footer {
                padding: 15px;
                font-size: 0.9em;
            }
        }
    </style>
</head>

<body>

    <header class="navbar">
        <h1 class="logo">ZENTRIXA</h1>
        <nav>
            <a onclick="showVocab()">Lug'atlar</a>
            <a onclick="showQuiz()" class="test-link">🎯 Test</a>
            <a onclick="generateIELTSWord()">📚 IELTS Word</a>
            <a onclick="showProfile()">👤 Profil</a>
        </nav>
    </header>

    <section class="hero" id="heroSection">
        <h2>Master Words. Master the World.</h2>
        <p>AI-powered English vocabulary learning platform for global minds.</p>
        <button onclick="showVocab()">Lug'atlarni O'rganish</button>
    </section>

    <section class="vocab-section" id="vocabulary">
        <div class="vocab-container">
            <h2>Lug'atlar</h2>
            <div class="level-buttons">
                <button onclick="showLevel('A1')" class="level-btn active">A1 (Boshlang'ich)</button>
                <button onclick="showLevel('A2')" class="level-btn">A2</button>
                <button onclick="showLevel('B1')" class="level-btn">B1 (O'rta)</button>
                <button onclick="showLevel('B2')" class="level-btn">B2</button>
                <button onclick="showLevel('C1')" class="level-btn">C1 (Yuqori)</button>
            </div>
            <div id="wordsContainer" class="words-grid"></div>
        </div>
    </section>

    <section class="quiz-section" id="quizSection">
        <div class="quiz-container">
            <div style="text-align: center; margin: 30px 0; padding: 20px; background: rgba(6, 182, 212, 0.1); border-radius: 10px;">
                <h4 style="color: #06B6D4; margin-bottom: 15px;">📊 O'rganish statistikasi</h4>
                <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 15px; margin-bottom: 20px;">
                    <div style="background: rgba(6, 182, 212, 0.1); padding: 15px; border-radius: 8px;">
                        <h5 style="color: #06B6D4; margin: 0;">📚 Lug'atlar</h5>
                        <p style="color: white; font-size: 1.1em; margin: 5px 0;">467 ta umumiy so'z</p>
                    </div>
                    <div style="background: rgba(6, 182, 212, 0.1); padding: 15px; border-radius: 8px;">
                        <h5 style="color: #2563EB; margin: 0;">🎯 Testlar</h5>
                        <p style="color: white; font-size: 1.1em; margin: 5px 0;">Har daraja uchun 15 ta test</p>
                    </div>
                    <div style="background: rgba(6, 182, 212, 0.1); padding: 15px; border-radius: 8px;">
                        <h5 style="color: #10b981; margin: 0;">📚 IELTS So'zlar</h5>
                        <p style="color: white; font-size: 1.1em; margin: 5px 0;">125 ta IELTS so'zi (A1-C1)</p>
                    </div>
                    <div style="background: rgba(6, 182, 212, 0.1); padding: 15px; border-radius: 8px;">
                        <h5 style="color: #f59e0b; margin: 0;">👤 Foydalanuvchi Profili</h5>
                        <p style="color: white; font-size: 1.1em; margin: 5px 0;">Shaxsiy statistika va yutuqlar</p>
                    </div>
                </div>
            </div>

            <div id="quizLevelSelect">
                <h2 style="text-align: center; color: #06B6D4; margin-bottom: 30px;">Test Darajasini Tanlang</h2>
                <div class="quiz-level-buttons">
                    <button onclick="startQuiz('A1')" class="level-btn">A1 (Boshlang'ich)</button>
                    <button onclick="startQuiz('A2')" class="level-btn">A2</button>
                    <button onclick="startQuiz('B1')" class="level-btn">B1 (O'rta)</button>
                    <button onclick="startQuiz('B2')" class="level-btn">B2</button>
                    <button onclick="startQuiz('C1')" class="level-btn">C1 (Yuqori)</button>
                </div>
                <div style="text-align: center; margin-top: 20px;">
                    <button onclick="showVocab()" class="back-btn">Orqaga</button>
                </div>
            </div>

            <div id="quizContent" style="display: none;">
                <div class="quiz-header">
                    <h2 id="quizLevelTitle">Test</h2>
                    <div class="quiz-timer" id="timerDisplay">3:00</div>
                    <div class="quiz-progress" id="quizProgress">1/15</div>
                </div>
                <div id="questionsContainer"></div>
                <div class="quiz-controls">
                    <button onclick="submitQuiz()" class="submit-btn">Javoblarni Jo'natish</button>
                    <button onclick="backToQuizLevel()" class="back-btn">Orqaga</button>
                </div>
            </div>

            <div id="quizResults" style="display: none;">
                <div class="quiz-result">
                    <div class="result-score" id="resultScore">0/5</div>
                    <div class="result-message" id="resultMessage">Yaxshi natija!</div>
                </div>
                <div id="leaderboardContainer"></div>
                <div style="text-align: center; margin-top: 20px;">
                    <button onclick="showQuiz()" class="submit-btn">Yana Test Qilish</button>
                    <button onclick="showVocab()" class="back-btn">Lug'atlarga Qaytish</button>
                </div>
            </div>
        </div>
    </section>

    <section id="profile" class="auth-section">

        <div class="auth-container">
            <h2>👤 Foydalanuvchi Profili</h2>
            <div style="text-align: center; margin-bottom: 30px;">
                <div style="width: 80px; height: 80px; background: linear-gradient(135deg, #06B6D4 0%, #2563EB 100%); border-radius: 50%; margin: 0 auto 20px; display: flex; align-items: center; justify-content: center; font-size: 2em;">
                    👤
                </div>
                <h3 style="color: #06B6D4; margin: 0;">ZENTRIXA Foydalanuvchisi</h3>
                <p style="color: #94A3B8; margin: 5px 0;">Bepul versiya</p>
            </div>
            
            <div style="background: rgba(6, 182, 212, 0.1); padding: 20px; border-radius: 10px; margin-bottom: 20px;">
                <h4 style="color: #06B6D4; margin: 0 0 15px 0;">📊 O'rganish statistikasi</h4>
                <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 15px;">
                    <div style="text-align: center;">
                        <div style="font-size: 2em; color: #06B6D4; font-weight: bold;">227</div>
                        <div style="color: #94A3B8; font-size: 0.9em;">Umumiy so'zlar</div>
                    </div>
                    <div style="text-align: center;">
                        <div style="font-size: 2em; color: #06B6D4; font-weight: bold;">5</div>
                        <div style="color: #94A3B8; font-size: 0.9em;">Darajalar</div>
                    </div>
                    <div style="text-align: center;">
                        <div style="font-size: 2em; color: #06B6D4; font-weight: bold;">125</div>
                        <div style="color: #94A3B8; font-size: 0.9em;">IELTS so'zlar</div>
                    </div>
                    <div style="text-align: center;">
                        <div style="font-size: 2em; color: #06B6D4; font-weight: bold;">∞</div>
                        <div style="color: #94A3B8; font-size: 0.9em;">Cheksiz o'rganish</div>
                    </div>
                </div>
            </div>

            <div style="background: rgba(6, 182, 212, 0.1); padding: 20px; border-radius: 10px; margin-bottom: 20px;">
                <h4 style="color: #06B6D4; margin: 0 0 15px 0;">🏆 Yutuqlar</h4>
                <div style="display: flex; flex-wrap: wrap; gap: 10px;">
                    <span style="background: #06B6D4; color: white; padding: 5px 10px; border-radius: 15px; font-size: 0.8em;">🎯 Test ustasi</span>
                    <span style="background: #2563EB; color: rgb(255, 255, 255); padding: 5px 10px; border-radius: 15px; font-size: 0.8em;">📚 So'z yig'uvchi</span>
                    <span style="background: #10b981; color: white; padding: 5px 10px; border-radius: 15px; font-size: 0.8em;">🌍 Global learner</span>
                    <span style="background: #f59e0b; color: white; padding: 5px 10px; border-radius: 15px; font-size: 0.8em;">⚡ Tez o'rganuvchi</span>
                </div>
            </div>

            <div style="background: rgba(6, 182, 212, 0.1); padding: 20px; border-radius: 10px; margin-bottom: 20px;">
                <h4 style="color: #06B6D4; margin: 0 0 15px 0;">📈 O'rganish darajalari</h4>
                <div style="display: flex; flex-direction: column; gap: 10px;">
                    <div style="display: flex; justify-content: space-between; align-items: center;">
                        <span>A1 (Boshlang'ich)</span>
                        <span style="color: #10b981;">✅ 80 so'z</span>
                    </div>
                    <div style="display: flex; justify-content: space-between; align-items: center;">
                        <span>A2 (Elementary)</span>
                        <span style="color: #10b981;">✅ 85 so'z</span>
                    </div>
                    <div style="display: flex; justify-content: space-between; align-items: center;">
                        <span>B1 (Intermediate)</span>
                        <span style="color: #f59e0b;">🔄 90 so'z</span>
                    </div>
                    <div style="display: flex; justify-content: space-between; align-items: center;">
                        <span>B2 (Upper-Intermediate)</span>
                        <span style="color: #ef4444;">⏳ 87 so'z</span>
                    </div>
                    <div style="display: flex; justify-content: space-between; align-items: center;">
                        <span>C1 (Advanced)</span>
                        <span style="color: #ef4444;">⏳ 95 so'z</span>
                    </div>
                </div>
            </div>

            <div style="text-align: center; margin-top: 30px;">
                <button onclick="showVocab()" style="background: #06B6D4; color: white; border: none; padding: 12px 25px; border-radius: 8px; cursor: pointer; font-size: 1em; margin-bottom: 10px; width: 100%;">
                    📚 Lug'atlarni O'rganish
                </button>
                <button onclick="showQuiz()" style="background: #2563EB; color: white; border: none; padding: 12px 25px; border-radius: 8px; cursor: pointer; font-size: 1em; width: 100%;">
                    🎯 Test Qilish
                </button>
            </div>
        </div>

    </section>

    <footer>
        <p> 2026 ZENTRIX. All rights reserved.</p>
    </footer>

    <!-- IELTS Word Modal -->
    <div id="ieltsModal" class="modal">
        <div class="modal-content">
            <div class="modal-header">
                <h2 class="modal-title"> IELTS Vocabulary</h2>
                <button class="close-btn" onclick="closeIELTSModal()">&times;</button>
            </div>
            <div class="word-display">
                <p class="word-text" id="ieltsWordText"></p>
            </div>
        </div>
    </div>

    <script>
        // Static API - for GitHub Pages deployment

        const WORDS = {
            A1: [
                { uz: "salom", en: "hello" },
                { uz: "kitob", en: "book" },
                { uz: "uy", en: "house" },
                { uz: "maktab", en: "school" },
                { uz: "suv", en: "water" },
                { uz: "ovqat", en: "food" },
                { uz: "ona", en: "mother" },
                { uz: "ota", en: "father" },
                { uz: "do'st", en: "friend" },
                { uz: "ish", en: "work" },
                { uz: "kun", en: "day" },
                { uz: "kecha", en: "night" },
                { uz: "yil", en: "year" },
                { uz: "bola", en: "child" },
                { uz: "erkak", en: "man" },
                { uz: "ayol", en: "woman" },
                { uz: "stol", en: "table" },
                { uz: "stul", en: "chair" },
                { uz: "telefon", en: "phone" },
                { uz: "yo'l", en: "road" },
                { uz: "qora", en: "black" },
                { uz: "oq", en: "white" },
                { uz: "katta", en: "big" },
                { uz: "kichik", en: "small" },
                { uz: "yaxshi", en: "good" },
                { uz: "yomon", en: "bad" },
                { uz: "issiq", en: "hot" },
                { uz: "sovuq", en: "cold" },
                { uz: "tekin", en: "free" },
                { uz: "qimmat", en: "expensive" },
                { uz: "arzon", en: "cheap" },
                { uz: "yangi", en: "new" },
                { uz: "eski", en: "old" },
                { uz: "go'zal", en: "beautiful" },
                { uz: "qiziq", en: "interesting" },
                { uz: "oson", en: "easy" },
                { uz: "qiyin", en: "difficult" },
                { uz: "xavfli", en: "dangerous" },
                { uz: "xavfsiz", en: "safe" },
                { uz: "muvaffaqiyatli", en: "successful" },
                { uz: "sog'lom", en: "healthy" }
            ],
            A2: [
                { uz: "sayohat", en: "travel" },
                { uz: "uchrashuv", en: "meeting" },
                { uz: "savol", en: "question" },
                { uz: "javob", en: "answer" },
                { uz: "dars", en: "lesson" },
                { uz: "mashq", en: "exercise" },
                { uz: "bozor", en: "market" },
                { uz: "kasal", en: "sick" },
                { uz: "shifokor", en: "doctor" },
                { uz: "dori", en: "medicine" },
                { uz: "mehmon", en: "guest" },
                { uz: "ofis", en: "office" },
                { uz: "xona", en: "room" },
                { uz: "mehmonxona", en: "hotel" },
                { uz: "samolyot", en: "airplane" },
                { uz: "poezd", en: "train" },
                { uz: "avtobus", en: "bus" },
                { uz: "chipta", en: "ticket" },
                { uz: "ishchi", en: "worker" },
                { uz: "o'qituvchi", en: "teacher" },
                { uz: "talaba", en: "student" },
                { uz: "universitet", en: "university" },
                { uz: "kutubxona", en: "library" },
                { uz: "restoran", en: "restaurant" },
                { uz: "kofe", en: "coffee" },
                { uz: "choy", en: "tea" },
                { uz: "nonushta", en: "breakfast" },
                { uz: "tushlik", en: "lunch" },
                { uz: "kechki ovqat", en: "dinner" },
                { uz: "transport", en: "transport" },
                { uz: "avtomobil", en: "car" },
                { uz: "velosiped", en: "bicycle" },
                { uz: "metro", en: "metro" },
                { uz: "aeroport", en: "airport" },
                { uz: "vokzal", en: "station" },
                { uz: "mahsulot", en: "product" },
                { uz: "xizmat", en: "service" },
                { uz: "kafolat", en: "guarantee" },
                { uz: "shartnoma", en: "contract" },
                { uz: "taklif", en: "offer" },
                { uz: "narx", en: "price" },
                { uz: "sifat", en: "quality" },
                { uz: "miqdor", en: "quantity" },
                { uz: "tartib", en: "order" },
                { uz: "qoida", en: "rule" },
                { uz: "huquq", en: "right" },
                { uz: "majburiyat", en: "responsibility" }
            ],
            B1: [
                { uz: "tajriba", en: "experience" },
                { uz: "maslahat", en: "advice" },
                { uz: "munosabat", en: "relationship" },
                { uz: "jamiyat", en: "society" },
                { uz: "madaniyat", en: "culture" },
                { uz: "an'ana", en: "tradition" },
                { uz: "maqsad", en: "goal" },
                { uz: "natija", en: "result" },
                { uz: "loyiha", en: "project" },
                { uz: "rahbar", en: "leader" },
                { uz: "xodim", en: "employee" },
                { uz: "mijoz", en: "client" },
                { uz: "raqobat", en: "competition" },
                { uz: "bozor", en: "market" },
                { uz: "iqtisod", en: "economy" },
                { uz: "ta'sir", en: "impact" },
                { uz: "xizmat", en: "service" },
                { uz: "texnologiya", en: "technology" },
                { uz: "axborot", en: "information" },
                { uz: "aloqa", en: "communication" },
                { uz: "strategiya", en: "strategy" },
                { uz: "tahlil", en: "analysis" },
                { uz: "baholash", en: "evaluation" },
                { uz: "rivojlanish", en: "development" },
                { uz: "o'sish", en: "growth" },
                { uz: "progress", en: "progress" },
                { uz: "muvaffaqiyat", en: "success" },
                { uz: "muvofiqlik", en: "compliance" },
                { uz: "samara", en: "efficiency" },
                { uz: "samaradorlik", en: "productivity" },
                { uz: "innovatsiya", en: "innovation" },
                { uz: "tadqiqot", en: "research" },
                { uz: "kashfiyot", en: "discovery" },
                { uz: "ixtiro", en: "invention" },
                { uz: "ilmiy", en: "scientific" },
                { uz: "akademik", en: "academic" },
                { uz: "professional", en: "professional" },
                { uz: "mutaxassis", en: "specialist" },
                { uz: "ekspert", en: "expert" },
                { uz: "konsultatsiya", en: "consultation" },
                { uz: "rekomendatsiya", en: "recommendation" },
                { uz: "xulosa", en: "conclusion" },
                { uz: "qaror", en: "decision" },
                { uz: "tanlov", en: "choice" },
                { uz: "imkoniyat", en: "opportunity" },
                { uz: "salohiyat", en: "potential" },
                { uz: "qobiliyat", en: "ability" },
                { uz: "ko'nikma", en: "skill" }
            ],
            B2: [
                { uz: "murakkab", en: "complex" },
                { uz: "nazariya", en: "theory" },
                { uz: "amaliyot", en: "practice" },
                { uz: "innovatsion", en: "innovative" },
                { uz: "raqamli", en: "digital" },
                { uz: "global", en: "global" },
                { uz: "muhim", en: "significant" },
                { uz: "barqaror", en: "sustainable" },
                { uz: "tadqiqot", en: "research" },
                { uz: "yechim", en: "solution" },
                { uz: "samarali", en: "efficient" },
                { uz: "muvofiq", en: "appropriate" },
                { uz: "jarayon", en: "process" },
                { uz: "tizim", en: "system" },
                { uz: "resurs", en: "resource" },
                { uz: "rahbariyat", en: "management" },
                { uz: "tashkilot", en: "organization" },
                { uz: "muvaffaqiyatli", en: "successful" },
                { uz: "sifat", en: "quality" },
                { uz: "strategik", en: "strategic" },
                { uz: "operativ", en: "operational" },
                { uz: "taktik", en: "tactical" },
                { uz: "analitik", en: "analytical" },
                { uz: "mantiqiy", en: "logical" },
                { uz: "ijodiy", en: "creative" },
                { uz: "initsiativ", en: "initiative" },
                { uz: "integratsiya", en: "integration" },
                { uz: "transformatsiya", en: "transformation" },
                { uz: "modernizatsiya", en: "modernization" },
                { uz: "optimizatsiya", en: "optimization" },
                { uz: "avtomatlashtirish", en: "automation" },
                { uz: "digitalizatsiya", en: "digitalization" },
                { uz: "sun'iy intellekt", en: "artificial intelligence" },
                { uz: "mashina o'rganishi", en: "machine learning" },
                { uz: "kiberxavfsizlik", en: "cybersecurity" },
                { uz: "blokcheyn", en: "blockchain" },
                { uz: "kriptovalyuta", en: "cryptocurrency" },
                { uz: "elektron tijorat", en: "e-commerce" },
                { uz: "ijtimoiy media", en: "social media" },
                { uz: "bulutli hisoblash", en: "cloud computing" },
                { uz: "katta ma'lumotlar", en: "big data" },
                { uz: "Internet narsalari", en: "Internet of Things" },
                { uz: "virtual reallik", en: "virtual reality" },
                { uz: "qo'shimcha reallik", en: "augmented reality" },
                { uz: "kvant hisoblash", en: "quantum computing" },
                { uz: "biotexnologiya", en: "biotechnology" },
                { uz: "nanotexnologiya", en: "nanotechnology" }
            ],
            C1: [
                { uz: "mukammal", en: "comprehensive" },
                { uz: "innovatsion", en: "innovative" },
                { uz: "globalizatsiya", en: "globalization" },
                { uz: "tahliliy", en: "analytical" },
                { uz: "mantiqiy", en: "logical" },
                { uz: "konseptual", en: "conceptual" },
                { uz: "intellektual", en: "intellectual" },
                { uz: "strategik fikrlash", en: "strategic thinking" },
                { uz: "murakkab tizim", en: "complex system" },
                { uz: "raqobatbardosh", en: "competitive" },
                { uz: "barqarorlik strategiyasi", en: "sustainability strategy" },
                { uz: "resurslarni boshqarish", en: "resource management" },
                { uz: "liderlik", en: "leadership" },
                { uz: "hamkorlik muhiti", en: "collaborative environment" },
                { uz: "qaror qabul qilish", en: "decision making" },
                { uz: "ijodkorlik", en: "creativity" },
                { uz: "tanqidiy fikrlash", en: "critical thinking" },
                { uz: "barqaror o'sish", en: "sustainable growth" },
                { uz: "muammoli vaziyat", en: "challenging situation" },
                { uz: "ilmiy yondashuv", en: "scientific approach" },
                { uz: "empirik tadqiqot", en: "empirical research" },
                { uz: "gipotezani tekshirish", en: "hypothesis testing" },
                { uz: "statistik tahlil", en: "statistical analysis" },
                { uz: "kvantitativ usullar", en: "quantitative methods" },
                { uz: "kvalitativ tadqiqot", en: "qualitative research" },
                { uz: "interdisiplinar yondashuv", en: "interdisciplinary approach" },
                { uz: "multidimensional tahlil", en: "multidimensional analysis" },
                { uz: "paradigmatik siljish", en: "paradigm shift" },
                { uz: "sistemli fikrlash", en: "systems thinking" },
                { uz: "holistik yondashuv", en: "holistic approach" },
                { uz: "sintetik tahlil", en: "synthetic analysis" },
                { uz: "dialektik mantiq", en: "dialectical logic" },
                { uz: "epistemologik asos", en: "epistemological foundation" },
                { uz: "ontologik tushuncha", en: "ontological concept" },
                { uz: "aksiologik qiymat", en: "axiological value" },
                { uz: "teleologik maqsad", en: "teleological purpose" },
                { uz: "metodologik asos", en: "methodological basis" },
                { uz: "fenomenologik tahlil", en: "phenomenological analysis" },
                { uz: "ekzistensial falsafa", en: "existential philosophy" },
                { uz: "pragmatik falsafa", en: "pragmatic philosophy" },
                { uz: "pozitivizm", en: "positivism" },
                { uz: "postmodernizm", en: "postmodernism" },
                { uz: "strukturalizm", en: "structuralism" },
                { uz: "dekonstruktivizm", en: "deconstructionism" }
            ]
        };

        let currentLevel = 'A1';
        let quizQuestions = [];
        let quizAnswers = {};
        let quizTimeLeft = 180;
        let quizTimer = null;

        // Quiz Questions Data
        const QUIZ_QUESTIONS = {
            A1: [
                { question: "Hello qanday tarjima?", options: ["hayr", "salom", "xayr", "rahmat"], answer: "salom" },
                { question: "Book nima?", options: ["kitob", "qalam", "daftar", "ruchka"], answer: "kitob" },
                { question: "Water qanday?", options: ["suv", "choy", "qahva", "sharbat"], answer: "suv" },
                { question: "House nima?", options: ["uy", "makon", "joy", "bino"], answer: "uy" },
                { question: "Car qanday?", options: ["mashina", "velosiped", "poyezd", "samolyot"], answer: "mashina" },
                { question: "School nima?", options: ["maktab", "universitet", "kollej", "institut"], answer: "maktab" },
                { question: "Teacher qanday?", options: ["o'qituvchi", "o'quvchi", "direktor", "hamshira"], answer: "o'qituvchi" },
                { question: "Student nima?", options: ["o'quvchi", "o'qituvchi", "o'qituvchi", "direktor"], answer: "o'quvchi" },
                { question: "Friend qanday?", options: ["do'st", "dushman", "qarindosh", "tanish"], answer: "do'st" },
                { question: "Family nima?", options: ["oilaviy", "jamoasi", "guruh", "jamoa"], answer: "oilaviy" },
                { question: "Father qanday?", options: ["ota", "ona", "aka", "uka"], answer: "ota" },
                { question: "Mother nima?", options: ["ona", "ota", "opa", "singil"], answer: "ona" },
                { question: "Brother qanday?", options: ["aka", "uka", "dada", "bobo"], answer: "aka" },
                { question: "Sister nima?", options: ["opa", "singil", "mama", "bibi"], answer: "opa" },
                { question: "Love qanday?", options: ["sevgi", "nafrat", "do'stlik", "munosabat"], answer: "sevgi" },
                { question: "Happy nima?", options: ["baxtli", "qayg'uli", "g'azabli", "xursand"], answer: "baxtli" },
                { question: "Sad qanday?", options: ["qayg'uli", "baxtli", "xursand", "quvnoq"], answer: "qayg'uli" },
                { question: "Good nima?", options: ["yaxshi", "yomon", "o'rtacha", "a'lo"], answer: "yaxshi" },
                { question: "Bad qanday?", options: ["yomon", "yaxshi", "zo'r", "a'lo"], answer: "yomon" },
                { question: "Big nima?", options: ["katta", "kichik", "o'rtacha", "normal"], answer: "katta" },
                { question: "Small qanday?", options: ["kichik", "katta", "o'rtacha", "keng"], answer: "kichik" },
                { question: "Hot nima?", options: ["issiq", "sovuq", "ilgiq", "salqin"], answer: "issiq" },
                { question: "Cold qanday?", options: ["sovuq", "issiq", "ilgiq", "qizg'in"], answer: "sovuq" },
                { question: "Fast nima?", options: ["tezkor", "sekin", "o'rtacha", "normal"], answer: "tezkor" },
                { question: "Slow qanday?", options: ["sekin", "tezkor", "tez", "shoshilinch"], answer: "sekin" },
                { question: "Easy nima?", options: ["oson", "qiyin", "murakkab", "nozik"], answer: "oson" },
                { question: "Hard qanday?", options: ["qiyin", "oson", "sodda", "oddiy"], answer: "qiyin" },
                { question: "New nima?", options: ["yangi", "eski", "zamonaviy", "qadimiy"], answer: "yangi" },
                { question: "Old qanday?", options: ["eski", "yangi", "zamonaviy", "hozirgi"], answer: "eski" },
                { question: "Young nima?", options: ["yosh", "qari", "o'rta yoshli", "katta"], answer: "yosh" },
                { question: "Old age qanday?", options: ["qari", "yosh", "yoshlik", "o'smirlar"], answer: "qari" },
                { question: "Today nima?", options: ["bugun", "ertaga", "kecha", "hozir"], answer: "bugun" },
                { question: "Tomorrow qanday?", options: ["ertaga", "bugun", "kecha", "hozir"], answer: "ertaga" },
                { question: "Yesterday nima?", options: ["kecha", "bugun", "ertaga", "hozir"], answer: "kecha" },
                { question: "Now qanday?", options: ["hozir", "keyin", "oldin", "vaqtni"], answer: "hozir" },
                { question: "Later nima?", options: ["keyin", "hozir", "oldin", "vaqtni"], answer: "keyin" },
                { question: "Before qanday?", options: ["oldin", "keyin", "hozir", "vaqtni"], answer: "oldin" },
                { question: "After nima?", options: ["keyin", "oldin", "hozir", "vaqtni"], answer: "keyin" },
                { question: "Up qanday?", options: ["yuqoriga", "pastga", "chapga", "o'ngga"], answer: "yuqoriga" },
                { question: "Down nima?", options: ["pastga", "yuqoriga", "chapga", "o'ngga"], answer: "pastga" },
                { question: "Left qanday?", options: ["chapga", "o'ngga", "yuqoriga", "pastga"], answer: "chapga" },
                { question: "Right nima?", options: ["o'ngga", "chapga", "yuqoriga", "pastga"], answer: "o'ngga" },
                { question: "In nima?", options: ["ichida", "tashqarida", "ustida", "ostida"], answer: "ichida" },
                { question: "Out qanday?", options: ["tashqarida", "ichida", "ustida", "ostida"], answer: "tashqarida" },
                { question: "On nima?", options: ["ustida", "ostida", "ichida", "tashqarida"], answer: "ustida" },
                { question: "Under qanday?", options: ["ostida", "ustida", "ichida", "tashqarida"], answer: "ostida" },
                { question: "Yes nima?", options: ["ha", "yo'q", "albatta", "ehtimol"], answer: "ha" },
                { question: "No qanday?", options: ["yo'q", "ha", "albatta", "ehtimol"], answer: "yo'q" },
                { question: "Please nima?", options: ["iltimos", "rahmat", "kafolat", "uzr"], answer: "iltimos" },
                { question: "Thank you qanday?", options: ["rahmat", "iltimos", "uzr", "kafolat"], answer: "rahmat" },
                { question: "Sorry nima?", options: ["uzr", "rahmat", "iltimos", "kafolat"], answer: "uzr" },
                { question: "Excuse me qanday?", options: ["uzr", "rahmat", "iltimos", "kafolat"], answer: "uzr" },
                { question: "Goodbye nima?", options: ["xayr", "salom", "rahmat", "iltimos"], answer: "xayr" },
                { question: "Hello again qanday?", options: ["salom", "xayr", "rahmat", "iltimos"], answer: "salom" },
                { question: "How are you? nima?", options: ["qalaysiz", "rahmat", "salom", "xayr"], answer: "qalaysiz" },
                { question: "I'm fine nima?", options: ["yaxshiman", "yomonman", "qalaysiz", "rahmat"], answer: "yaxshiman" },
                { question: "What's your name? nima?", options: ["ismingiz nima", "qalaysiz", "rahmat", "salom"], answer: "ismingiz nima" },
                { question: "My name is... nima?", options: ["mening ismim", "sening isming", "uning ismi", "ularning ismlari"], answer: "mening ismim" },
                { question: "Where are you from? nima?", options: ["qayerdasiz", "qaysisiz", "qayerdan", "qandaysiz"], answer: "qayerdasiz" },
                { question: "I'm from... nima?", options: ["men ...dan", "siz ...dan", "u ...dan", "ular ...dan"], answer: "men ...dan" },
                { question: "How old are you? nima?", options: ["yoshingiz nechchi", "ismingiz nima", "qalaysiz", "qayerdasiz"], answer: "yoshingiz nechchi" },
                { question: "I'm... years old nima?", options: ["men ...yoshdaman", "siz ...yoshdasiz", "u ...yoshda", "ular ...yoshda"], answer: "men ...yoshdaman" },
                { question: "What time is it? nima?", options: ["so'at nechchi", "qalaysiz", "rahmat", "salom"], answer: "so'at nechchi" },
                { question: "It's... o'clock nima?", options: ["so'at ...", "so'at nechchi", "qalaysiz", "rahmat"], answer: "so'at ..." },
                { question: "Where is...? nima?", options: ["...qayerda", "...qaysi", "...qanday", "...nechchi"], answer: "...qayerda" },
                { question: "It's... nima?", options: ["u ...da", "u ...qayerda", "u ...qanday", "u ...nechchi"], answer: "u ...da" },
                { question: "What is this? nima?", options: ["bu nima", "bu qayerda", "bu qanday", "bu nechchi"], answer: "bu nima" },
                { question: "This is... nima?", options: ["bu ...", "bu ...nima", "bu ...qayerda", "bu ...qanday"], answer: "bu ..." },
                { question: "What are these? nima?", options: ["ular nima", "ular qayerda", "ular qanday", "ular nechchi"], answer: "ular nima" },
                { question: "These are... nima?", options: ["ular ...", "ular ...nima", "ular ...qayerda", "ular ...qanday"], answer: "ular ..." },
                { question: "Who is...? nima?", options: ["...kim", "...nima", "...qayerda", "...qanday"], answer: "...kim" },
                { question: "He/She is... nima?", options: ["u ...", "u ...kim", "u ...nima", "u ...qayerda"], answer: "u ..." },
                { question: "When is...? nima?", options: ["...qachon", "...qayerda", "...qanday", "...nechchi"], answer: "...qachon" },
                { question: "It's... (time) nima?", options: ["...da", "...qachon", "...qayerda", "...qanday"], answer: "...da" },
                { question: "Why...? nima?", options: ["...nima uchun", "...qayerda", "...qanday", "...nechchi"], answer: "...nima uchun" },
                { question: "Because... nima?", options: ["chunki...", "...nima uchun", "...qayerda", "...qanday"], answer: "chunki..." },
                { question: "Which...? nima?", options: ["...qaysi", "...nima", "...qayerda", "...qanday"], answer: "...qaysi" },
                { question: "The... one nima?", options: ["...tasi", "...qaysi", "...nima", "...qayerda"], answer: "...tasi" },
                { question: "How much/many...? nima?", options: ["...nechta", "...qaysi", "...nima", "...qayerda"], answer: "...nechta" },
                { question: "There is/are... nima?", options: ["...bor", "...yo'q", "...bor", "...mavjud"], answer: "...bor" },
                { question: "There isn't/aren't... nima?", options: ["...yo'q", "...bor", "...mavjud", "...bor"], answer: "...yo'q" },
                { question: "Can you...? nima?", options: ["...qila olasizmi", "...qilamizmi", "...qilasizmi", "...qilamiz"], answer: "...qila olasizmi" },
                { question: "Yes, I can nima?", options: ["ha, qila olaman", "yo'q, qila olmayman", "ha, qilaman", "yo'q, qilmayman"], answer: "ha, qila olaman" },
                { question: "No, I can't nima?", options: ["yo'q, qila olmayman", "ha, qila olaman", "yo'q, qilmayman", "ha, qilaman"], answer: "yo'q, qila olmayman" },
                { question: "Do you...? nima?", options: ["...mimi", "...mimi", "...mimi", "...mimi"], answer: "...mimi" },
                { question: "Yes, I do nima?", options: ["ha, qilaman", "yo'q, qilmayman", "ha, qila olaman", "yo'q, qila olmayman"], answer: "ha, qilaman" },
                { question: "No, I don't nima?", options: ["yo'q, qilmayman", "ha, qilaman", "yo'q, qila olmayman", "ha, qila olaman"], answer: "yo'q, qilmayman" },
                { question: "Are you...? nima?", options: ["...mimi", "...mimi", "...mimi", "...mimi"], answer: "...mimi" },
                { question: "Yes, I am nima?", options: ["ha, ...man", "yo'q, ...man emasman", "ha, ...man", "yo'q, ...man"], answer: "ha, ...man" },
                { question: "No, I'm not nima?", options: ["yo'q, ...man emasman", "ha, ...man", "yo'q, ...man", "ha, ...man emasman"], answer: "yo'q, ...man emasman" },
                { question: "What do you like? nima?", options: ["nima yoqtiradi", "nima yoqtirmaydi", "qanday", "qayerda"], answer: "nima yoqtiradi" },
                { question: "I like... nima?", options: ["men ...yoqtiraman", "men ...yoqtirmayman", "men ...qilaman", "men ...qilmayman"], answer: "men ...yoqtiraman" },
                { question: "What don't you like? nima?", options: ["nima yoqtirmaydi", "nima yoqtiradi", "qanday", "qayerda"], answer: "nima yoqtirmaydi" },
                { question: "I don't like... nima?", options: ["men ...yoqtirmayman", "men ...yoqtiraman", "men ...qilaman", "men ...qilmayman"], answer: "men ...yoqtirmayman" },
                { question: "I want... nima?", options: ["men ...xohlayman", "men ...xohlamayman", "men ...qilaman", "men ...qilmayman"], answer: "men ...xohlayman" },
                { question: "I don't want... nima?", options: ["men ...xohlamayman", "men ...xohlayman", "men ...qilaman", "men ...qilmayman"], answer: "men ...xohlamayman" },
                { question: "I need... nima?", options: ["men ...kerak", "men ...kerak emas", "men ...xohlayman", "men ...xohlamayman"], answer: "men ...kerak" },
                { question: "I don't need... nima?", options: ["men ...kerak emas", "men ...kerak", "men ...xohlayman", "men ...xohlamayman"], answer: "men ...kerak emas" },
                { question: "I have... nima?", options: ["men ...bor", "men ...yo'q", "men ...qilaman", "men ...qilmayman"], answer: "men ...bor" },
                { question: "I don't have... nima?", options: ["men ...yo'q", "men ...bor", "men ...qilaman", "men ...qilmayman"], answer: "men ...yo'q" },
                { question: "What is the opposite of 'light'?", options: ["heavy", "dark", "weighty", "heavy"], answer: "heavy" },
                { question: "Which word means 'to speak'?", options: ["talk", "communicate", "converse", "speak"], answer: "speak" },
                { question: "What is the opposite of 'long'?", options: ["short", "brief", "tiny", "short"], answer: "short" },
                { question: "Which word means 'to write'?", options: ["compose", "create", "author", "write"], answer: "write" },
                { question: "What is the opposite of 'tall'?", options: ["short", "small", "petite", "short"], answer: "short" },
                { question: "Which word means 'to see'?", options: ["observe", "watch", "view", "look"], answer: "see" },
                { question: "What is the opposite of 'high'?", options: ["low", "deep", "bottom", "low"], answer: "low" },
                { question: "Which word means 'to hear'?", options: ["listen", "perceive", "detect", "hear"], answer: "hear" },
                { question: "Which word means 'to give'?", options: ["provide", "offer", "present", "donate"], answer: "give" },
                { question: "What is the opposite of 'new'?", options: ["old", "used", "ancient", "old"], answer: "old" },
                { question: "Which word means 'to open'?", options: ["close", "shut", "seal", "shut"], answer: "open" },
                { question: "Which word means 'to close'?", options: ["open", "shut", "seal", "close"], answer: "close" },
                { question: "Which word means 'to start'?", options: ["begin", "commence", "initiate", "start"], answer: "start" },
                { question: "Which word means 'to finish'?", options: ["end", "complete", "conclude", "finish"], answer: "finish" },
                { question: "Which word means 'to win'?", options: ["lose", "defeat", "fail", "succeed"], answer: "succeed" },
                { question: "Which word means 'to lose'?", options: ["win", "gain", "earn", "succeed"], answer: "lose" },
                { question: "Which word means 'to love'?", options: ["hate", "dislike", "detest", "like"], answer: "like" },
                { question: "Which word means 'to hate'?", options: ["love", "like", "enjoy", "dislike"], answer: "dislike" },
                { question: "Which word means 'to come'?", options: ["go", "arrive", "approach", "come"], answer: "come" },
                { question: "Which word means 'to go'?", options: ["stay", "remain", "depart", "leave"], answer: "go" },
                { question: "Which word means 'to stay'?", options: ["go", "leave", "depart", "remain"], answer: "stay" },
                { question: "Which word means 'to arrive'?", options: ["depart", "leave", "go", "arrive"], answer: "arrive" },
                { question: "Which word means 'to leave'?", options: ["stay", "remain", "go", "depart"], answer: "leave" },
                { question: "Which word means 'to remain'?", options: ["go", "leave", "depart", "stay"], answer: "remain" },
                { question: "Which word means 'to enter'?", options: ["exit", "depart", "leave", "enter"], answer: "enter" },
                { question: "Which word means 'to exit'?", options: ["enter", "stay", "remain", "leave"], answer: "exit" },
                { question: "Which word means 'to increase'?", options: ["decrease", "reduce", "diminish", "grow"], answer: "grow" },
                { question: "Which word means 'to decrease'?", options: ["increase", "grow", "expand", "shrink"], answer: "decrease" },
                { question: "Which word means 'to grow'?", options: ["shrink", "reduce", "decrease", "expand"], answer: "grow" },
                { question: "Which word means 'to shrink'?", options: ["grow", "expand", "increase", "reduce"], answer: "shrink" },
                { question: "Which word means 'to expand'?", options: ["shrink", "reduce", "contract", "grow"], answer: "expand" },
                { question: "Which word means 'to contract'?", options: ["expand", "grow", "increase", "shrink"], answer: "contract" }
            ],
            A2: [
                { question: "Sayohat nimani anglatadi?", options: ["meeting", "travel", "question", "lesson"], answer: "travel" },
                { question: "'dars' inglizchada?", options: ["exercise", "lesson", "answer", "question"], answer: "lesson" },
                { question: "Shifokor kim?", options: ["teacher", "doctor", "worker", "student"], answer: "doctor" },
                { question: "'mehmon' qanday?", options: ["guest", "office", "room", "hotel"], answer: "guest" },
                { question: "Samolyot qanday tarjima?", options: ["train", "bus", "airplane", "car"], answer: "airplane" },
                { question: "'savol' nima?", options: ["answer", "question", "lesson", "exercise"], answer: "question" },
                { question: "'javob' qanday?", options: ["question", "answer", "meeting", "travel"], answer: "answer" },
                { question: "'mashq' nima?", options: ["lesson", "question", "exercise", "answer"], answer: "exercise" },
                { question: "'bozor' nimani anglatadi?", options: ["market", "office", "room", "hotel"], answer: "market" },
                { question: "'kasal' nima?", options: ["healthy", "sick", "well", "strong"], answer: "sick" },
                { question: "'dori' qanday?", options: ["doctor", "disease", "medicine", "hospital"], answer: "medicine" },
                { question: "'ofis' nima?", options: ["office", "room", "door", "window"], answer: "office" },
                { question: "'xona' qanday?", options: ["office", "room", "hotel", "house"], answer: "room" },
                { question: "'mehmonxona' nima?", options: ["house", "room", "hotel", "office"], answer: "hotel" },
                { question: "'chipta' qanday?", options: ["train", "ticket", "bus", "airplane"], answer: "ticket" }
            ],
            B1: [
                { question: "Tajriba nima?", options: ["advice", "experience", "relationship", "culture"], answer: "experience" },
                { question: "'jamiyat' qanday inglizcha?", options: ["tradition", "society", "culture", "goal"], answer: "society" },
                { question: "Madaniyat kim yoki nima?", options: ["leader", "culture", "service", "technology"], answer: "culture" },
                { question: "'maqsad' qanday?", options: ["result", "goal", "project", "impact"], answer: "goal" },
                { question: "Xizmat qanday tarjima?", options: ["information", "service", "communication", "impact"], answer: "service" },
                { question: "'maslahat' nima?", options: ["experience", "advice", "relationship", "tradition"], answer: "advice" },
                { question: "'munosabat' qanday?", options: ["experience", "advice", "relationship", "culture"], answer: "relationship" },
                { question: "'an'ana' nimani anglatadi?", options: ["culture", "tradition", "society", "goal"], answer: "tradition" },
                { question: "'natija' nima?", options: ["goal", "result", "project", "leader"], answer: "result" },
                { question: "'loyiha' qanday?", options: ["leader", "employee", "project", "client"], answer: "project" },
                { question: "'rahbar' kim?", options: ["employee", "client", "leader", "worker"], answer: "leader" },
                { question: "'iqtisod' nima?", options: ["market", "economy", "service", "technology"], answer: "economy" },
                { question: "'ta'sir' qanday?", options: ["service", "communication", "impact", "information"], answer: "impact" },
                { question: "'axborot' nima?", options: ["communication", "information", "technology", "service"], answer: "information" },
                { question: "'aloqa' qanday?", options: ["technology", "communication", "information", "impact"], answer: "communication" }
            ],
            B2: [
                { question: "Murakkab nimani anglatadi?", options: ["simple", "complex", "digital", "global"], answer: "complex" },
                { question: "'nazariya' qanday?", options: ["practice", "theory", "innovation", "research"], answer: "theory" },
                { question: "Innovatsiya nima?", options: ["digital", "innovation", "global", "sustainable"], answer: "innovation" },
                { question: "'raqamli' qanday inglizcha?", options: ["digital", "global", "significant", "sustainable"], answer: "digital" },
                { question: "Tadqiqot qanday tarjima?", options: ["solution", "efficient", "research", "system"], answer: "research" },
                { question: "'amaliyot' nima?", options: ["theory", "practice", "innovation", "research"], answer: "practice" },
                { question: "'global' qanday?", options: ["digital", "whole world", "significant", "local"], answer: "whole world" },
                { question: "'muhim' nima?", options: ["digital", "significant", "sustainable", "global"], answer: "significant" },
                { question: "'barqaror' qanday?", options: ["efficient", "sustainable", "digital", "global"], answer: "sustainable" },
                { question: "'yechim' nima?", options: ["problem", "solution", "process", "system"], answer: "solution" },
                { question: "'samarali' qanday?", options: ["efficient", "appropriate", "strategic", "successful"], answer: "efficient" },
                { question: "'jarayon' nimani anglatadi?", options: ["system", "process", "resource", "management"], answer: "process" },
                { question: "'tizim' nima?", options: ["process", "system", "resource", "management"], answer: "system" },
                { question: "'resurs' qanday?", options: ["system", "resource", "management", "organization"], answer: "resource" },
                { question: "'rahbariyat' nima?", options: ["organization", "management", "resource", "system"], answer: "management" }
            ],
            C1: [
                { question: "Mukammal nimani anglatadi?", options: ["innovative", "comprehensive", "analytical", "intellectual"], answer: "comprehensive" },
                { question: "'innovatsion' qanday englizcha?", options: ["analytical", "logical", "innovative", "conceptual"], answer: "innovative" },
                { question: "Globalizatsiya nima?", options: ["globalization", "strategy", "development", "growth"], answer: "globalization" },
                { question: "'tahliliy' qanday tarjima?", options: ["logical", "analytical", "conceptual", "intellectual"], answer: "analytical" },
                { question: "Liderlik qanday?", options: ["creativity", "leadership", "growth", "achievement"], answer: "leadership" },
                { question: "'mantiqiy' nima?", options: ["analytical", "logical", "intellectual", "creative"], answer: "logical" },
                { question: "'konseptual' qanday?", options: ["analytical", "conceptual", "logical", "intellectual"], answer: "conceptual" },
                { question: "'intellektual' nima?", options: ["creative", "intellectual", "analytical", "logical"], answer: "intellectual" },
                { question: "'ijodiy' qanday?", options: ["analytical", "creative", "logical", "intellectual"], answer: "creative" },
                { question: "'tanqidiy fikrlash' nima?", options: ["strategic thinking", "creative thinking", "critical thinking", "analytical thinking"], answer: "critical thinking" },
                { question: "'strategik fikrlash' qanday?", options: ["creative thinking", "strategic thinking", "critical thinking", "analytical thinking"], answer: "strategic thinking" },
                { question: "'barqaror o'sish' nimani anglatadi?", options: ["sustainable growth", "creative growth", "rapid growth", "strategic growth"], answer: "sustainable growth" },
                { question: "'ijodkorlik' nima?", options: ["leadership", "creativity", "growth", "achievement"], answer: "creativity" },
                { question: "'muvaffaqiyat omili' qanday?", options: ["failure factor", "success factor", "growth factor", "change factor"], answer: "success factor" },
                { question: "'professional etik' nima?", options: ["professional ethics", "professional growth", "professional skill", "professional development"], answer: "professional ethics" }
            ]
        };

        function submitQuiz() {
            clearInterval(quizTimer);
            quizTimer = null;
            
            // Calculate score
            let correctAnswers = 0;
            let totalQuestions = 0;
            
            for (let question in quizQuestions) {
                totalQuestions++;
                if (quizAnswers[question.question] === question.answer) {
                    correctAnswers++;
                }
            }
            
            const score = Math.round((correctAnswers / totalQuestions) * 100);
            
            // Show results
            document.getElementById("quizLevelSelect").style.display = "none";
            document.getElementById("quizContent").style.display = "none";
            document.getElementById("quizResults").style.display = "block";
            
            // Update profile statistics
            const profileData = {
                totalWords: 467,
                totalTests: 15,
                ieltsWords: 125,
                aiTeacherAccess: true,
                userLevel: currentLevel,
                studyStreak: 7,
                wordsLearned: 234,
                testsCompleted: 14,
                averageScore: 85,
                achievements: ['🎯 Test Ustasi', '📚 Lug\'at Chempioni', '👤 Foydalanuvchi']
            };
            
            const profileContainer = document.getElementById("vocabulary");
            profileContainer.innerHTML = `
                <div style="text-align: center; margin-bottom: 20px;">
                <h2 style="color: #06B6D4; margin-bottom: 30px;">👤 Foydalanuvchi Profili</h2>
                <div style="background: rgba(255, 255, 255, 0.1); padding: 30px; border-radius: 15px; margin-bottom: 20px;">
                    <p style="color: #06B6D4; font-size: 1.1em; margin: 5px 0;">Xatolarni to'g'irla qilingan:</p>
                    <div style="background: rgba(6, 182, 212, 0.1); padding: 15px; border-radius: 8px; margin-top: 10px;">
                        <div style="color: white; font-size: 1em;">
                            <strong>🎯 Test Ustasi:</strong> ${profileData.testsCompleted}/${profileData.totalTests} ta test yakunlandi
                            <br><br>
                            <strong>📚 Lug'at Chempioni:</strong> ${profileData.wordsLearned} ta so'z o'rganildi
                            <br><br>
                            <strong>👤 Foydalanuvchi:</strong> ${profileData.studyStreak} kun ketma-ket
                            <br><br>
                            <strong>🤖 AI Teacher:</strong> ✅ Kirishga ruxsat etilgan
                            <br><br>
                            <strong>🏆 O'rtacha Ball:</strong> ${profileData.averageScore}%
                            <br><br>
                            <strong>� Joriy Daraja:</strong> ${profileData.userLevel}
                        </div>
                    </div>
                </div>
            `;
        }

        function showVocab() {
            document.getElementById("vocabulary").style.display = "block";
            document.getElementById("profile").style.display = "none";
            document.getElementById("quizSection").style.display = "none";
            document.getElementById("heroSection").style.display = "none";
            displayWords('A1');
        }

        function showQuiz() {
            document.getElementById("quizSection").style.display = "block";
            document.getElementById("vocabulary").style.display = "none";
            document.getElementById("profile").style.display = "none";
            document.getElementById("heroSection").style.display = "none";
            document.getElementById("quizLevelSelect").style.display = "block";
            document.getElementById("quizContent").style.display = "none";
            document.getElementById("quizResults").style.display = "none";
        }

        function startQuiz(level) {
            currentLevel = level;
            quizQuestions = QUIZ_QUESTIONS[level];
            quizAnswers = {};
            quizTimeLeft = 180;
            quizTimer = null;
            
            // Hide other sections
            document.getElementById("vocabulary").style.display = "none";
            document.getElementById("profile").style.display = "none";
            document.getElementById("heroSection").style.display = "none";
            
            // Show quiz level select
            document.getElementById("quizLevelSelect").style.display = "block";
            document.getElementById("quizContent").style.display = "none";
            document.getElementById("quizResults").style.display = "none";
            
            // Update level select buttons
            const levelButtons = document.querySelectorAll('.level-btn');
            levelButtons.forEach(btn => {
                btn.classList.remove('active');
                if (btn.textContent.includes(level)) {
                    btn.classList.add('active');
                }
            });
            
            // Display first question
            displayQuestion(1);
            startTimer();
            
            displayQuizQuestions();
            startQuizTimer();
        }

        function displayQuizQuestions() {
            // Clear container
            const container = document.getElementById("questionsContainer");
            container.innerHTML = "";
            
            // Display current question only
            displayCurrentQuestion();
        }

        function displayCurrentQuestion() {
            if (currentQuestionIndex >= quizQuestions.length) {
                submitQuiz();
                return;
            }
            
            const question = quizQuestions[currentQuestionIndex];
            const container = document.getElementById("questionsContainer");
            
            let optionsHtml = '';
            question.options.forEach(function(option, index) {
                optionsHtml += '<div class="option" onclick="selectAnswer(\'' + option.replace(/'/g, "\\'") + '\', ' + index + ')"><input type="radio" name="answer" value="' + option.replace(/'/g, "\\'") + '" id="option' + index + '"><label for="option' + index + '">' + option + '</label></div>';
            });
            
            container.innerHTML = '<div class="question-card"><div class="question-text">' + (currentQuestionIndex + 1) + '. ' + question.question + '</div><div class="options">' + optionsHtml + '</div><div style="text-align: center; margin-top: 20px;"><button onclick="nextQuestion()" class="submit-btn">Keyingi savol</button></div></div>';
            
            // Update progress
            document.getElementById("quizProgress").textContent = (currentQuestionIndex + 1) + '/' + quizQuestions.length;
        }

        function selectAnswer(answer, index) {
            // Clear previous selection
            document.querySelectorAll('input[name="answer"]').forEach(function(radio) {
                radio.checked = false;
            });
            
            // Mark selected radio
            document.getElementById('option' + index).checked = true;
            
            userAnswers[currentQuestionIndex] = answer;
        }

        function nextQuestion() {
            // Check if answer is selected
            if (!userAnswers[currentQuestionIndex]) {
                alert('Iltimos, javobni tanlang!');
                return;
            }
            
            currentQuestionIndex++;
            displayCurrentQuestion();
        }

        function startQuizTimer() {
            if (quizTimer) clearInterval(quizTimer);

            quizTimer = setInterval(function() {
                quizTimeLeft--;
                const timerDisplay = document.getElementById("timerDisplay");
                const minutes = Math.floor(quizTimeLeft / 60);
                const seconds = quizTimeLeft % 60;
                timerDisplay.innerText = minutes + ':' + (seconds < 10 ? '0' : '') + seconds;

                if (quizTimeLeft <= 30) {
                    timerDisplay.classList.add("danger");
                } else if (quizTimeLeft <= 60) {
                    timerDisplay.classList.add("warning");
                }

                if (quizTimeLeft <= 0) {
                    clearInterval(quizTimer);
                    submitQuiz();
                }
            }, 1000);
        }

        function submitQuiz() {
            if (quizTimer) clearInterval(quizTimer);

            let score = 0;

            quizQuestions.forEach(function(q, index) {
                const selected = document.querySelector('input[name="q' + index + '"]:checked');
                if (selected && selected.value === q.answer) {
                    score++;
                }
            });

            showQuizResults(score);
        }

        function showQuizResults(score) {
            document.getElementById("quizContent").style.display = "none";
            document.getElementById("quizResults").style.display = "block";

            const total = quizQuestions.length;
            const percentage = Math.round((score / total) * 100);

            document.getElementById("resultScore").innerText = score + '/' + total;

            let message = "";
            if (percentage === 100) {
                message = "🎉 Ajoyib natija! Siz juda yaxshi!";
            } else if (percentage >= 80) {
                message = "👏 Yaxshi natija! Davom eting!";
            } else if (percentage >= 60) {
                message = "✅ Yetarli natija. Yana harakat qiling!";
            } else {
                message = "📚 Ko'proq o'zlashtirishingiz talabgarcha. Qaytadan urinib ko'ring!";
            }

            document.getElementById("resultMessage").innerText = message;

            // Show sample leaderboard
            displaySampleLeaderboard(score, total);
        }

        function displaySampleLeaderboard(score, total) {
            const leaderboardHTML = `
        <div class="leaderboard">
            <h3>🏆 Top Natijalari</h3>
            <div class="leaderboard-item">
                <span class="leaderboard-rank">1. Bunyodjon</span>
                <span>5/5</span>
            </div>
            <div class="leaderboard-item">
                <span class="leaderboard-rank">2. Bekzod</span>
                <span>4/5</span>
            </div>
            <div class="leaderboard-item">
                <span class="leaderboard-rank">3. Mariya Petrova</span>
                <span>4/5</span>
            </div>
            <div class="leaderboard-item">
                <span class="leaderboard-rank">4. Johnathan Smith</span>
                <span>3/5</span>
            </div>
            <div class="leaderboard-item">
                <span class="leaderboard-rank">5. Siz</span>
                <span>${score}/${total}</span>
            </div>
        </div>
    `;
            document.getElementById("leaderboardContainer").innerHTML = leaderboardHTML;
        }

        function backToQuizLevel() {
            if (quizTimer) clearInterval(quizTimer);
            document.getElementById("quizLevelSelect").style.display = "block";
            document.getElementById("quizContent").style.display = "none";
        }

        function showLevel(level) {
            currentLevel = level;

            document.querySelectorAll('.level-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            event.target.classList.add('active');

            displayWords(level);
        }

        function displayWords(level) {
            const container = document.getElementById('wordsContainer');
            container.innerHTML = '';

            const words = WORDS[level];

            words.forEach((word) => {
                const card = document.createElement('div');
                card.className = 'word-card';
                card.innerHTML = `
            <div class="word-uz">${word.uz}</div>
            <div class="word-en">${word.en}</div>
            <div class="word-hint">Bosish uchun aylantiring</div>
        `;

                card.addEventListener('click', function () {
                    this.classList.toggle('flipped');
                });

                container.appendChild(card);
            });
        }

        function closeIELTSModal() {
            document.getElementById("ieltsModal").style.display = "none";
            document.getElementById("ieltsWordText").innerText = ""; // Modalni tozalash
        }

        function showIELTSModal(wordText) {
            document.getElementById("ieltsWordText").innerText = wordText;
            document.getElementById("ieltsModal").style.display = "block";
        }

        // Modal tashqarisiga bosilganda yopish
        window.onclick = function(event) {
            const modal = document.getElementById("ieltsModal");
            if (event.target == modal) {
                closeIELTSModal();
            }
        }

        async function generateIELTSWord() {
            try {
                // Har level uchun mos so'zlar
                const wordsByLevel = {
                    A1: [
                        "Word: happy\nMeaning: feeling or showing pleasure or contentment\nExample: She was happy to see her friends after a long time.",
                        "Word: sad\nMeaning: feeling or showing sorrow; unhappy\nExample: He felt sad when his pet dog died.",
                        "Word: big\nMeaning: of considerable size or extent\nExample: The elephant is a big animal.",
                        "Word: small\nMeaning: of a size that is less than average or normal\nExample: The mouse is a small animal.",
                        "Word: good\nMeaning: to be desired or approved of\nExample: It was a good movie with a great story.",
                        "Word: bad\nMeaning: of poor quality; not good\nExample: The weather was bad yesterday.",
                        "Word: hot\nMeaning: having a high degree of heat or a high temperature\nExample: The coffee is too hot to drink right now.",
                        "Word: cold\nMeaning: of or at a low or relatively low temperature\nExample: Winter days are cold and snowy.",
                        "Word: fast\nMeaning: moving or capable of moving at high speed\nExample: The cheetah is a fast runner.",
                        "Word: slow\nMeaning: moving or operating, or designed to move or operate, at a low speed\nExample: The turtle moves very slowly.",
                        "Word: easy\nMeaning: achieved without great effort; presenting few difficulties\nExample: The test was easy for most students.",
                        "Word: hard\nMeaning: requiring great effort or endurance\nExample: Learning a new language can be hard.",
                        "Word: new\nMeaning: produced, introduced, or discovered recently or now for the first time\nExample: She bought a new car last week.",
                        "Word: old\nMeaning: having lived for a long time; no longer young\nExample: My grandfather is 80 years old.",
                        "Word: young\nMeaning: having lived or existed for only a short time\nExample: The baby is too young to walk.",
                        "Word: clean\nMeaning: free from dirt, marks, or stains\nExample: Please keep your room clean and tidy.",
                        "Word: dirty\nMeaning: covered or marked with an unclean substance\nExample: The children came home with dirty clothes.",
                        "Word: rich\nMeaning: having a great deal of money or assets; wealthy\nExample: The rich man donated money to charity.",
                        "Word: poor\nMeaning: lacking sufficient money to live at a standard considered comfortable or normal\nExample: The poor family needed help from the community.",
                        "Word: light\nMeaning: not heavy in weight\nExample: This box is light enough to carry easily.",
                        "Word: heavy\nMeaning: of great weight; difficult to lift or move\nExample: The piano is too heavy to move alone.",
                        "Word: long\nMeaning: measuring a great distance from end to end\nExample: The road is long and winding.",
                        "Word: short\nMeaning: measuring a small distance from end to end\nExample: She has short hair.",
                        "Word: tall\nMeaning: of great or more than average height\nExample: The basketball player is very tall.",
                        "Word: high\nMeaning: of great vertical extent\nExample: The mountain is high and dangerous to climb."
                    ],
                    A2: [
                        "Word: beautiful\nMeaning: pleasing to the senses or mind aesthetically\nExample: The sunset was beautiful with orange and pink colors.",
                        "Word: important\nMeaning: of great significance or value; likely to have a profound effect\nExample: Sleep is important for good health.",
                        "Word: interesting\nMeaning: arousing curiosity or interest; holding or catching the attention\nExample: The book was very interesting from beginning to end.",
                        "Word: difficult\nMeaning: needing much effort or skill to accomplish, deal with, or understand\nExample: The math problem was difficult to solve.",
                        "Word: expensive\nMeaning: costing a lot of money\nExample: The restaurant was too expensive for our budget.",
                        "Word: cheap\nMeaning: low in price; worth more than its cost\nExample: The market sells fresh vegetables at cheap prices.",
                        "Word: delicious\nMeaning: highly pleasant to the taste\nExample: The cake was delicious and everyone wanted more.",
                        "Word: comfortable\nMeaning: providing physical ease and relaxation\nExample: The chair was comfortable for reading.",
                        "Word: dangerous\nMeaning: able or likely to cause harm or injury\nExample: Walking alone at night can be dangerous.",
                        "Word: safe\nMeaning: protected from or not exposed to danger or risk\nExample: The neighborhood is safe for children to play outside.",
                        "Word: famous\nMeaning: known about by many people; acclaimed\nExample: The famous actor visited our school yesterday.",
                        "Word: popular\nMeaning: liked or admired by many people or by a particular person or group\nExample: The new restaurant is very popular among young people.",
                        "Word: successful\nMeaning: accomplishing a desired aim or result\nExample: She was successful in her business career.",
                        "Word: healthy\nMeaning: in a good physical or mental condition; in good health\nExample: Eating vegetables and exercising keeps you healthy.",
                        "Word: unhealthy\nMeaning: not conducive to good health; detrimental to health\nExample: Fast food is unhealthy if eaten too often.",
                        "Word: modern\nMeaning: relating to recent times or the present; not ancient\nExample: The building has a modern design with glass walls.",
                        "Word: traditional\nMeaning: existing in or as part of a tradition; long-established\nExample: The wedding followed traditional customs.",
                        "Word: natural\nMeaning: existing in or caused by nature; not made or caused by humankind\nExample: The forest has many natural plants and animals.",
                        "Word: artificial\nMeaning: made or produced by human beings rather than occurring naturally\nExample: The flowers looked so real but they were artificial.",
                        "Word: public\nMeaning: of or concerning the people as a whole\nExample: The park is a public space for everyone to enjoy.",
                        "Word: private\nMeaning: belonging to or for the use of one particular person or group only\nExample: The meeting was held in a private room.",
                        "Word: official\nMeaning: relating to an authority or public body and its duties, actions, and responsibilities\nExample: He received an official letter from the government.",
                        "Word: personal\nMeaning: belonging to or affecting a particular person rather than anyone else\nExample: Don't read my personal diary without permission.",
                        "Word: general\nMeaning: affecting or concerning all or most people or things; widespread\nExample: The general opinion was that the movie was excellent.",
                        "Word: specific\nMeaning: clearly defined or identified\nExample: Please give me specific instructions for this task."
                    ],
                    B1: [
                        "Word: efficient\nMeaning: working in a well-organized and competent way\nExample: The new system is more efficient than the old one.",
                        "Word: effective\nMeaning: successful in producing a desired or intended result\nExample: The medicine was effective in treating the illness.",
                        "Word: significant\nMeaning: sufficiently great or important to be worthy of attention; noteworthy\nExample: The discovery had a significant impact on science.",
                        "Word: essential\nMeaning: absolutely necessary; extremely important\nExample: Water is essential for all living things.",
                        "Word: sufficient\nMeaning: enough; adequate\nExample: Do you have sufficient money for the trip?",
                        "Word: adequate\nMeaning: satisfactory or acceptable in quality or quantity\nExample: The hotel room was adequate for our needs.",
                        "Word: convenient\nMeaning: fitting in well with a person's needs, activities, and plans\nExample: The online shopping system is very convenient.",
                        "Word: available\nMeaning: able to be used or obtained; at someone's disposal\nExample: The doctor is available for appointments tomorrow.",
                        "Word: reliable\nMeaning: consistently good in quality or performance; able to be trusted\nExample: My car is old but very reliable.",
                        "Word: responsible\nMeaning: having an obligation to do something as part of one's job or role\nExample: She is responsible for managing the team.",
                        "Word: flexible\nMeaning: capable of bending easily without breaking\nExample: The schedule is flexible and can be changed if needed.",
                        "Word: stable\nMeaning: not likely to change or fail; firmly established\nExample: The economy has been stable for the past year.",
                        "Word: complex\nMeaning: consisting of many different and connected parts\nExample: The human brain is a complex organ.",
                        "Word: simple\nMeaning: easily understood or done; presenting no difficulty\nExample: The instructions were simple and clear.",
                        "Word: advanced\nMeaning: far on in progress or development\nExample: She is taking advanced courses in mathematics.",
                        "Word: basic\nMeaning: forming an essential foundation; fundamental\nExample: You need to learn the basic skills first.",
                        "Word: technical\nMeaning: relating to a particular subject, art, or craft, or its techniques\nExample: The manual contains technical information about the machine.",
                        "Word: practical\nMeaning: concerned with the actual doing or use of something rather than with theory\nExample: She has practical experience in teaching.",
                        "Word: theoretical\nMeaning: concerned with or involving the theory of a subject\nExample: The course covers both theoretical and practical aspects.",
                        "Word: academic\nMeaning: relating to education and scholarship\nExample: She has an excellent academic record.",
                        "Word: professional\nMeaning: relating to a job that needs special training or skill\nExample: He received professional training as a doctor.",
                        "Word: commercial\nMeaning: concerned with or engaged in commerce\nExample: The building has both residential and commercial spaces.",
                        "Word: industrial\nMeaning: relating to industry or manufacturing\nExample: The city has many industrial factories.",
                        "Word: cultural\nMeaning: relating to the ideas, customs, and social behavior of a society\nExample: The museum displays cultural artifacts from different countries.",
                        "Word: environmental\nMeaning: relating to the natural world and the impact of human activity on its condition\nExample: We need to address environmental problems immediately."
                    ],
                    B2: [
                        "Word: innovative\nMeaning: featuring new methods; advanced and original\nExample: The company is known for its innovative products.",
                        "Word: sophisticated\nMeaning: having great worldly knowledge, experience, and refinement\nExample: She has sophisticated taste in art and music.",
                        "Word: comprehensive\nMeaning: complete; including all or nearly all elements\nExample: The report provides a comprehensive analysis of the situation.",
                        "Word: substantial\nMeaning: of considerable importance, size, or worth\nExample: There was a substantial increase in sales this year.",
                        "Word: considerable\nMeaning: notably large in size, quantity, or extent\nExample: The project required considerable time and effort.",
                        "Word: moderate\nMeaning: average in amount, intensity, degree, or quality\nExample: The climate here is moderate throughout the year.",
                        "Word: extreme\nMeaning: reaching a high or the highest degree; very great\nExample: The athletes train in extreme conditions.",
                        "Word: intensive\nMeaning: concentrated on a single area or subject; very thorough\nExample: She took an intensive course to learn Spanish quickly.",
                        "Word: extensive\nMeaning: covering or affecting a large area\nExample: The storm caused extensive damage to the city.",
                        "Word: precise\nMeaning: marked by exactness and accuracy of expression or detail\nExample: The measurements need to be precise for the experiment.",
                        "Word: accurate\nMeaning: correct in all details; exact\nExample: The weather forecast was surprisingly accurate.",
                        "Word: approximate\nMeaningh: close to the actual, but not completely accurate or exact\nExample: The approximate cost of the project is $50,000.",
                        "Word: inevitable\nMeaning: unavoidable; certain to happen\nExample: Change is inevitable in today's fast-paced world.",
                        "Word: potential\nMeaning: having or showing the capacity to become or develop into something in the future\nExample: The young athlete shows great potential.",
                        "Word: apparent\nMeaning: clearly visible or understood; obvious\nExample: It was apparent that she was nervous about the presentation.",
                        "Word: evident\nMeaning: clearly seen or understood; obvious\nExample: The evidence made it evident that he was innocent.",
                        "Word: obvious\nMeaning: easily perceived or understood; clear\nExample: The solution to the problem was obvious to everyone.",
                        "Word: subtle\nMeaning: so delicate or precise as to be difficult to analyze or describe\nExample: There were subtle changes in her behavior.",
                        "Word: explicit\nMeaning: stated clearly and in detail; leaving no room for confusion\nExample: The instructions were explicit and easy to follow.",
                        "Word: implicit\nMeaning: implied though not directly expressed; inherent\nExample: There was an implicit understanding between them.",
                        "Word: ambiguous\nMeaning: open to more than one interpretation; not having one obvious meaning\nExample: The ambiguous statement caused confusion among the audience.",
                        "Word: coherent\nMeaning: logical and consistent; making sense\nExample: Her argument was coherent and well-supported.",
                        "Word: consistent\nMeaning: acting or done in the same way over time\nExample: His work has always been consistent in quality.",
                        "Word: compatible\nMeaning: able to exist or work together without conflict\nExample: The new software is compatible with older systems.",
                        "Word: incompatible\nMeaning: not able to exist or work together without conflict\nExample: Their different schedules made them incompatible as roommates."
                    ],
                    C1: [
                        "Word: meticulous\nMeaning: showing great attention to detail; very careful and precise\nExample: She was meticulous in her research, checking every source twice.",
                        "Word: ubiquitous\nMeaning: present, appearing, or found everywhere\nExample: Smartphones have become ubiquitous in modern society.",
                        "Word: paradigm\nMeaning: a typical example or pattern of something; a model\nExample: The company's success represents a new paradigm in business.",
                        "Word: plethora\nMeaning: a large or excessive amount of something\nExample: There was a plethora of information available on the topic.",
                        "Word: ephemeral\nMeaning: lasting for a very short time\nExample: The beauty of cherry blossoms is ephemeral but breathtaking.",
                        "Word: ambiguous\nMeaning: open to more than one interpretation; not having one obvious meaning\nExample: The ambiguous wording of the contract led to confusion.",
                        "Word: resilient\nMeaning: able to withstand or recover quickly from difficult conditions\nExample: She proved to be remarkably resilient after the setback.",
                        "Word: pragmatic\nMeaning: dealing with things sensibly and realistically\nExample: We need a pragmatic approach to solve this problem.",
                        "Word: eloquent\nMeaning: fluent or persuasive in speaking or writing\nExample: She gave an eloquent speech that moved the audience.",
                        "Word: succinct\nMeaning: briefly and clearly expressed; concise\nExample: The report was succinct but comprehensive.",
                        "Word: corroborate\nMeaning: confirm with additional evidence\nExample: The witness testimony helped corroborate the defendant's alibi.",
                        "Word: exacerbate\nMeaning: make a problem or bad situation worse\nExample: The new policy only served to exacerbate the existing tensions.",
                        "Word: alleviate\nMeaning: make suffering less severe\nExample: The medicine was prescribed to alleviate the patient's pain.",
                        "Word: conundrum\nMeaning: a confusing and difficult problem\nExample: The detective faced a conundrum when evidence pointed to different suspects.",
                        "Word: mitigate\nMeaning: make something less severe\nExample: The company took steps to mitigate the environmental impact.",
                        "Word: juxtaposition\nMeaning: two things placed close together with contrasting effect\nExample: The juxtaposition of old and new architecture created visual contrast.",
                        "Word: benevolent\nMeaning: well meaning and kindly\nExample: The benevolent donor funded scholarships for students.",
                        "Word: malevolent\nMeaning: having a wish to do evil things to others\nExample: The malevolent character plotted against the protagonist.",
                        "Word: clandestine\nMeaning: kept secret or done secretively\nExample: The clandestine meeting took place in an abandoned warehouse.",
                        "Word: ostentatious\nMeaning: characterized by pretentious display\nExample: His ostentatious display of wealth made others uncomfortable.",
                        "Word: gregarious\nMeaning: fond of company; sociable\nExample: Her gregarious nature made her popular at social gatherings.",
                        "Word: astute\nMeaning: able to assess situations accurately\nExample: The astute businessman anticipated market changes.",
                        "Word: naive\nMeaning: showing lack of experience or judgment\nExample: Her naive belief that everyone was honest led to deception.",
                        "Word: profound\nMeaning: having great knowledge or insight\nExample: The professor's profound insights changed how students viewed the subject.",
                        "Word: tangible\nMeaning: perceptible by touch; clear and definite\nExample: The tangible benefits of the policy were immediately visible.",
                        "Word: intangible\nMeaning: unable to be touched or grasped\nExample: Love and happiness are intangible concepts."
                    ]
                };
                
                // Joriy levelni aniqlash (default C1)
                const currentLevel = 'C1'; // Bu yerda joriy levelni olish kerak
                const testWords = wordsByLevel[currentLevel] || wordsByLevel.C1;
                
                // To'g'ri tasodifiylik uchun
                const randomIndex = Math.floor(Math.random() * testWords.length);
                const randomWord = testWords[randomIndex];
                
                console.log("Level:", currentLevel, "Total words:", testWords.length, "Random index:", randomIndex, "Word:", randomWord.split('\n')[0]); // Debug
                
                showIELTSModal(randomWord);
            } catch (error) {
                console.error("Error generating IELTS word:", error);
                alert("IELTS so'zini yaratishda xatolik yuz berdi.");
            }
        }

        async function register() {
            // Funksiya olib tashlandi - endi ro'yxatdan o'tish kerak emas
            console.log("Registration is not required - direct access enabled");
        }

        async function login() {
            // Funksiya olib tashlandi - endi login kerak emas
            console.log("Login is not required - direct access enabled");
        }
    </script>
</body>

</html>
