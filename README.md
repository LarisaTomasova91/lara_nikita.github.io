<!DOCTYPE html>

<html lang="ru">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Лара и Никита | Детали свадьбы 30.08.2025</title>

    <script src="https://cdn.tailwindcss.com"></script>

    <script src="https://api-maps.yandex.ru/2.1/?apikey=ваш_api_ключ&lang=ru_RU" type="text/javascript"></script>

    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

    <style>

        body {

            font-family: 'Montserrat', sans-serif;

            color: #333;

            scroll-behavior: smooth;

            background-color: #f9f5f0;

        }

        .heading-font {

            font-family: 'Playfair Display', serif;

        }

        .hero {

            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');

            background-size: cover;

            background-position: center;

            background-attachment: fixed;

        }

        .divider {

            height: 2px;

            background: linear-gradient(to right, transparent, #d4a373, transparent);

            width: 150px;

            margin: 2rem auto;

        }

        .gold-divider {

            height: 1px;

            background: linear-gradient(to right, transparent, #d4af37, transparent);

            width: 200px;

            margin: 2rem auto;

        }

        .map-container {

            height: 400px;

            width: 100%;

            border-radius: 12px;

            box-shadow: 0 4px 20px rgba(0,0,0,0.1);

            border: 1px solid #e5e5e5;

        }

        .form-input {

            border-bottom: 1px solid #d4a373;

            transition: all 0.3s;

            background-color: transparent;

        }

        .form-input:focus {

            border-bottom: 2px solid #d4a373;

            outline: none;

        }

        .btn-primary {

            background-color: #d4a373;

            transition: all 0.3s;

            letter-spacing: 1px;

        }

        .btn-primary:hover {

            background-color: #b08968;

            transform: translateY(-2px);

        }

        .btn-gold {

            background-color: #d4af37;

            color: white;

            transition: all 0.3s;

            letter-spacing: 1px;

        }

        .btn-gold:hover {

            background-color: #c9a227;

            transform: translateY(-2px);

        }

        .btn-green {

            background-color: #4CAF50;

            color: white;

            transition: all 0.3s;

            letter-spacing: 1px;

        }

        .btn-green:hover {

            background-color: #3e8e41;

            transform: translateY(-2px);

        }

        .floral-divider {

            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath d='M12 2c3.31 0 6 2.69 6 6 0 2.22-1.21 4.16-3 5.2.9 3.37-1.66 6.8-5 6.8-3.31 0-6-2.69-6-6 0-2.22 1.21-4.16 3-5.2-.9-3.37 1.66-6.8 5-6.8zm0-2c-4.42 0-8 3.58-8 8 0 3.03 1.69 5.66 4.17 7 .34-2.66 2.35-4.64 5.08-5.42C13.5 8.83 12 6.5 12 4c0-.55.45-1 1-1s1 .45 1 1c0 2.4 1.53 4.48 3.73 5.42 2.73.78 4.74 2.76 5.08 5.42C22.31 15.66 24 13.03 24 10c0-4.42-3.58-8-8-8z' fill='%23d4af37'/%3E%3C/svg%3E");

            background-repeat: repeat-x;

            background-position: center;

            height: 24px;

            opacity: 0.7;

            margin: 3rem auto;

        }

        .countdown-number {

            transition: all 0.3s ease;

            font-weight: 300;

            letter-spacing: 2px;

        }

        .countdown-number:hover {

            transform: scale(1.1);

        }

        .guest-info {

            display: none;

            background: rgba(212, 175, 55, 0.1);

            padding: 1.5rem;

            border-radius: 0.5rem;

            margin-top: 1rem;

            border-left: 3px solid #d4af37;

            animation: slideIn 0.5s ease-out;

        }

        @keyframes slideIn {

            from { opacity: 0; transform: translateX(20px); }

            to { opacity: 1; transform: translateX(0); }

        }

        .program-card {

            background: rgba(255, 255, 255, 0.9);

            border-radius: 8px;

            padding: 30px;

            box-shadow: 0 5px 25px rgba(0,0,0,0.05);

            transition: all 0.3s;

            border: 1px solid rgba(212, 175, 55, 0.2);

            text-align: center;

        }

        .program-card:hover {

            transform: translateY(-5px);

            box-shadow: 0 8px 30px rgba(0,0,0,0.1);

        }

        .program-time {

            font-size: 1.5rem;

            color: #d4af37;

            margin-bottom: 1rem;

            font-weight: 600;

        }

        .program-title {

            font-size: 1.2rem;

            margin-bottom: 0.5rem;

            color: #333;

        }

        .program-description {

            text-align: center;

            margin-top: 0.5rem;

        }

        .page-section {

            position: relative;

            padding: 6rem 1rem;

        }

        .bg-overlay {

            position: absolute;

            top: 0;

            left: 0;

            right: 0;

            bottom: 0;

            background-color: rgba(0,0,0,0.4);

            z-index: -1;

        }

        .bg-image {

            position: absolute;

            top: 0;

            left: 0;

            right: 0;

            bottom: 0;

            background-size: cover;

            background-position: center;

            z-index: -2;

        }

        .color-circle {

            display: inline-block;

            width: 24px;

            height: 24px;

            border-radius: 50%;

            margin-right: 8px;

            border: 1px solid #eee;

            box-shadow: 0 2px 4px rgba(0,0,0,0.1);

        }

        .gallery-grid {

            display: grid;

            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));

            gap: 20px;

            margin-top: 30px;

        }

        .gallery-item {

            overflow: hidden;

            border-radius: 8px;

            box-shadow: 0 4px 15px rgba(0,0,0,0.1);

            transition: transform 0.3s;

            height: 250px;

            position: relative;

        }

        .gallery-item:hover {

            transform: scale(1.03);

            box-shadow: 0 6px 20px rgba(0,0,0,0.15);

        }

        .gallery-item img {

            width: 100%;

            height: 100%;

            object-fit: cover;

        }

        .section-title {

            position: relative;

            display: inline-block;

            margin-bottom: 3rem;

        }

        .section-title:after {

            content: '';

            position: absolute;

            bottom: -15px;

            left: 50%;

            transform: translateX(-50%);

            width: 80px;

            height: 2px;

            background: #d4af37;

        }

        .checkbox-container {

            display: flex;

            align-items: center;

            margin-bottom: 0.5rem;

        }

        .checkbox-container input {

            margin-right: 0.5rem;

        }

        .contact-button {

            display: inline-flex;

            align-items: center;

            background-color: #4CAF50;

            color: white;

            padding: 0.75rem 1.5rem;

            border-radius: 9999px;

            margin: 0.5rem;

            transition: all 0.3s;

            text-decoration: none;

        }

        .contact-button:hover {

            background-color: #3e8e41;

            transform: translateY(-2px);

        }

        .contact-button i {

            margin-right: 0.5rem;

        }

        .detail-item {

            display: flex;

            flex-direction: column;

            height: 100%;

        }

        .detail-content {

            flex-grow: 1;

        }

        .icon-center {

            display: flex;

            justify-content: center;

            margin-bottom: 1.5rem;

        }

 

        /* Мобильные стили */

        @media (max-width: 767px) {

            .hero {

                background-attachment: scroll;

                min-height: 90vh;

                padding-top: 60px;

            }

           

            h1 {

                font-size: 2.5rem;

                margin-bottom: 1rem;

            }

           

            .countdown-number {

                font-size: 2rem;

            }

           

            .countdown-label {

                font-size: 0.7rem;

            }

           

            .page-section {

                padding: 3rem 1rem;

            }

           

            .section-title {

                font-size: 2rem;

                margin-bottom: 2rem;

            }

           

            .section-title:after {

                bottom: -10px;

                width: 60px;

            }

           

            .program-card {

                padding: 20px;

            }

           

            .program-time {

                font-size: 1.2rem;

            }

           

            .program-title {

                font-size: 1rem;

            }

           

            .detail-item {

                padding: 20px;

            }

           

            .map-container {

                height: 300px;

            }

           

            .gallery-grid {

                grid-template-columns: 1fr;

                gap: 15px;

            }

           

            .gallery-item {

                height: 200px;

            }

           

            .contact-button {

                padding: 0.5rem 1rem;

                font-size: 0.9rem;

                margin: 0.25rem;

            }

           

            .btn-primary, .btn-gold, .btn-green {

                padding: 0.75rem 1.5rem;

                font-size: 1rem;

            }

           

            #countdown {

                gap: 0.5rem;

                margin-bottom: 1.5rem;

            }

           

            .floral-divider {

                margin: 2rem auto;

                height: 20px;

            }

           

            footer {

                padding: 2rem 1rem;

            }

           

            /* Форма RSVP */

            iframe {

                width: 100%;

                min-width: 100%;

                max-width: 100%;

            }

        }

       

        @media (max-width: 480px) {

            h1 {

                font-size: 2rem;

            }

           

            .countdown-number {

                font-size: 1.5rem;

            }

           

            .btn-primary, .btn-gold, .btn-green {

                padding: 0.6rem 1.2rem;

                font-size: 0.9rem;

            }

           

            .program-card {

                padding: 15px;

            }

           

            .detail-item {

                padding: 15px;

            }

        }

    </style>

