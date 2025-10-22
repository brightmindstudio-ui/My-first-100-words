# My-first-100-words
About Brightmind Studio • Headline: About Brightmind Studio • Tagline: Smart ideas for curious minds. • Short Description: Briefly describe the publisher's mission to create high-quality, engaging educational materials for young learners.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First 100 English Words - Brightmind Studio</title>
    <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Nunito', 'sans-serif'],
                    },
                    colors: {
                        primary: '#FFD700', // light yellow/cream
                        secondary: '#87CEEB', // light blue
                        accent1: '#FFA500', // orange
                        accent2: '#FF0000', // red
                        accent3: '#00FF00', // green
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Nunito', sans-serif;
        }
        .hero-bg {
            background: linear-gradient(135deg, #FFD700 0%, #87CEEB 100%);
        }
        .nav-fixed {
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 10;
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
        }
        .flashcard {
            perspective: 1000px;
        }
        .flashcard-inner {
            position: relative;
            width: 100%;
            height: 100%;
            text-align: center;
            transition: transform 0.6s;
            transform-style: preserve-3d;
        }
        .flashcard.flipped .flashcard-inner {
            transform: rotateY(180deg);
        }
        .flashcard-front, .flashcard-back {
            position: absolute;
            width: 100%;
            height: 100%;
            -webkit-backface-visibility: hidden;
            backface-visibility: hidden;
            border-radius: 10px;
        }
        .flashcard-back {
            transform: rotateY(180deg);
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">
    <!-- Header & Navigation -->
    <header class="nav-fixed shadow-md">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <div class="flex items-center">
                <img src="brightmind-logo.png" alt="Brightmind Studio Logo" class="h-10 w-10 mr-2">
                <span class="text-xl font-bold text-gray-800">Brightmind Studio</span>
            </div>
            <nav class="hidden md:flex space-x-6">
                <a href="#hero" class="text-gray-700 hover:text-primary transition">Home</a>
                <a href="#features" class="text-gray-700 hover:text-primary transition">Features</a>
                <a href="#look-inside" class="text-gray-700 hover:text-primary transition">Look Inside</a>
                <a href="#about" class="text-gray-700 hover:text-primary transition">About</a>
                <a href="#purchase" class="bg-accent1 text-white px-4 py-2 rounded-full hover:bg-accent1/80 transition">Buy Now</a>
            </nav>
            <button class="md:hidden" id="nav-toggle">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                </svg>
            </button>
        </div>
        <div class="md:hidden hidden" id="mobile-nav">
            <nav class="bg-white shadow-md py-4">
                <a href="#hero" class="block px-4 py-2 text-gray-700 hover:bg-gray-100">Home</a>
                <a href="#features" class="block px-4 py-2 text-gray-700 hover:bg-gray-100">Features</a>
                <a href="#look-inside" class="block px-4 py-2 text-gray-700 hover:bg-gray-100">Look Inside</a>
                <a href="#about" class="block px-4 py-2 text-gray-700 hover:bg-gray-100">About</a>
                <a href="#purchase" class="block px-4 py-2 bg-accent1 text-white text-center">Buy Now</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="hero" class="hero-bg min-h-screen flex items-center justify-center pt-20">
        <div class="container mx-auto px-4 text-center">
            <h1 class="text-4xl md:text-6xl font-bold text-gray-800 mb-4">My First 100 English Words</h1>
            <p class="text-lg md:text-xl text-gray-700 mb-2">Vocabulary with Example Sentences & Exercises for Beginners.</p>
            <p class="text-md md:text-lg text-gray-600 mb-8">Smart Ideas for Curious Minds.</p>
            <img src="book-cover.jpg" alt="Book Cover" class="mx-auto mb-8 w-64 md:w-80 shadow-lg rounded-lg">
            <div class="space-x-4">
                <a href="#purchase" class="bg-accent2 text-white px-8 py-3 rounded-full text-lg font-semibold hover:bg-accent2/80 transition">Buy Now</a>
                <a href="#look-inside" class="bg-white text-gray-800 px-8 py-3 rounded-full text-lg font-semibold border border-gray-300 hover:bg-gray-100 transition">Look Inside</a>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section id="features" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-gray-800 mb-12">Start Your Child's English Journey!</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="text-center">
                    <div class="bg-primary rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <span class="text-2xl">📚</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">100 Essential Words</h3>
                    <p>Covers fundamental vocabulary across key topics.</p>
                </div>
                <div class="text-center">
                    <div class="bg-secondary rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <span class="text-2xl">🍎</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Thematic Units</h3>
                    <p>Includes words for Food, Drink, School, Family, and Work.</p>
                </div>
                <div class="text-center">
                    <div class="bg-accent1 rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <span class="text-2xl">🎨</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Engaging Illustrations</h3>
                    <p>Fun, clear, and colorful visuals aid memory.</p>
                </div>
                <div class="text-center">
                    <div class="bg-accent3 rounded-full w-16 h-16 mx-auto mb-4 flex items-center justify-center">
                        <span class="text-2xl">✏️</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Practice Exercises</h3>
                    <p>Includes "Write" and "Match" activities for active learning.</p>
                </div>
            </div>
            <div class="mt-8 text-center">
                <p class="text-gray-600">Example Sentences: Learn words in context (e.g., "This is a red apple.").</p>
            </div>
        </div>
    </section>

    <!-- Look Inside Section -->
    <section id="look-inside" class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-gray-800 mb-12">See the Learning in Action!</h2>
            <div class="flex overflow-x-auto space-x-4 pb-4">
                <img src="page1.jpg" alt="Unit 1: Food" class="w-64 h-80 object-cover rounded-lg shadow-md">
                <img src="page2.jpg" alt="Practice Lines" class="w-64 h-80 object-cover rounded-lg shadow-md">
                <img src="page3.jpg" alt="Example Sentences" class="w-64 h-80 object-cover rounded-lg shadow-md">
            </div>
            <p class="text-center text-gray-600 mt-4">Unit 1: Food - Clear visuals, practice lines, and example sentences.</p>
            <div class="mt-12 text-center">
                <h3 class="text-2xl font-semibold mb-4">Interactive Flashcards</h3>
                <div class="flex justify-center space-x-4">
                    <div class="flashcard w-32 h-32 cursor-pointer" onclick="flipCard(this)">
                        <div class="flashcard-inner">
                            <div class="flashcard-front bg-accent1 text-white flex items-center justify-center rounded-lg">
                                Apple
                            </div>
                            <div class="flashcard-back bg-accent2 text-white flex items-center justify-center rounded-lg">
                                🍎
                            </div>
                        </div>
                    </div>
                    <div class="flashcard w-32 h-32 cursor-pointer" onclick="flipCard(this)">
                        <div class="flashcard-inner">
                            <div class="flashcard-front bg-accent1 text-white flex items-center justify-center rounded-lg">
                                Bread
                            </div>
                            <div class="flashcard-back bg-accent2 text-white flex items-center justify-center rounded-lg">
                                🍞
                            </div>
                        </div>
                    </div>
                    <div class="flashcard w-32 h-32 cursor-pointer" onclick="flipCard(this)">
                        <div class="flashcard-inner">
                            <div class="flashcard-front bg-accent1 text-white flex items-center justify-center rounded-lg">
                                Bed
                            </div>
                            <div class="flashcard-back bg-accent2 text-white flex items-center justify-center rounded-lg">
                                🛏️
                            </div>
                        </div>
                    </div>
                    <div class="flashcard w-32 h-32 cursor-pointer" onclick="flipCard(this)">
                        <div class="flashcard-inner">
                            <div class="flashcard-front bg-accent1 text-white flex items-center justify-center rounded-lg">
                                House
                            </div>
                            <div class="flashcard-back bg-accent2 text-white flex items-center justify-center rounded-lg">
                                🏠
                            </div>
                        </div>
                    </div>
                    <div class="flashcard w-32 h-32 cursor-pointer" onclick="flipCard(this)">
                        <div class="flashcard-inner">
                            <div class="flashcard-front bg-accent1 text-white flex items-center justify-center rounded-lg">
                                Pencil
                            </div>
                            <div class="flashcard-back bg-accent2 text-white flex items-center justify-center rounded-lg">
                                ✏️
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-4">About Brightmind Studio</h2>
            <p class="text-lg text-gray-600 mb-8">Smart Ideas for Curious Minds.</p>
            <p class="text-gray-700 max-w-2xl mx-auto">Brightmind Studio is dedicated to creating high-quality, engaging educational materials for young learners. Our mission is to spark curiosity and foster a love for learning through fun, interactive content that makes education accessible and enjoyable for children and parents alike.</p>
        </div>
    </section>

    <!-- Purchase Section -->
    <section id="purchase" class="py-16 bg-gray-100">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-gray-800 mb-8">Ready to Begin?</h2>
            <div class="bg-white p-8 rounded-lg shadow-md max-w-md mx-auto">
                <h3 class="text-2xl font-semibold mb-4">My First 100 English Words</h3>
                <p class="text-gray-600 mb-2">Author: Brightmind Studio Team</p>
                <p class="text-gray-600 mb-2">Format: Paperback</p>
                <p class="text-2xl font-bold text-accent2 mb-4">$19.99</p>
                <a href="#" class="bg-accent2 text-white px-8 py-3 rounded-full text-lg font-semibold hover:bg-accent2/80 transition">Add to Cart</a>
                <div class="mt-4 flex justify-center space-x-2">
                    <img src="visa.png" alt="Visa" class="h-6">
                    <img src="paypal.png" alt="PayPal" class="h-6">
                    <img src="mastercard.png" alt="Mastercard" class="h-6">
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-4 text-center">
            <div class="mb-4">
                <a href="#" class="text-gray-400 hover:text-white mx-4">Privacy Policy</a>
                <a href="#" class="text-gray-400 hover:text-white mx-4">Contact Us</a>
            </div>
            <p>&copy; 2023 Brightmind Studio. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Mobile nav toggle
        const navToggle = document.getElementById('nav-toggle');
        const mobileNav = document.getElementById('mobile-nav');
        navToggle.addEventListener('click', () => {
            mobileNav.classList.toggle('hidden');
        });

        // Flashcard flip
        function flipCard(card) {
            card.classList.toggle('flipped');
        }
    </script>
</body>
</html>
