<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vinh Danh Học Sinh Xuất Sắc - 20 Năm học</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;800;900&display=swap" rel="stylesheet">
    <style>
        /* ===== RESET & BASE STYLES ===== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Quicksand', sans-serif;
        }
        
        :root {
            --primary-color: #1a2a6c;
            --secondary-color: #2A4D9B;
            --accent-color: #3a6dc9;
            --gold-color: #FFD700;
            --gold-light: #FFEC8B;
            --orange-color: #FF8C42;
            --text-light: #F8F6F2;
            --text-dark: #0a192f;
            --shadow-light: rgba(255, 255, 255, 0.1);
            --shadow-dark: rgba(0, 0, 0, 0.3);
            --gradient-primary: linear-gradient(135deg, #1a2a6c, #2A4D9B, #3a6dc9);
            --gradient-gold: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            --gradient-card: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            --gradient-orange: linear-gradient(135deg, rgba(255, 140, 66, 0.9), rgba(232, 106, 51, 0.9));
            --transition-slow: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            --transition-medium: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            --transition-fast: all 0.3s ease;
        }
        
        body {
            background: var(--gradient-primary);
            color: var(--text-light);
            min-height: 100vh;
            overflow-x: hidden;
            position: relative;
        }
        
        /* ===== BACKGROUND EFFECTS ===== */
        .dynamic-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -3;
            background: linear-gradient(-45deg, #1a2a6c, #2A4D9B, #3a6dc9, #4d8ae6, #1a2a6c);
            background-size: 400% 400%;
            animation: gradientShift 20s ease infinite;
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -2;
            overflow: hidden;
        }
        
        .particle {
            position: absolute;
            background: radial-gradient(circle, rgba(255, 215, 0, 0.7) 0%, rgba(255, 215, 0, 0) 70%);
            border-radius: 50%;
            animation: particleFloat 25s infinite linear;
            filter: blur(1px);
        }
        
        @keyframes particleFloat {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .floating-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .floating-element {
            position: absolute;
            background: rgba(255, 215, 0, 0.1);
            border-radius: 50%;
            animation: float 25s infinite linear;
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.3);
        }
        
        @keyframes float {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-1000px) rotate(360deg);
                opacity: 0;
            }
        }
        
        .spotlight {
            position: fixed;
            width: 300px;
            height: 300px;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(255,215,0,0.2) 0%, rgba(255,215,0,0) 70%);
            pointer-events: none;
            z-index: -1;
            animation: spotlightMove 20s infinite linear;
            filter: blur(15px);
        }
        
        @keyframes spotlightMove {
            0% { transform: translate(10vw, 10vh); }
            25% { transform: translate(80vw, 30vh); }
            50% { transform: translate(40vw, 70vh); }
            75% { transform: translate(70vw, 50vh); }
            100% { transform: translate(10vw, 10vh); }
        }
        
        /* ===== CONTAINER & LAYOUT ===== */
        .container {
            width: 100%;
            min-height: 100vh;
            background: rgba(10, 25, 47, 0.85);
            backdrop-filter: blur(20px);
            position: relative;
            overflow: hidden;
        }
        
        .container::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="50" cy="50" r="1" fill="rgba(255,255,255,0.03)"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>'),
                linear-gradient(135deg, transparent 0%, rgba(255, 215, 0, 0.05) 100%);
            pointer-events: none;
            z-index: 0;
        }
        
        /* ===== HEADER STYLES ===== */
        header {
            background: 
                linear-gradient(135deg, rgba(42, 77, 155, 0.9), rgba(58, 109, 201, 0.8)),
                url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 L100,0 L100,100 Z" fill="rgba(255,215,0,0.1)"/></svg>');
            color: var(--text-light);
            text-align: center;
            padding: 120px 20px 100px;
            position: relative;
            overflow: hidden;
            border-bottom: 1px solid rgba(255, 215, 0, 0.3);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 80%, rgba(255, 215, 0, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(255, 215, 0, 0.1) 0%, transparent 50%);
            z-index: 1;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        .header-logo {
            position: absolute;
            top: 30px;
            left: 50px;
            height: 180px;
            width: auto;
            z-index: 10;
            filter: drop-shadow(0 0 15px rgba(255, 215, 0, 0.7));
            transition: var(--transition-medium);
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            padding: 10px;
            backdrop-filter: blur(10px);
        }
        
        .header-logo:hover {
            transform: scale(1.1) rotate(5deg);
            filter: drop-shadow(0 0 20px rgba(255, 215, 0, 0.9));
        }
        
        .header-icon {
            font-size: 4rem;
            color: var(--gold-color);
            margin-bottom: 30px;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.7);
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
        
        .glowing-text {
            font-size: 5rem;
            margin-bottom: 20px;
            text-shadow: 0 0 10px rgba(254 , 224 , 255 , 0 ), 0 0 20px rgba(255, 215, 0, 0.5), 0 0 30px rgba(255, 215, 0, 0 );
            position: relative;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
            letter-spacing: 2px;
            animation: glow 3s ease-in-out infinite alternate;
            font-family: 'Playfair Display', serif;
        }
        
        @keyframes glow {
            0% {
                text-shadow: 0 0 10px rgba(255, 215, 0, 0), 0 0 20px rgba(255, 215, 0, 0.5), 0 0 30px rgba(255, 215, 0, 0 );
            }
            100% {
                text-shadow: 0 0 15px rgba(255, 215, 0, 0.8), 0 0 25px rgba(255, 215, 0, 0.6), 0 0 35px rgba(255, 215, 0, 0.4);
            }
        }
        
        .subtitle {
            font-size: 2.2rem;
            margin-bottom: 10px;
            position: relative;
            color: #e0e0ff;
            font-weight: 500;
        }
        
        .header-decoration {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 20px;
            background: linear-gradient(90deg, transparent, var(--gold-color), transparent);
            opacity: 0.5;
        }
        
        /* ===== MAIN CONTENT STYLES ===== */
        .main-content {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 80vh;
            padding: 80px 20px;
            flex-direction: column;
            gap: 100px;
        }
        
        .section-title {
            font-size: 3.5rem;
            text-align: center;
            margin-bottom: 60px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
            position: relative;
            display: inline-block;
            padding: 0 20px;
            font-family: 'Playfair Display', serif;
        }
        
        .section-title::after {
            content: "";
            position: absolute;
            bottom: -15px;
            left: 20%;
            width: 60%;
            height: 4px;
            background: linear-gradient(90deg, transparent, #FFD700, transparent);
            border-radius: 2px;
        }
        
        .section-title i {
            margin-right: 15px;
            font-size: 3rem;
            vertical-align: middle;
        }
        
        /* ===== YEAR CARDS STYLES ===== */
        .large-years {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 50px;
            width: 100%;
            max-width: 1600px;
        }
        
        .large-year {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            border-radius: 25px;
            width: 320px;
            height: 380px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: 2.8rem;
            font-weight: bold;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3), 0 0 25px rgba(255, 215, 0, 0.2);
            cursor: pointer;
            text-align: center;
            padding: 30px;
            position: relative;
            overflow: hidden;
        }
        
        .large-year::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.1), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.8s;
        }
        
        .large-year:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .large-year:hover {
            transform: translateY(-15px) scale(1.05);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4), 0 0 40px rgba(255, 215, 0, 0.4);
        }
        
        .large-year .year-icon {
            font-size: 7rem;
            margin-bottom: 30px;
            color: #FFD700;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 10px rgba(255, 215, 0, 0.5));
            transition: all 0.4s;
        }
        
        .large-year:hover .year-icon {
            transform: scale(1.2) rotate(10deg);
            filter: drop-shadow(0 0 15px rgba(255, 215, 0, 0.8));
        }
        
        .large-year .year-period {
            font-size: 3rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .large-year .year-label {
            font-size: 1.6rem;
            opacity: 0.9;
            color: #e0e0ff;
            font-weight: 500;
        }
        
        /* ===== MASTERS/PHD BUTTON STYLES ===== */
        .masters-phd-section {
            width: 100%;
            text-align: center;
            margin-top: 30px;
        }
        
        .masters-phd-button {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.9), rgba(232, 106, 51, 0.9));
            border-radius: 35px;
            width: 650px;
            height: 240px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            font-weight: bold;
            border: 4px solid rgba(255, 215, 0, 0.7);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.5), 0 0 40px rgba(255, 140, 66, 0.6);
            cursor: pointer;
            text-align: center;
            padding: 40px;
            margin: 0 auto;
            position: relative;
            overflow: hidden;
        }
        
        .masters-phd-button::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.2), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.8s;
        }
        
        .masters-phd-button:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .masters-phd-button:hover {
            transform: translateY(-15px) scale(1.1);
            box-shadow: 0 35px 70px rgba(0, 0, 0, 0.6), 0 0 60px rgba(255, 140, 66, 0.8);
        }
        
        .masters-phd-button .button-icon {
            font-size: 5.5rem;
            margin-bottom: 20px;
            color: #FFD700;
            text-shadow: 0 0 30px rgba(255, 215, 0, 0.9);
            filter: drop-shadow(0 0 20px rgba(255, 215, 0, 0.7));
            transition: all 0.4s;
        }
        
        .masters-phd-button:hover .button-icon {
            transform: scale(1.3) rotate(15deg);
            filter: drop-shadow(0 0 25px rgba(255, 215, 0, 1));
        }
        
        .masters-phd-button .button-text {
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 800;
            letter-spacing: 1px;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            line-height: 1.2;
        }
        
        /* ===== YEAR BUTTONS CONTAINER ===== */
        .year-buttons-container {
            display: none;
            flex-direction: column;
            align-items: center;
            margin-top: 40px;
            padding: 40px 20px;
            background: rgba(20, 40, 80, 0.9);
            border-radius: 0;
            width: 100%;
            min-height: 100vh;
            border: none;
            box-shadow: none;
        }
        
        .year-buttons-title {
            font-size: 3rem;
            margin-bottom: 40px;
            text-align: center;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .year-buttons {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 25px;
            width: 100%;
            max-width: 1200px;
        }
        
        .year-button {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            border-radius: 15px;
            padding: 25px 35px;
            font-size: 1.8rem;
            font-weight: bold;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3), 0 0 15px rgba(255, 215, 0, 0.2);
            cursor: pointer;
            min-width: 180px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .year-button::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.1), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.6s;
        }
        
        .year-button:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .year-button:hover {
            transform: scale(1.08);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 25px rgba(255, 215, 0, 0.4);
        }
        
        /* ===== BUTTON STYLES ===== */
        .back-button {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.9), rgba(232, 106, 51, 0.9));
            margin-top: 40px;
            padding: 18px 35px;
            border-radius: 12px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            color: #F8F6F2;
            font-size: 1.5rem;
            transition: all 0.4s;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .back-button:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 20px rgba(255, 140, 66, 0.5);
        }
        
        /* ===== STUDENT PAGE STYLES ===== */
        .student-page {
            display: none;
            padding: 60px 20px;
            text-align: center;
            min-height: 100vh;
            width: 100%;
        }
        
        .student-page h2 {
            font-size: 3.5rem;
            margin-bottom: 50px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
        }
        
        .students-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 35px;
            margin-top: 40px;
            width: 100%;
            max-width: 1400px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .student-card {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.7), rgba(42, 77, 155, 0.8));
            border-radius: 20px;
            padding: 35px;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            min-height: 420px;
            justify-content: space-between;
            position: relative;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3);
        }
        
        .student-card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.1), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.8s;
        }
        
        .student-card:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .student-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4), 0 0 30px rgba(255, 215, 0, 0.4);
        }
        
        .student-image {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 215, 0, 0.5);
            margin-bottom: 25px;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.4);
        }
        
        .student-card h3 {
            font-size: 2rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .student-card p {
            margin-bottom: 10px;
            font-size: 1.3rem;
            color: #e0e0ff;
        }
        
        .student-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #FFD700;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 8px rgba(255, 215, 0, 0.5));
        }
        
        .back-to-years {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.9), rgba(42, 77, 155, 0.9));
            margin-top: 50px;
            padding: 18px 40px;
            border-radius: 12px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            color: #F8F6F2;
            font-size: 1.5rem;
            transition: all 0.4s;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .back-to-years:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 20px rgba(58, 109, 201, 0.5);
        }
        
        /* ===== MASTERS/PHD PAGE STYLES ===== */
        .masters-phd-page {
            display: none;
            padding: 60px 20px;
            text-align: center;
            min-height: 100vh;
            width: 100%;
        }
        
        .masters-phd-page h2 {
            font-size: 3.5rem;
            margin-bottom: 50px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
        }
        
        .graduates-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(400px, 1fr));
            gap: 40px;
            margin-top: 40px;
            width: 100%;
            max-width: 1400px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .graduate-card {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.7), rgba(232, 106, 51, 0.8));
            border-radius: 20px;
            padding: 40px;
            border: 2px solid rgba(255, 215, 0, 0.5);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            min-height: 480px;
            justify-content: space-between;
            position: relative;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3);
        }
        
        .graduate-card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(45deg, transparent, rgba(255,255,255,0.15), transparent);
            transform: translateX(-100%) skewX(-15deg);
            transition: transform 0.8s;
        }
        
        .graduate-card:hover::before {
            transform: translateX(100%) skewX(-15deg);
        }
        
        .graduate-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.4), 0 0 30px rgba(255, 140, 66, 0.6);
        }
        
        .graduate-image {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 215, 0, 0.6);
            margin-bottom: 25px;
            box-shadow: 0 0 25px rgba(255, 215, 0, 0.5);
        }
        
        .graduate-card h3 {
            font-size: 2.2rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .degree-badge {
            background: linear-gradient(135deg, #FF8C42, #E86A33);
            padding: 10px 25px;
            border-radius: 25px;
            font-weight: bold;
            margin-bottom: 20px;
            font-size: 1.4rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            border: 1px solid rgba(255, 215, 0, 0.5);
        }
        
        .graduate-card p {
            margin-bottom: 12px;
            font-size: 1.3rem;
            color: #fff;
        }
        
        .graduate-icon {
            font-size: 3.5rem;
            margin-bottom: 25px;
            color: #FFD700;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 10px rgba(255, 215, 0, 0.5));
        }
        
        .back-to-main {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.9), rgba(42, 77, 155, 0.9));
            margin-top: 50px;
            padding: 18px 40px;
            border-radius: 12px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            color: #F8F6F2;
            font-size: 1.5rem;
            transition: all 0.4s;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .back-to-main:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 20px rgba(58, 109, 201, 0.5);
        }
        
        /* ===== MODAL STYLES ===== */
        .detail-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            z-index: 1000;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .modal-content {
            background: linear-gradient(135deg, rgba(20, 40, 80, 0.95), rgba(42, 77, 155, 0.95));
            border-radius: 25px;
            padding: 40px;
            max-width: 800px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            position: relative;
            box-shadow: 0 25px 60px rgba(0, 0, 0, 0.6);
            border: 2px solid rgba(255, 215, 0, 0.5);
            animation: modalAppear 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        
        @keyframes modalAppear {
            0% {
                opacity: 0;
                transform: scale(0.8) translateY(-50px);
            }
            100% {
                opacity: 1;
                transform: scale(1) translateY(0);
            }
        }
        
        .close-modal {
            position: absolute;
            top: 20px;
            right: 25px;
            font-size: 2.5rem;
            cursor: pointer;
            color: #FFD700;
            transition: transform 0.3s;
            text-shadow: 0 0 10px rgba(255, 215, 0, 0.7);
        }
        
        .close-modal:hover {
            transform: scale(1.2) rotate(90deg);
        }
        
        .modal-header {
            text-align: center;
            margin-bottom: 30px;
        }
        
        .modal-header h3 {
            font-size: 2.5rem;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 15px;
            font-weight: 700;
        }
        
        .modal-body {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 25px;
        }
        
        .modal-image {
            width: 220px;
            height: 220px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid rgba(255, 215, 0, 0.6);
            box-shadow: 0 0 30px rgba(255, 215, 0, 0.5);
        }
        
        .modal-info {
            width: 100%;
            text-align: left;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255, 215, 0, 0.3);
        }
        
        .modal-info p {
            margin-bottom: 12px;
            font-size: 1.3rem;
            padding: 8px 0;
            border-bottom: 1px solid rgba(255, 215, 0, 0.2);
        }
        
        .modal-info strong {
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        /* ===== FOOTER STYLES ===== */
        footer {
            text-align: center;
            padding: 40px;
            background: rgba(15, 30, 60, 0.8);
            color: #b0b0ff;
            border-top: 1px solid rgba(255, 215, 0, 0.2);
            font-size: 1.2rem;
        }
        
        .footer-text {
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 600;
        }
        
        /* ===== ENHANCED STYLES ===== */
        .enhanced-card {
            position: relative;
            overflow: hidden;
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        
        .enhanced-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.7s;
        }
        
        .enhanced-card:hover::before {
            left: 100%;
        }
        
        .enhanced-card:hover {
            transform: translateY(-10px) scale(1.03);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4), 0 0 40px rgba(255, 215, 0, 0.5);
        }
        
        .page-transition {
            animation: pageFadeIn 0.8s ease-out;
        }
        
        @keyframes pageFadeIn {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .loading-spinner {
            display: none;
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 9999;
        }
        
        .spinner {
            width: 70px;
            height: 70px;
            border: 7px solid rgba(255, 215, 0, 0.3);
            border-radius: 50%;
            border-top-color: #FFD700;
            animation: spin 1s linear infinite;
        }
        
        @keyframes spin {
            100% { transform: rotate(360deg); }
        }
        
        .typewriter {
            overflow: hidden;
            border-right: .15em solid #FFD700;
            white-space: nowrap;
            margin: 0 auto;
            animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #FFD700; }
        }
        
        .image-3d {
            transition: transform 0.5s ease;
            transform-style: preserve-3d;
        }
        
        .image-3d:hover {
            transform: perspective(1000px) rotateY(10deg) rotateX(5deg) scale(1.05);
        }
        
        .magic-button {
            position: relative;
            overflow: hidden;
        }
        
        .magic-button::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: conic-gradient(from 0deg, transparent, rgba(255,215,0,0.5), transparent);
            animation: rotate 3s linear infinite;
        }
        
        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .magic-button:hover::after {
            animation-duration: 1s;
        }
        
        /* ===== RESPONSIVE STYLES ===== */
        @media (max-width: 1200px) {
            .large-years {
                gap: 30px;
            }
            
            .large-year {
                width: 280px;
                height: 340px;
            }
            
            .large-year .year-period {
                font-size: 2.5rem;
            }
            
            .masters-phd-button {
                width: 500px;
                height: 200px;
                font-size: 2.5rem;
            }
            
            .masters-phd-button .button-icon {
                font-size: 4.5rem;
            }
        }
        
        @media (max-width: 768px) {
            .header-logo {
                height: 80px;
                top: 20px;
                left: 20px;
            }
            
            .glowing-text {
                font-size: 3rem;
            }
            
            .subtitle {
                font-size: 1.6rem;
            }
            
            .large-years {
                flex-direction: column;
                gap: 25px;
            }
            
            .large-year {
                width: 280px;
                height: 320px;
            }
            
            .large-year .year-period {
                font-size: 2.2rem;
            }
            
            .large-year .year-label {
                font-size: 1.3rem;
            }
            
            .masters-phd-button {
                width: 350px;
                height: 160px;
                font-size: 2.2rem;
                padding: 30px;
            }
            
            .masters-phd-button .button-icon {
                font-size: 4rem;
                margin-bottom: 15px;
            }
            
            .section-title {
                font-size: 2.5rem;
            }
            
            .year-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .year-button {
                width: 90%;
                max-width: 300px;
            }
            
            .students-list, .graduates-list {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 480px) {
            .header-logo {
                height: 60px;
                top: 15px;
                left: 15px;
            }
            
            .glowing-text {
                font-size: 2.2rem;
            }
            
            .subtitle {
                font-size: 1.3rem;
            }
            
            .large-year {
                width: 260px;
                height: 300px;
            }
            
            .large-year .year-period {
                font-size: 2rem;
            }
            
            .large-year .year-icon {
                font-size: 5rem;
            }
            
            .masters-phd-button {
                width: 300px;
                height: 140px;
                font-size: 1.8rem;
                padding: 25px;
            }
            
            .masters-phd-button .button-icon {
                font-size: 3.5rem;
                margin-bottom: 10px;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .modal-content {
                padding: 25px;
            }
            
            .modal-image {
                width: 180px;
                height: 180px;
            }
        }
    </style>
</head>
<body>
    <!-- Hiệu ứng nền động -->
    <div class="dynamic-bg"></div>
    
    <!-- Hiệu ứng hạt ánh sáng -->
    <div class="particles" id="particles"></div>
    
    <!-- Hiệu ứng ánh sáng chiếu -->
    <div class="spotlight"></div>
    
    <!-- Loading spinner -->
    <div class="loading-spinner" id="loadingSpinner">
        <div class="spinner"></div>
    </div>
    
    <div class="floating-elements">
        <!-- Thêm nhiều phần tử trôi nổi hơn -->
        <div class="floating-element" style="width: 80px; height: 80px; top: 5%; left: 5%; animation-delay: 0s; animation-duration: 25s;"></div>
        <div class="floating-element" style="width: 120px; height: 120px; top: 15%; left: 80%; animation-delay: -2s; animation-duration: 30s;"></div>
        <div class="floating-element" style="width: 60px; height: 60px; top: 70%; left: 10%; animation-delay: -5s; animation-duration: 20s;"></div>
        <div class="floating-element" style="width: 100px; height: 100px; top: 40%; left: 60%; animation-delay: -8s; animation-duration: 35s;"></div>
        <div class="floating-element" style="width: 90px; height: 90px; top: 85%; left: 75%; animation-delay: -12s; animation-duration: 28s;"></div>
        <div class="floating-element" style="width: 70px; height: 70px; top: 20%; left: 30%; animation-delay: -15s; animation-duration: 22s;"></div>
    </div>
    
    <div class="container">
        <header>
            <div class="header-content">
                <div class="header-icon">
                    <i class="fas fa-trophy"></i>
                </div>
                <h1 class="glowing-text typewriter">BẢNG VINH DANH</h1>
                <div class="subtitle">20 NĂM HỌC THÀNH TÍCH RỰC RỠ</div>
            </div>
            <img src="https://i.postimg.cc/zGwcmPH1/image.png" alt="Logo" class="header-logo">
        </header>
        
        <!-- TRANG CHÍNH -->
        <div class="main-content page-transition" id="mainPage">
            <!-- Mảng 1: Vinh danh học sinh giỏi -->
            <div class="students-section">
                <h2 class="section-title">
                    <i class="fas fa-crown"></i> VINH DANH HỌC SINH CÓ THÀNH TÍCH CAO 
                </h2>
                <div class="large-years">
                    <div class="large-year enhanced-card magic-button" data-year="2005-2010">
                        <div class="year-icon"><i class="fas fa-seedling"></i></div>
                        <div class="year-period">2005-2010</div>
                        <div class="year-label">Giai đoạn Khởi đầu</div>
                    </div>
                    <div class="large-year enhanced-card magic-button" data-year="2010-2015">
                        <div class="year-icon"><i class="fas fa-chart-line"></i></div>
                        <div class="year-period">2010-2015</div>
                        <div class="year-label">Giai đoạn Phát triển</div>
                    </div>
                    <div class="large-year enhanced-card magic-button" data-year="2015-2020">
                        <div class="year-icon"><i class="fas fa-user-graduate"></i></div>
                        <div class="year-period">2015-2020</div>
                        <div class="year-label">Giai đoạn Trưởng thành</div>
                    </div>
                    <div class="large-year enhanced-card magic-button" data-year="2020-2025">
                        <div class="year-icon"><i class="fas fa-laptop-code"></i></div>
                        <div class="year-period">2020-2025</div>
                        <div class="year-label">Giai đoạn Hiện đại</div>
                    </div>
                    <div class="large-year enhanced-card magic-button" data-year="2025-2030">
                        <div class="year-icon"><i class="fas fa-rocket"></i></div>
                        <div class="year-period">2025-2030</div>
                        <div class="year-label">Giai đoạn Tương lai</div>
                    </div>
                </div>
            </div>
            
            <!-- Mảng 2: Vinh danh Thạc sĩ, Tiến sĩ - NÚT LỚN HƠN với chữ nhỏ hơn -->
            <div class="masters-phd-section">
                <h2 class="section-title">
                    <i class="fas fa-gem"></i> VINH DANH THẠC SĨ - TIẾN SĨ
                </h2>
                <div class="masters-phd-button enhanced-card magic-button" id="mastersPhdButton">
                    <div class="button-icon"><i class="fas fa-award"></i></div>
                    <div class="button-text">KHÁM PHÁ DANH SÁCH</div>
                </div>
            </div>
        </div>
        
        <!-- Container for year buttons -->
        <div class="year-buttons-container page-transition" id="yearButtonsContainer">
            <h2 class="year-buttons-title" id="yearButtonsTitle">Học sinh xuất sắc năm học</h2>
            <div class="year-buttons" id="yearButtons"></div>
            <button class="back-button magic-button" id="backButton">Quay lại</button>
        </div>
        
        <!-- Container for student page -->
        <div class="student-page page-transition" id="studentPage">
            <h2 id="studentPageTitle">VINH DANH HỌC SINH XUẤT SẮC NĂM HỌC</h2>
            <div class="students-list" id="studentsList"></div>
            <button class="back-to-years magic-button" id="backToYears">Quay lại danh sách năm học</button>
        </div>
        
        <!-- TRANG THẠC SĨ, TIẾN SĨ -->
        <div class="masters-phd-page page-transition" id="mastersPhdPage">
            <h2><i class="fas fa-gem"></i> VINH DANH CỰU HỌC SINH ĐẠT THẠC SĨ - TIẾN SĨ</h2>
            <div class="graduates-list" id="graduatesList"></div>
            <button class="back-to-main magic-button" id="backToMain">Quay lại trang chính</button>
        </div>
        
        <!-- Modal for details -->
        <div class="detail-modal" id="detailModal">
            <div class="modal-content">
                <span class="close-modal" id="closeModal">&times;</span>
                <div class="modal-header">
                    <h3 id="modalPersonName">Học sinh 1</h3>
                </div>
                <div class="modal-body">
                    <img src="" alt="Ảnh" class="modal-image image-3d" id="modalPersonImage">
                    <div class="modal-info" id="modalPersonInfo">
                        <!-- Information will be inserted here -->
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Tạo hiệu ứng hạt ánh sáng
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            for (let i = 0; i < 50; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                
                const size = Math.random() * 10 + 5;
                const left = Math.random() * 100;
                const animationDuration = Math.random() * 20 + 10;
                const animationDelay = Math.random() * 20;
                
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${left}%`;
                particle.style.animationDuration = `${animationDuration}s`;
                particle.style.animationDelay = `-${animationDelay}s`;
                
                particlesContainer.appendChild(particle);
            }
        }
        
        // Tạo hiệu ứng cho các phần tử trôi nổi
        function createFloatingElements() {
            const container = document.querySelector('.floating-elements');
            for (let i = 0; i < 15; i++) {
                const element = document.createElement('div');
                element.className = 'floating-element';
                const size = Math.random() * 80 + 40;
                const left = Math.random() * 100;
                const delay = Math.random() * 20;
                const duration = Math.random() * 20 + 20;
                
                element.style.width = `${size}px`;
                element.style.height = `${size}px`;
                element.style.top = `${Math.random() * 100}%`;
                element.style.left = `${left}%`;
                element.style.animationDelay = `-${delay}s`;
                element.style.animationDuration = `${duration}s`;
                
                container.appendChild(element);
            }
        }
        
        // Hiệu ứng loading
        function showLoading() {
            document.getElementById('loadingSpinner').style.display = 'block';
            setTimeout(() => {
                document.getElementById('loadingSpinner').style.display = 'none';
            }, 800);
        }
        
        // Hiệu ứng cho năm (cả nút nhỏ và nút lớn)
        document.querySelectorAll('.large-year').forEach(year => {
            year.addEventListener('click', function() {
                showLoading();
                setTimeout(() => {
                    const yearPeriod = this.getAttribute('data-year');
                    showYearButtons(yearPeriod);
                }, 500);
            });
        });
        
        // Xử lý nút Thạc sĩ, Tiến sĩ
        document.getElementById('mastersPhdButton').addEventListener('click', function() {
            showLoading();
            setTimeout(() => {
                showMastersPhdPage();
            }, 500);
        });
        
        // Hàm hiển thị các nút năm học
        function showYearButtons(yearPeriod) {
            // Ẩn nội dung chính
            document.getElementById('mainPage').style.display = 'none';
            
            // Hiển thị container các nút năm học
            const yearButtonsContainer = document.getElementById('yearButtonsContainer');
            yearButtonsContainer.style.display = 'flex';
            
            // Cập nhật tiêu đề
            document.getElementById('yearButtonsTitle').textContent = `Học sinh xuất sắc giai đoạn ${yearPeriod}`;
            
            // Tạo các nút năm học
            const yearButtons = document.getElementById('yearButtons');
            yearButtons.innerHTML = ''; // Xóa nội dung cũ
            
            // Lấy năm học bắt đầu và kết thúc từ yearPeriod (vd: "2005-2010")
            const [startYear, endYear] = yearPeriod.split('-').map(Number);
            
            // Tạo nút cho từng năm học trong giai đoạn
            for (let year = startYear; year <= endYear; year++) {
                const nextYear = year + 1;
                const yearButton = document.createElement('div');
                yearButton.className = 'year-button enhanced-card magic-button';
                yearButton.textContent = `Năm học ${year}-${nextYear}`;
                yearButton.addEventListener('click', function() {
                    showLoading();
                    setTimeout(() => {
                        showStudentPage(`${year}-${nextYear}`);
                    }, 500);
                });
                yearButtons.appendChild(yearButton);
            }
        }
        
        // Hàm hiển thị trang vinh danh học sinh
        function showStudentPage(year) {
            // Ẩn tất cả các phần khác
            document.getElementById('mainPage').style.display = 'none';
            document.getElementById('yearButtonsContainer').style.display = 'none';
            document.getElementById('mastersPhdPage').style.display = 'none';
            
            // Hiển thị trang học sinh
            const studentPage = document.getElementById('studentPage');
            studentPage.style.display = 'block';
            
            // Cập nhật tiêu đề
            document.getElementById('studentPageTitle').textContent = `VINH DANH HỌC SINH XUẤT SẮC NĂM HỌC ${year}`;
            
            // Tạo danh sách học sinh mẫu
            const studentsList = document.getElementById('studentsList');
            studentsList.innerHTML = ''; // Xóa nội dung cũ
            
            // Tạo 5 học sinh mẫu
            for (let i = 1; i <= 5; i++) {
                const studentCard = document.createElement('div');
                studentCard.className = 'student-card enhanced-card';
                studentCard.innerHTML = `
                    <div class="student-icon"><i class="fas fa-star"></i></div>
                    <img src="https://via.placeholder.com/160x160/3a6dc9/FFFFFF?text=HS+${i}" alt="Học sinh ${i}" class="student-image image-3d">
                    <h3>Học sinh ${i}</h3>
                    <p>Thành tích: Giải Nhất môn Toán</p>
                    <p>Lớp: 9A${i}</p>
                    <p>Điểm TB: 9.${i}</p>
                `;
                
                // Thêm sự kiện click để hiển thị modal
                studentCard.addEventListener('click', function() {
                    showDetailModal(i, year, 'student');
                });
                
                studentsList.appendChild(studentCard);
            }
        }
        
        // Hàm hiển thị trang Thạc sĩ, Tiến sĩ
        function showMastersPhdPage() {
            // Ẩn tất cả các phần khác
            document.getElementById('mainPage').style.display = 'none';
            document.getElementById('yearButtonsContainer').style.display = 'none';
            document.getElementById('studentPage').style.display = 'none';
            
            // Hiển thị trang Thạc sĩ, Tiến sĩ
            const mastersPhdPage = document.getElementById('mastersPhdPage');
            mastersPhdPage.style.display = 'block';
            
            // Tạo danh sách cựu học sinh mẫu
            const graduatesList = document.getElementById('graduatesList');
            graduatesList.innerHTML = ''; // Xóa nội dung cũ
            
            // Danh sách các học vị và thông tin mẫu
            const graduates = [
                {
                    name: "Nguyễn Văn A",
                    degree: "Tiến sĩ",
                    major: "Khoa học Máy tính",
                    workplace: "Đại học Quốc gia Hà Nội",
                    achievement: "Nghiên cứu về Trí tuệ Nhân tạo",
                    year: 2010,
                    icon: "fas fa-user-graduate"
                },
                {
                    name: "Trần Thị B",
                    degree: "Thạc sĩ", 
                    major: "Quản trị Kinh doanh",
                    workplace: "Tập đoàn FPT",
                    achievement: "Quản lý dự án phần mềm",
                    year: 2012,
                    icon: "fas fa-briefcase"
                },
                {
                    name: "Lê Văn C",
                    degree: "Tiến sĩ",
                    major: "Y học",
                    workplace: "Bệnh viện Bạch Mai",
                    achievement: "Nghiên cứu điều trị ung thư",
                    year: 2015,
                    icon: "fas fa-user-md"
                },
                {
                    name: "Phạm Thị D",
                    degree: "Thạc sĩ",
                    major: "Luật học",
                    workplace: "Văn phòng Luật sư Dragon",
                    achievement: "Chuyên gia luật quốc tế",
                    year: 2013,
                    icon: "fas fa-balance-scale"
                },
                {
                    name: "Hoàng Văn E",
                    degree: "Tiến sĩ",
                    major: "Vật lý học",
                    workplace: "Viện Hàn lâm Khoa học",
                    achievement: "Nghiên cứu vật liệu mới",
                    year: 2018,
                    icon: "fas fa-atom"
                },
                {
                    name: "Vũ Thị F",
                    degree: "Thạc sĩ",
                    major: "Ngôn ngữ học",
                    workplace: "Đại học Sư phạm Hà Nội",
                    achievement: "Giáo viên xuất sắc",
                    year: 2016,
                    icon: "fas fa-chalkboard-teacher"
                }
            ];
            
            // Tạo card cho từng cựu học sinh
            graduates.forEach((graduate, index) => {
                const graduateCard = document.createElement('div');
                graduateCard.className = 'graduate-card enhanced-card';
                graduateCard.innerHTML = `
                    <div class="graduate-icon"><i class="${graduate.icon}"></i></div>
                    <img src="https://via.placeholder.com/180x180/FF8C42/FFFFFF?text=${graduate.name.split(' ').pop()}" alt="${graduate.name}" class="graduate-image image-3d">
                    <div class="degree-badge">${graduate.degree}</div>
                    <h3>${graduate.name}</h3>
                    <p>Chuyên ngành: ${graduate.major}</p>
                    <p>Nơi công tác: ${graduate.workplace}</p>
                    <p>Tốt nghiệp: ${graduate.year}</p>
                `;
                
                // Thêm sự kiện click để hiển thị modal
                graduateCard.addEventListener('click', function() {
                    showDetailModal(index, graduate, 'graduate');
                });
                
                graduatesList.appendChild(graduateCard);
            });
        }
        
        // Hàm hiển thị modal thông tin chi tiết
        function showDetailModal(id, data, type) {
            const modal = document.getElementById('detailModal');
            const personName = document.getElementById('modalPersonName');
            const personImage = document.getElementById('modalPersonImage');
            const personInfo = document.getElementById('modalPersonInfo');
            
            if (type === 'student') {
                // Hiển thị thông tin học sinh
                personName.textContent = `Học sinh ${id}`;
                personImage.src = `https://via.placeholder.com/220x220/3a6dc9/FFFFFF?text=HS+${id}`;
                personImage.alt = `Học sinh ${id}`;
                
                personInfo.innerHTML = `
                    <p><strong>Năm học:</strong> ${data}</p>
                    <p><strong>Lớp:</strong> 9A${id}</p>
                    <p><strong>Thành tích:</strong> Giải Nhất môn Toán</p>
                    <p><strong>Điểm trung bình:</strong> 9.${id}</p>
                    <p><strong>Ghi chú:</strong> Học sinh xuất sắc toàn diện</p>
                `;
            } else {
                // Hiển thị thông tin cựu học sinh
                const graduate = data;
                personName.textContent = graduate.name;
                personImage.src = `https://via.placeholder.com/220x220/FF8C42/FFFFFF?text=${graduate.name.split(' ').pop()}`;
                personImage.alt = graduate.name;
                
                personInfo.innerHTML = `
                    <p><strong>Học vị:</strong> ${graduate.degree}</p>
                    <p><strong>Chuyên ngành:</strong> ${graduate.major}</p>
                    <p><strong>Nơi công tác:</strong> ${graduate.workplace}</p>
                    <p><strong>Năm tốt nghiệp:</strong> ${graduate.year}</p>
                    <p><strong>Thành tích nổi bật:</strong> ${graduate.achievement}</p>
                    <p><strong>Ghi chú:</strong> Cựu học sinh xuất sắc của trường</p>
                `;
            }
            
            // Hiển thị modal
            modal.style.display = 'flex';
        }
        
        // Đóng modal
        document.getElementById('closeModal').addEventListener('click', function() {
            document.getElementById('detailModal').style.display = 'none';
        });
        
        // Đóng modal khi click bên ngoài
        window.addEventListener('click', function(event) {
            const modal = document.getElementById('detailModal');
            if (event.target === modal) {
                modal.style.display = 'none';
            }
        });
        
        // Xử lý nút quay lại từ danh sách năm học
        document.getElementById('backButton').addEventListener('click', function() {
            showLoading();
            setTimeout(() => {
                // Ẩn container các nút năm học
                document.getElementById('yearButtonsContainer').style.display = 'none';
                
                // Hiển thị lại nội dung chính
                document.getElementById('mainPage').style.display = 'flex';
            }, 500);
        });
        
        // Xử lý nút quay lại từ trang học sinh
        document.getElementById('backToYears').addEventListener('click', function() {
            showLoading();
            setTimeout(() => {
                // Ẩn trang học sinh
                document.getElementById('studentPage').style.display = 'none';
                
                // Hiển thị lại container các nút năm học
                document.getElementById('yearButtonsContainer').style.display = 'flex';
            }, 500);
        });
        
        // Xử lý nút quay lại từ trang Thạc sĩ, Tiến sĩ
        document.getElementById('backToMain').addEventListener('click', function() {
            showLoading();
            setTimeout(() => {
                // Ẩn trang Thạc sĩ, Tiến sĩ
                document.getElementById('mastersPhdPage').style.display = 'none';
                
                // Hiển thị lại nội dung chính
                document.getElementById('mainPage').style.display = 'flex';
            }, 500);
        });
        
        // Khởi tạo hiệu ứng khi trang tải xong
        window.addEventListener('DOMContentLoaded', function() {
            createParticles();
            createFloatingElements();
        });
    </script>
</body>
</html>