</head>

<body class="overflow-x-hidden">

    <!-- Hero Section -->

    <section class="hero min-h-screen flex items-center justify-center text-center text-white relative">

        <div class="absolute inset-0 bg-black opacity-30"></div>

        <div class="container px-4 mx-auto relative z-10">

            <div class="gold-divider"></div>

            <h1 class="heading-font text-5xl md:text-7xl mb-6 tracking-wider">Лара & Никита</h1>

            <p class="text-xl md:text-2xl mb-8 tracking-widest">30 АВГУСТА 2025 ГОДА</p>

            <div class="gold-divider"></div>

            <p class="text-lg md:text-xl mb-12 max-w-2xl mx-auto leading-relaxed">Дорогие гости, с радостью приглашаем вас разделить с нами этот особенный день</p>

           

            <!-- Countdown Timer -->

            <div id="countdown" class="flex justify-center gap-6 md:gap-10 mb-12">

                <div class="text-center">

                    <div class="text-4xl md:text-6xl font-light days countdown-number">00</div>

                    <div class="text-sm md:text-base tracking-widest">ДНЕЙ</div>

                </div>

                <div class="text-center">

                    <div class="text-4xl md:text-6xl font-light hours countdown-number">00</div>

                    <div class="text-sm md:text-base tracking-widest">ЧАСОВ</div>

                </div>

                <div class="text-center">

                    <div class="text-4xl md:text-6xl font-light minutes countdown-number">00</div>

                    <div class="text-sm md:text-base tracking-widest">МИНУТ</div>

                </div>

                <div class="text-center">

                    <div class="text-4xl md:text-6xl font-light seconds countdown-number">00</div>

                    <div class="text-sm md:text-base tracking-widest">СЕКУНД</div>

                </div>

            </div>

           

            <button id="rsvp-button" class="btn-gold inline-block px-10 py-4 rounded-full text-white font-semibold text-lg shadow-lg hover:shadow-xl transition-all duration-300 tracking-widest">ПОДТВЕРДИТЬ ПРИСУТСТВИЕ</button>

        </div>

    </section>

 

    <!-- Программа свадьбы -->

    <section class="page-section">

        <div class="bg-image" style="background-image: url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');"></div>

        <div class="bg-overlay"></div>

        <div class="container mx-auto max-w-5xl relative z-10">

            <h2 class="heading-font text-4xl md:text-5xl text-center mb-16 text-white section-title">ПРОГРАММА ТОРЖЕСТВА</h2>

           

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">

                <!-- Роспись -->

                <div class="program-card">

                    <div class="text-4xl mb-4 text-amber-700">

                        <i class="fas fa-file-signature"></i>

                    </div>

                    <div class="program-time">11:00</div>

                    <h3 class="program-title heading-font">РОСПИСЬ В ЗАГСЕ</h3>

                    <p class="program-description text-gray-600">Моложены и Родители</p>

                </div>

               

                <!-- Welcome -->

                <div class="program-card">

                    <div class="text-4xl mb-4 text-amber-700">

                        <i class="fas fa-glass-cheers"></i>

                    </div>

                    <div class="program-time">14:00</div>

                    <h3 class="program-title heading-font">WELCOME</h3>

                    <p class="program-description text-gray-600">Фуршет и Знакомство гостей</p>

                </div>

               

                <!-- Церемония -->

                <div class="program-card">

                    <div class="text-4xl mb-4 text-amber-700">

                        <i class="fas fa-heart"></i>

                    </div>

                    <div class="program-time">15:30</div>

                    <h3 class="program-title heading-font">ТОРЖЕСТВЕННАЯ ЦЕРЕМОНИЯ</h3>

                    <p class="program-description text-gray-600">Начало официальной части торжества</p>

                </div>

               

                <!-- Салют -->

                <div class="program-card">

                    <div class="text-4xl mb-4 text-amber-700">

                        <i class="fas fa-fire"></i>

                    </div>

                    <div class="program-time">22:00</div>

                    <h3 class="program-title heading-font">САЛЮТ И ЗАВЕРШЕНИЕ</h3>

                    <p class="program-description text-gray-600">Яркий финал торжества</p>

                </div>

            </div>

           

            <div class="floral-divider"></div>

        </div>

    </section>

 

    <!-- Детали свадьбы -->

    <section class="page-section bg-white">

        <div class="bg-image" style="background-image: url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');"></div>

        <div class="bg-overlay"></div>

        <div class="container mx-auto max-w-5xl relative z-10">

            <h2 class="heading-font text-4xl md:text-5xl text-center mb-16 text-black section-title">ДЕТАЛИ</h2>

           

            <div class="grid md:grid-cols-3 gap-8 mb-16">

                <!-- Дресс-код -->

               <div class="detail-item text-center p-8 rounded-lg bg-white bg-opacity-90 hover:bg-opacity-100 transition-all duration-300 shadow-md">

    <div class="detail-content">

        <div class="text-4xl mb-6 text-amber-700">

            <i class="fas fa-tshirt"></i>

        </div>

        <h3 class="heading-font text-2xl mb-4">ДРЕСС-КОД</h3>

        <p class="font-medium">Вечерний наряд</p>

        <div class="mt-4 mb-2">

            <span class="color-circle" style="background-color: #F7E5CE;"></span> <!-- Шампань -->

            <span class="color-circle" style="background-color: #E3B5A4;"></span> <!-- Мягкая черешня -->

            <span class="color-circle" style="background-color: #9F6B6B;"></span> <!-- Вишня -->

            <span class="color-circle" style="background-color: #D9B8B8;"></span> <!-- Нежная клюква -->

            <span class="color-circle" style="background-color: #BEA5A5;"></span> <!-- Пепельная роза -->

            <span class="color-circle" style="background-color: #8C4F4F;"></span> <!-- Вавилон -->

        </div>

        <p class="text-sm text-gray-600">Цветовая гамма: шампань, мягкая черешня, вишня, нежная клюква, пепельная роза, вавилон</p>

    </div>

