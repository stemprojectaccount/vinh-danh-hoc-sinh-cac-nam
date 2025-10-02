<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vinh Danh Học Sinh Xuất Sắc - 20 Năm học</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
.header-logo {
    position: absolute;
    top: 20px;
    left: 30px;
    height: 175px; 
    width: auto;
    z-index: 10;
    filter: drop-shadow(0 0 10px rgba(255, 215, 0, 0.5));
    transition: all 0.3s ease;
}

.header-logo:hover {
    transform: scale(1.05);
    filter: drop-shadow(0 0 15px rgba(255, 215, 0, 0.8));
}

/* Responsive cho mobile */
@media (max-width: 768px) {
    .header-logo {
        height: 60px;
        top: 15px;
        left: 20px;
    }
}

@media (max-width: 480px) {
    .header-logo {
        height: 50px;
        top: 10px;
        left: 15px;
    }
}

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Quicksand', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #2A4D9B, #3a6dc9);
            color: #F8F6F2;
            min-height: 100vh;
            padding: 20px;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 100%;
            margin: 0 auto;
            background: rgba(10, 25, 47, 0.85);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.1);
            position: relative;
        }
        
        .container::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="50" cy="50" r="1" fill="rgba(255,255,255,0.03)"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
            pointer-events: none;
        }
        
        header {
            background: linear-gradient(135deg, rgba(42, 77, 155, 0.9), rgba(58, 109, 201, 0.8));
            color: #F8F6F2;
            text-align: center;
            padding: 80px 20px 60px;
            position: relative;
            overflow: hidden;
            border-bottom: 1px solid rgba(255, 215, 0, 0.3);
        }
        
        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none"><path d="M0,0 L100,0 L100,100 Z" fill="rgba(255,215,0,0.1)"/></svg>');
            background-size: cover;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        .glowing-text {
            font-size: 4.5rem;
            margin-bottom: 20px;
            text-shadow: 0 0 10px rgba(254 , 224 , 255 , 0 ), 0 0 20px rgba(255, 215, 0, 0.5), 0 0 30px rgba(255, 215, 0, 0 );
            position: relative;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
            letter-spacing: 2px;
            animation: glow 3s ease-in-out infinite alternate;
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
            font-size: 2rem;
            margin-bottom: 10px;
            position: relative;
            color: #e0e0ff;
            font-weight: 500;
        }
        
        .header-icon {
            font-size: 3rem;
            color: #FFD700;
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
        
        .main-content {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 70vh;
            padding: 60px 20px;
            flex-direction: column;
            gap: 80px;
        }
        
        .section-title {
            font-size: 3.2rem;
            text-align: center;
            margin-bottom: 50px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
            position: relative;
            display: inline-block;
            padding: 0 20px;
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
        
        .large-years {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 40px;
            width: 100%;
            max-width: 1400px;
        }
        
        .large-year {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            border-radius: 25px;
            width: 300px;
            height: 350px;
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
            font-size: 6rem;
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
            font-size: 2.8rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .large-year .year-label {
            font-size: 1.5rem;
            opacity: 0.9;
            color: #e0e0ff;
            font-weight: 500;
        }
        
        /* Nút Thạc sĩ, Tiến sĩ - LỚN HƠN với chữ nhỏ hơn */
        .masters-phd-section {
            width: 100%;
            text-align: center;
            margin-top: 30px;
        }
        
        .masters-phd-button {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.9), rgba(232, 106, 51, 0.9));
            border-radius: 35px;
            width: 600px;
            height: 220px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: 2.8rem; /* Giảm kích thước chữ */
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
            font-size: 5rem; /* Giảm kích thước icon */
            margin-bottom: 20px; /* Giảm khoảng cách */
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
            letter-spacing: 1px; /* Giảm khoảng cách chữ */
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            line-height: 1.2; /* Điều chỉnh khoảng cách dòng */
        }
        
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
            animation: float 20s infinite linear;
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
        
        /* Styles for year buttons */
        .year-buttons-container {
            display: none;
            flex-direction: column;
            align-items: center;
            margin-top: 40px;
            padding: 30px;
            background: rgba(20, 40, 80, 0.8);
            border-radius: 20px;
            width: 90%;
            max-width: 900px;
            margin: 40px auto;
            border: 1px solid rgba(255, 215, 0, 0.3);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3);
        }
        
        .year-buttons-title {
            font-size: 2.5rem;
            margin-bottom: 30px;
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
            gap: 20px;
            width: 100%;
        }
        
        .year-button {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.8), rgba(42, 77, 155, 0.9));
            border-radius: 15px;
            padding: 20px 30px;
            font-size: 1.5rem;
            font-weight: bold;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3), 0 0 15px rgba(255, 215, 0, 0.2);
            cursor: pointer;
            min-width: 150px;
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
        
        .back-button {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.9), rgba(232, 106, 51, 0.9));
            margin-top: 30px;
            padding: 15px 30px;
            border-radius: 12px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            color: #F8F6F2;
            font-size: 1.3rem;
            transition: all 0.4s;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .back-button:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 20px rgba(255, 140, 66, 0.5);
        }
        
        /* Styles for student page */
        .student-page {
            display: none;
            padding: 50px 20px;
            text-align: center;
        }
        
        .student-page h2 {
            font-size: 3.2rem;
            margin-bottom: 40px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
        }
        
        .students-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .student-card {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.7), rgba(42, 77, 155, 0.8));
            border-radius: 20px;
            padding: 30px;
            border: 2px solid rgba(255, 215, 0, 0.4);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            min-height: 380px;
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
            width: 140px;
            height: 140px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 215, 0, 0.5);
            margin-bottom: 20px;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.4);
        }
        
        .student-card h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .student-card p {
            margin-bottom: 8px;
            font-size: 1.2rem;
            color: #e0e0ff;
        }
        
        .student-icon {
            font-size: 2.5rem;
            margin-bottom: 15px;
            color: #FFD700;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 8px rgba(255, 215, 0, 0.5));
        }
        
        .back-to-years {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.9), rgba(42, 77, 155, 0.9));
            margin-top: 40px;
            padding: 15px 35px;
            border-radius: 12px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            color: #F8F6F2;
            font-size: 1.3rem;
            transition: all 0.4s;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .back-to-years:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 20px rgba(58, 109, 201, 0.5);
        }
        
        /* Styles for masters-phd page */
        .masters-phd-page {
            display: none;
            padding: 50px 20px;
            text-align: center;
        }
        
        .masters-phd-page h2 {
            font-size: 3.2rem;
            margin-bottom: 40px;
            background: linear-gradient(45deg, #FFD700, #FFA500, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.5);
            font-weight: 700;
        }
        
        .graduates-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(380px, 1fr));
            gap: 35px;
            margin-top: 40px;
        }
        
        .graduate-card {
            background: linear-gradient(135deg, rgba(255, 140, 66, 0.7), rgba(232, 106, 51, 0.8));
            border-radius: 20px;
            padding: 35px;
            border: 2px solid rgba(255, 215, 0, 0.5);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            min-height: 450px;
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
            width: 160px;
            height: 160px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid rgba(255, 215, 0, 0.6);
            margin-bottom: 25px;
            box-shadow: 0 0 25px rgba(255, 215, 0, 0.5);
        }
        
        .graduate-card h3 {
            font-size: 2rem;
            margin-bottom: 15px;
            background: linear-gradient(45deg, #FFD700, #FFA500);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .degree-badge {
            background: linear-gradient(135deg, #FF8C42, #E86A33);
            padding: 8px 20px;
            border-radius: 25px;
            font-weight: bold;
            margin-bottom: 20px;
            font-size: 1.3rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            border: 1px solid rgba(255, 215, 0, 0.5);
        }
        
        .graduate-card p {
            margin-bottom: 10px;
            font-size: 1.2rem;
            color: #fff;
        }
        
        .graduate-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #FFD700;
            text-shadow: 0 0 20px rgba(255, 215, 0, 0.7);
            filter: drop-shadow(0 0 10px rgba(255, 215, 0, 0.5));
        }
        
        .back-to-main {
            background: linear-gradient(135deg, rgba(58, 109, 201, 0.9), rgba(42, 77, 155, 0.9));
            margin-top: 40px;
            padding: 15px 35px;
            border-radius: 12px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            color: #F8F6F2;
            font-size: 1.3rem;
            transition: all 0.4s;
            border: 2px solid rgba(255, 215, 0, 0.4);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .back-to-main:hover {
            transform: scale(1.05);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4), 0 0 20px rgba(58, 109, 201, 0.5);
        }
        
        /* Modal styles for details */
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
        
        @media (max-width: 1200px) {
            .large-years {
                gap: 30px;
            }
            
            .large-year {
                width: 280px;
                height: 320px;
            }
            
            .large-year .year-period {
                font-size: 2.5rem;
            }
            
            .masters-phd-button {
                width: 500px;
                height: 180px;
                font-size: 2.5rem; /* Giảm kích thước chữ cho màn hình vừa */
            }
            
            .masters-phd-button .button-icon {
                font-size: 4.5rem; /* Giảm kích thước icon cho màn hình vừa */
            }
        }
        
        @media (max-width: 768px) {
            .glowing-text {
                font-size: 2.8rem;
            }
            
            .subtitle {
                font-size: 1.6rem;
            }
            
            .large-years {
                flex-direction: column;
                gap: 25px;
            }
            
            .large-year {
                width: 260px;
                height: 300px;
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
                font-size: 2.2rem; /* Giảm kích thước chữ cho màn hình nhỏ */
                padding: 30px;
            }
            
            .masters-phd-button .button-icon {
                font-size: 3.5rem; /* Giảm kích thước icon cho màn hình nhỏ */
            }
            
            .year-buttons {
                gap: 15px;
            }
            
            .year-button {
                padding: 15px 25px;
                font-size: 1.3rem;
                min-width: 130px;
            }
            
            .student-page h2, .masters-phd-page h2 {
                font-size: 2.5rem;
            }
            
            .students-list, .graduates-list {
                grid-template-columns: 1fr;
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
                <h1 class="glowing-text">BẢNG VINH DANH</h1>
                <div class="subtitle">20 NĂM HỌC THÀNH TÍCH RỰC RỠ</div>
            </div>
     <img src="https://i.postimg.cc/zGwcmPH1/image.png" alt="Logo" class="header-logo">
                </div>
        </header>
        
        <!-- TRANG CHÍNH -->
        <div class="main-content" id="mainPage">
            <!-- Mảng 1: Vinh danh học sinh giỏi -->
            <div class="students-section">
                <h2 class="section-title">
                    <i class="fas fa-crown"></i> VINH DANH HỌC SINH CÓ THÀNH TÍCH CAO 
                </h2>
                <div class="large-years">
                    <div class="large-year" data-year="2005-2010">
                        <div class="year-icon"><i class="fas fa-seedling"></i></div>
                        <div class="year-period">2005-2010</div>
                        <div class="year-label">Giai đoạn Khởi đầu</div>
                    </div>
                    <div class="large-year" data-year="2010-2015">
                        <div class="year-icon"><i class="fas fa-chart-line"></i></div>
                        <div class="year-period">2010-2015</div>
                        <div class="year-label">Giai đoạn Phát triển</div>
                    </div>
                    <div class="large-year" data-year="2015-2020">
                        <div class="year-icon"><i class="fas fa-user-graduate"></i></div>
                        <div class="year-period">2015-2020</div>
                        <div class="year-label">Giai đoạn Trưởng thành</div>
                    </div>
                    <div class="large-year" data-year="2020-2025">
                        <div class="year-icon"><i class="fas fa-laptop-code"></i></div>
                        <div class="year-period">2020-2025</div>
                        <div class="year-label">Giai đoạn Hiện đại</div>
                    </div>
                    <div class="large-year" data-year="2025-2030">
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
                <div class="masters-phd-button" id="mastersPhdButton">
                    <div class="button-icon"><i class="fas fa-award"></i></div>
                    <div class="button-text">KHÁM PHÁ DANH SÁCH</div>
                </div>
            </div>
        </div>
        
        <!-- Container for year buttons -->
        <div class="year-buttons-container" id="yearButtonsContainer">
            <h2 class="year-buttons-title" id="yearButtonsTitle">Học sinh xuất sắc năm học</h2>
            <div class="year-buttons" id="yearButtons"></div>
            <button class="back-button" id="backButton">Quay lại</button>
        </div>
        
        <!-- Container for student page -->
        <div class="student-page" id="studentPage">
            <h2 id="studentPageTitle">VINH DANH HỌC SINH XUẤT SẮC NĂM HỌC</h2>
            <div class="students-list" id="studentsList"></div>
            <button class="back-to-years" id="backToYears">Quay lại danh sách năm học</button>
        </div>
        
        <!-- TRANG THẠC SĨ, TIẾN SĨ -->
        <div class="masters-phd-page" id="mastersPhdPage">
            <h2><i class="fas fa-gem"></i> VINH DANH CỰU HỌC SINH ĐẠT THẠC SĨ - TIẾN SĨ</h2>
            <div class="graduates-list" id="graduatesList"></div>
            <button class="back-to-main" id="backToMain">Quay lại trang chính</button>
        </div>
        
        <!-- Modal for details -->
        <div class="detail-modal" id="detailModal">
            <div class="modal-content">
                <span class="close-modal" id="closeModal">&times;</span>
                <div class="modal-header">
                    <h3 id="modalPersonName">Học sinh 1</h3>
                </div>
                <div class="modal-body">
                    <img src="" alt="Ảnh" class="modal-image" id="modalPersonImage">
                    <div class="modal-info" id="modalPersonInfo">
                        <!-- Information will be inserted here -->
                    </div>
                </div>
            </div>
        </div>

    <script>
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
        
        createFloatingElements();
        
        // Hiệu ứng cho năm (cả nút nhỏ và nút lớn)
        document.querySelectorAll('.large-year').forEach(year => {
            year.addEventListener('click', function() {
                const yearPeriod = this.getAttribute('data-year');
                showYearButtons(yearPeriod);
            });
        });
        
        // Xử lý nút Thạc sĩ, Tiến sĩ
        document.getElementById('mastersPhdButton').addEventListener('click', function() {
            showMastersPhdPage();
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
                yearButton.className = 'year-button';
                yearButton.textContent = `Năm học ${year}-${nextYear}`;
                yearButton.addEventListener('click', function() {
                    showStudentPage(`${year}-${nextYear}`);
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
                studentCard.className = 'student-card';
                studentCard.innerHTML = `
                    <div class="student-icon"><i class="fas fa-star"></i></div>
                    <img src="https://via.placeholder.com/140x140/3a6dc9/FFFFFF?text=HS+${i}" alt="Học sinh ${i}" class="student-image">
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
                graduateCard.className = 'graduate-card';
                graduateCard.innerHTML = `
                    <div class="graduate-icon"><i class="${graduate.icon}"></i></div>
                    <img src="https://via.placeholder.com/160x160/FF8C42/FFFFFF?text=${graduate.name.split(' ').pop()}" alt="${graduate.name}" class="graduate-image">
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
            // Ẩn container các nút năm học
            document.getElementById('yearButtonsContainer').style.display = 'none';
            
            // Hiển thị lại nội dung chính
            document.getElementById('mainPage').style.display = 'flex';
        });
        
        // Xử lý nút quay lại từ trang học sinh
        document.getElementById('backToYears').addEventListener('click', function() {
            // Ẩn trang học sinh
            document.getElementById('studentPage').style.display = 'none';
            
            // Hiển thị lại container các nút năm học
            document.getElementById('yearButtonsContainer').style.display = 'flex';
        });
        
        // Xử lý nút quay lại từ trang Thạc sĩ, Tiến sĩ
        document.getElementById('backToMain').addEventListener('click', function() {
            // Ẩn trang Thạc sĩ, Tiến sĩ
            document.getElementById('mastersPhdPage').style.display = 'none';
            
            // Hiển thị lại nội dung chính
            document.getElementById('mainPage').style.display = 'flex';
        });
    </script>
</body>
</html>