</div>

               

                <!-- Пожелания по подарку -->

                <div class="detail-item text-center p-8 rounded-lg bg-white bg-opacity-90 hover:bg-opacity-100 transition-all duration-300 shadow-md">

                    <div class="detail-content">

                        <div class="text-4xl mb-6 text-amber-700">

                            <i class="fas fa-gift"></i>

                        </div>

                        <h3 class="heading-font text-2xl mb-4">ПОЖЕЛАНИЯ ПО ПОДАРКУ</h3>

                        <p class="mb-4 text-gray-600">Мы будем рады конверту на наши мечты</p>

                        <div class="text-2xl mb-4 text-amber-700">

                            <i class="fas fa-heart"></i>

                        </div>

                        <p class="text-sm text-gray-600">Ваше присутствие - лучший подарок для нас!</p>

                    </div>

                </div>

               

                <!-- Место мероприятия -->

                <div class="detail-item text-center p-8 rounded-lg bg-white bg-opacity-90 hover:bg-opacity-100 transition-all duration-300 shadow-md">

                    <div class="detail-content">

                        <div class="text-4xl mb-6 text-amber-700">

                            <i class="fas fa-map-marker-alt"></i>

                        </div>

                        <h3 class="heading-font text-2xl mb-4">МЕСТО МЕРОПРИЯТИЯ</h3>

                        <div class="mb-2">

                            <div class="font-semibold text-lg">ЯХТ-КЛУБ "ПОРТОФИНО"</div>

                            <div class="text-gray-600">г. Мытищи, Прибрежная улица, стр.19</div>

                        </div>

                    </div>

                </div>

            </div>

           

            <!-- Как добраться -->

            <div class="mt-12 bg-white bg-opacity-90 p-8 rounded-lg shadow-md">

                <h3 class="heading-font text-3xl text-center mb-8">КАК ДОБРАТЬСЯ</h3>

                <div class="map-container">

                    <iframe

                      src="https://yandex.ru/map-widget/v1/?ll=37.712413%2C55.974290&pt=37.712413%2C55.974290%2Cpm2rd3&z=17"

                      width="100%"

                      height="400"

                      frameborder="0">

                    </iframe>

                </div>

                <p class="text-center mt-6 text-gray-600">Для навигации используйте адрес: Прибрежная ул., с19, Мытищи</p>

            </div>    

           

            <div class="floral-divider"></div>

        </div>

    </section>

 

    <!-- Фотографии -->

    <section class="page-section">

        <div class="bg-image" style="background-image: url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');"></div>

        <div class="bg-overlay"></div>

        <div class="container mx-auto max-w-6xl relative z-10">

            <h2 class="heading-font text-4xl md:text-5xl text-center mb-16 text-white section-title">НАШИ ФОТОГРАФИИ</h2>

           

            <div class="bg-white bg-opacity-95 p-10 rounded-xl shadow-lg">

                <p class="text-center mb-10 text-xl max-w-3xl mx-auto leading-relaxed">Дорогие гости, здесь вы найдете все памятные моменты нашего торжества.</p>

               

                <div class="grid md:grid-cols-2 gap-10 mb-12">

                    <div class="bg-white p-8 rounded-lg shadow-lg border border-amber-100 transform transition-all duration-300 hover:scale-[1.02]">

                        <div class="icon-center">

                            <div class="text-5xl text-amber-700">

                                <i class="fas fa-camera-retro"></i>

                            </div>

                        </div>

                        <h3 class="heading-font text-2xl mb-4 text-center">ОФИЦИАЛЬНЫЕ ФОТОГРАФИИ</h3>

                        <p class="mb-6 text-gray-600 text-center">Профессиональные снимки от нашего фотографа</p>

                        <div class="text-center">

                            <a href="https://drive.google.com/drive/folders/1Cp5hnF7xIiEhDM-NN3O4Pb4SnzjhdZn1?usp=drive_link" target="_blank" class="btn-gold inline-block px-8 py-3 rounded-full text-white font-medium text-lg hover:shadow-lg transition-all">GOOGLE ДИСК</a>

                        </div>

                    </div>

                   

                    <div class="bg-white p-8 rounded-lg shadow-lg border border-amber-100 transform transition-all duration-300 hover:scale-[1.02]">

                        <div class="icon-center">

                            <div class="text-5xl text-amber-700">

                                <i class="fas fa-mobile-alt"></i>

                            </div>

                        </div>

                        <h3 class="heading-font text-2xl mb-4 text-center">ФОТО ОТ ГОСТЕЙ</h3>

                        <p class="mb-6 text-gray-600 text-center">Ваши любимые моменты, запечатленные на камеры</p>

                        <div class="text-center">

                            <a href="https://drive.google.com/drive/folders/10iitnEsqlgQ0P_-n1GiAp24hYsluaC-c?usp=drive_link" target="_blank" class="btn-gold inline-block px-8 py-3 rounded-full text-white font-medium text-lg hover:shadow-lg transition-all">GOOGLE ДИСК</a>

                        </div>

                    </div>

                </div>

               

                <div class="bg-amber-50 p-8 rounded-lg border border-amber-200 max-w-4xl mx-auto">

                    <div class="flex flex-col md:flex-row items-center">

                        <div class="text-4xl mb-6 md:mb-0 md:mr-8 text-amber-700">

                            <i class="fas fa-cloud-upload-alt"></i>

                        </div>

                        <div>

                            <h3 class="heading-font text-2xl mb-4 text-center md:text-left">КАК ДОБАВИТЬ СВОИ ФОТОГРАФИИ?</h3>

                            <ol class="space-y-3 text-gray-700">

                                <li class="flex items-start">

                                    <span class="bg-amber-700 text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 flex-shrink-0">1</span>

                                    <span>Скачайте приложение <strong>Google Диск</strong> (если еще не установлено)</span>

                                </li>

                                <li class="flex items-start">

                                    <span class="bg-amber-700 text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 flex-shrink-0">2</span>

                                    <span>Перейдите в папку <a href="https://drive.google.com/drive/folders/10iitnEsqlgQ0P_-n1GiAp24hYsluaC-c?usp=drive_link" class="text-amber-700 font-medium hover:underline">"Наша свадьба"</a></span>

                                </li>

                                <li class="flex items-start">

                                    <span class="bg-amber-700 text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 flex-shrink-0">3</span>

                                    <span>Нажмите "+ Новый" → "Загрузить файлы" и добавьте свои фотографии</span>

                                </li>

                                <li class="flex items-start">

                                    <span class="bg-amber-700 text-white rounded-full w-6 h-6 flex items-center justify-center mr-3 flex-shrink-0">4</span>

                                    <span>Подпишите фото (укажите кто на фото и когда сделано)</span>

                                </li>

                            </ol>

                            <p class="mt-6 text-sm text-amber-800 text-center md:text-left">Фотографии будут храниться в течение года после свадьбы</p>

                        </div>

                    </div>

                </div>

            </div>

           

            <div class="floral-divider"></div>

        </div>

    </section>

 

    <!-- RSVP Section -->

    <section id="rsvp-section" class="page-section">

        <div class="bg-image" style="background-image: url('https://images.unsplash.com/photo-1519225421980-715cb0215aed?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');"></div>

        <div class="bg-overlay"></div>

        <div class="container mx-auto max-w-3xl relative z-10">

            <h2 class="heading-font text-4xl md:text-5xl text-center mb-12 text-white section-title">ПОДТВЕРДИТЕ ВАШЕ ПРИСУТСТВИЕ</h2>

            <p class="text-center mb-12 text-lg text-white">Пожалуйста, ответьте до 20 июля 2025 года</p>

            <div style="display: flex; justify-content: center; margin: 20px 0;">

                <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfO0wXMS9TkiUgqZUiIxxHeRzzetqIrykAk_zd3bpO3LZG_Eg/viewform?embedded=true" width="100%" height="1381" frameborder="1" marginheight="1" marginwidth="0">Загрузка…</iframe>

            </div>

        </div>

    </section>

 

    <!-- Футер -->

    <footer class="py-16 px-4 bg-amber-100 text-center">

        <div class="container mx-auto max-w-4xl">

            <h3 class="heading-font text-2xl text-amber-800 mb-6">КОНТАКТНЫЕ ДАННЫЕ</h3>

           

            <div class="flex flex-wrap justify-center mb-8">

                <div class="flex items-center mr-4">

                    <span class="mr-2">Лара:</span>

                    <a href="tel:+79153592609" class="btn-green inline-block px-4 py-2 rounded-full text-white font-medium">

                        +7 (915) 359-26-09

                    </a>

                </div>

                <div class="flex items-center">

                    <span class="mr-2">Никита:</span>

                    <a href="tel:+79778614828" class="btn-green inline-block px-4 py-2 rounded-full text-white font-medium">

                        +7 (977) 861-48-28

                    </a>

                </div>

            </div>

           

            <div class="flex justify-center space-x-4 mb-8">

                <a href="https://wa.me/79153592609" class="contact-button" target="_blank">

                    <i class="fab fa-whatsapp"></i> WhatsApp

                </a>

                <a href="https://t.me/tomasovalara" class="contact-button" target="_blank">

                    <i class="fab fa-telegram"></i> Telegram

                </a>

            </div>

           

            <div class="gold-divider max-w-xs mx-auto"></div>

            <p class="heading-font text-2xl text-amber-800 mt-8 mb-4">С ЛЮБОВЬЮ, ЛАРА И НИКИТА</p>

            <p class="text-gray-600">30 августа 2025 года</p>

        </div>

    </footer>

 

    <script>

        // Исправленный счетчик

        function updateCountdown() {

            // Указываем конкретную дату и время (30 августа 2025, 14:00 по Москве)

            const weddingDate = new Date('2025-08-30T14:00:00+03:00').getTime();

            const now = new Date().getTime();

            const distance = weddingDate - now;

           

            // Расчет временных единиц

            const days = Math.floor(distance / (1000 * 60 * 60 * 24));

            const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));

            const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));

            const seconds = Math.floor((distance % (1000 * 60)) / 1000);

           

            // Безопасное обновление элементов

            try {

                document.querySelector('.days').textContent = days.toString().padStart(2, '0');

                document.querySelector('.hours').textContent = hours.toString().padStart(2, '0');

                document.querySelector('.minutes').textContent = minutes.toString().padStart(2, '0');

                document.querySelector('.seconds').textContent = seconds.toString().padStart(2, '0');

               

                if (distance < 0) {

                    clearInterval(countdownTimer);

                    document.getElementById('countdown').innerHTML = `

                        <div class="text-3xl">Свадьба состоялась! Спасибо, что были с нами!</div>

                    `;

                }

            } catch (e) {

                console.error("Ошибка в счетчике:", e);

            }

        }

 

        // Запускаем счетчик

        let countdownTimer;

        document.addEventListener('DOMContentLoaded', function() {

            updateCountdown();

            countdownTimer = setInterval(updateCountdown, 1000);

           

            // Добавляем обработчик для кнопки подтверждения

            document.getElementById('rsvp-button').addEventListener('click', function() {

                const rsvpSection = document.getElementById('rsvp-section');

                rsvpSection.scrollIntoView({ behavior: 'smooth' });

            });

        });

    </script>

</body>

</html>

 
