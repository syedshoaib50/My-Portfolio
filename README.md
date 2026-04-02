<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Syed Muhammad Shoaib Mehdi | Portfolio</title>
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    
    <style>
        :root {
            --primary: #6366f1;
            --secondary: #a855f7;
            --accent: #ec4899;
        }

        body {
            background: #0f172a;
            color: white;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }

        .mesh-bg {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            z-index: -1;
            background: radial-gradient(circle at 0% 0%, rgba(99, 102, 241, 0.15) 0%, transparent 50%),
                        radial-gradient(circle at 100% 100%, rgba(236, 72, 153, 0.15) 0%, transparent 50%);
        }

        .box-3d {
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            transform-style: preserve-3d;
            transition: all 0.5s cubic-bezier(0.23, 1, 0.32, 1);
        }
        img {
            background-position: center;
            width: 50px;
            height: 100px;
        }
        .box-3d:hover {
            transform: rotateY(10deg) rotateX(10deg) translateY(-10px);
            border-color: var(--accent);
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }

        .nav-link:hover {
            text-shadow: 0 0 10px var(--primary);
            color: white;
        }

        .swiper {
            width: 100%;
            padding-top: 50px;
            padding-bottom: 50px;
        }

        .swiper-slide {
            background-position: center;
            background-size: cover;
            width: 300px;
            height: 400px;
            border-radius: 20px;
            overflow: hidden;
            border: 4px solid rgba(255, 255, 255, 0.1);
        }

        .slide-content {
            background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: flex-end;
            padding: 20px;
        }
    </style>
</head>
<body>

    <div class="mesh-bg"></div>

    <nav class="fixed top-0 w-full z-50 bg-slate-900/50 backdrop-blur-lg border-b border-white/10">
        <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
            <div class="text-2xl font-black bg-gradient-to-r from-indigo-500 to-pink-500 bg-clip-text text-transparent">
               <a href="#home" class="nav-link transition"> SMSMS. </a>
            </div>
            <div class="hidden md:flex space-x-10 font-medium text-gray-400">
                <a href="#home" class="nav-link transition">Home</a>
                <a href="#projects" class="nav-link transition">Projects</a>
                <a href="#education" class="nav-link transition"> My Edu.</a>
                <a href="#contact" class="nav-link transition">Contact</a>
            </div>
            <button class="bg-indigo-600 hover:bg-indigo-500 px-6 py-2 rounded-full font-bold transition shadow-lg shadow-indigo-500/20">
                Hire Me
            </button>
        </div>
    </nav>

    <section id="home" class="pt-32 pb-20 px-6 text-center">
        <h1 class="text-6xl md:text-8xl font-bold mb-6 tracking-tight">
            Syed Muhammad <br> <span class="text-transparent bg-clip-text bg-gradient-to-r from-pink-500 via-purple-500 to-indigo-500">Shoaib Mehdi</span>
        </h1>
        <p class="max-w-2xl mx-auto text-gray-400 text-lg">
            Specializing in advanced research and innovative methodology. Turning complex data into visual stories.
        </p>
    </section>

    <section id="projects" class="py-20 bg-slate-900/30">
        <div class="text-center mb-10">
            <h2 class="text-3xl font-bold">Featured Works</h2>
            <div class="h-1 w-20 bg-pink-500 mx-auto mt-2"></div>
        </div>

        <div class="swiper mySwiper">
            <div class="swiper-wrapper">
                <div class="swiper-slide" style="background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT8rZVeF58-kHCrUenUq_q0agy0VYLEgj1r1Q&s')">
                    <div class="slide-content">
                        <h3 class="font-bold text-xl">CV / Resume Writer</h3>
                        <p class="text-sm text-gray-300">Creating a Professional CV for your Career.</p>
                    </div>
                </div>
                <div class="swiper-slide" style="background-image: url('data:image/jpeg;base64,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')">
                    <div class="slide-content">
                        <h3 class="font-bold text-xl">Front-End Developer</h3>
                        <p class="text-sm text-gray-300">Create a creative webpages for your Website.</p>
                    </div>
                </div>
                    <div class="swiper-slide" style="background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQDbfV-tyKw0PN-mNcqXef1ymCVYgn0nxO_vA&s')">
                    <div class="slide-content">
                        <h3 class="font-bold text-xl">Website Design</h3>
                        <p class="text-sm text-gray-300">Modern Interfaces with Html/CSS</p>
                    </div>
                </div>
                <div class="swiper-slide" style="background-image: url('data:image/jpeg;base64,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')">
                    <div class="slide-content">
                        <h3 class="font-bold text-xl">Logo Designer</h3>
                        <p class="text-sm text-gray-300">Make a logo for your websites and For your businesses.</p>
                    </div>
                </div>
            </div>
            <div class="swiper-pagination"></div>
        </div>
    </section>

    <section id="education" class="py-24 px-6 relative">
    <div class="text-center mb-16">
        <h2 class="text-indigo-400 font-mono tracking-widest text-sm mb-2">MY JOURNEY</h2>
        <h3 class="text-4xl font-black italic">Academic Background</h3>
        <div class="h-1 w-20 bg-gradient-to-r from-indigo-500 to-pink-500 mx-auto mt-4"></div>
    </div>

    <div class="max-w-4xl mx-auto relative">
        <div class="absolute left-1/2 transform -translate-x-1/2 h-full w-1 bg-gradient-to-b from-indigo-600 via-purple-600 to-transparent opacity-30"></div>

        <div class="mb-12 flex justify-between items-center w-full right-timeline">
            <div class="order-1 w-5/12"></div>
            <div class="z-20 flex items-center order-1 bg-indigo-600 shadow-xl w-8 h-8 rounded-full border-4 border-slate-900">
                <div class="mx-auto font-semibold text-xs text-white">1</div>
            </div>
            <div class="order-1 glass-card w-5/12 px-6 py-4 hover:scale-105 transition-transform">
                <h4 class="mb-1 font-bold text-lg text-indigo-400">MPhil Scholar</h4>
                <p class="text-sm leading-snug tracking-wide text-gray-200 text-opacity-100">University of Lahore</p>
                <p class="text-xs text-gray-500 mt-1">2025 - Present</p>
                <p class="text-xs mt-2 italic text-gray-400">Specializing in advanced research methodologies and core academic excellence.</p>
            </div>
        </div>

        <div class="mb-12 flex justify-between items-center w-full left-timeline">
            <div class="order-1 glass-card w-5/12 px-6 py-4 hover:scale-105 transition-transform text-right">
                <h4 class="mb-1 font-bold text-lg text-pink-400">Bachelor's Degree</h4>
                <p class="text-sm leading-snug tracking-wide text-gray-200 text-opacity-100">Islamia University of Bahawalpur</p>
                <p class="text-xs text-gray-500 mt-1">Graduated 2025</p>
                <p class="text-xs mt-2 italic text-gray-400">Focused on foundational concepts and practical application.</p>
            </div>
            <div class="z-20 flex items-center order-1 bg-pink-600 shadow-xl w-8 h-8 rounded-full border-4 border-slate-900">
                <div class="mx-auto font-semibold text-xs text-white">2</div>
            </div>
            <div class="order-1 w-5/12"></div>
        </div>

        <div class="mb-12 flex justify-between items-center w-full right-timeline">
            <div class="order-1 w-5/12"></div>
            <div class="z-20 flex items-center order-1 bg-purple-600 shadow-xl w-8 h-8 rounded-full border-4 border-slate-900">
                <div class="mx-auto font-semibold text-xs text-white">3</div>
            </div>
            <div class="order-1 glass-card w-5/12 px-6 py-4 hover:scale-105 transition-transform">
                <h4 class="mb-1 font-bold text-lg text-purple-400">Intermediate / FSc</h4>
                <p class="text-sm leading-snug tracking-wide text-gray-200 text-opacity-100">Punjab Group of Colleges Alipur Campus</p>
                <p class="text-xs text-gray-500 mt-1">Completed - 2020</p>
            </div>
        </div>
        <div class="mb-12 flex justify-between items-center w-full left-timeline">
            <div class="order-1 glass-card w-5/12 px-6 py-4 hover:scale-105 transition-transform text-right">
                <h4 class="mb-1 font-bold text-lg text-pink-400">Matric</h4>
                <p class="text-sm leading-snug tracking-wide text-gray-200 text-opacity-100">Gov't High School Alipur </p>
                <p class="text-xs text-gray-500 mt-1">Completed - 2018</p>
                <p class="text-xs mt-2 italic text-gray-400">Doing With Science Group.</p>
            </div>
            <div class="z-20 flex items-center order-1 bg-pink-600 shadow-xl w-8 h-8 rounded-full border-4 border-slate-900">
                <div class="mx-auto font-semibold text-xs text-white">4</div>
            </div>
            <div class="order-1 w-5/12"></div>
        </div>
    </div>
</section>

    <section id="about" class="max-w-7xl mx-auto py-24 px-6">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-10">
            <div class="box-3d p-10 rounded-3xl">
                <div class="w-14 h-14 bg-indigo-600/20 flex items-center justify-center rounded-2xl mb-6 text-indigo-400">
                    <i class="fas fa-brain text-2xl"></i>
                </div>
                <h3 class="text-2xl font-bold mb-4">Analytical Thinking</h3>
                <p class="text-gray-400">Highly focused on data-driven results for MPhil level research and problem solving.</p>
            </div>

            <div class="box-3d p-10 rounded-3xl">
                <div class="w-14 h-14 bg-pink-600/20 flex items-center justify-center rounded-2xl mb-6 text-pink-400">
                    <i class="fas fa-microscope text-2xl"></i>
                </div>
                <h3 class="text-2xl font-bold mb-4">Advanced Research</h3>
                <p class="text-gray-400">Deep academic foundation from the University of Lahore, specializing in modern methodologies.</p>
            </div>

            <div class="box-3d p-10 rounded-3xl">
                <div class="w-14 h-14 bg-purple-600/20 flex items-center justify-center rounded-2xl mb-6 text-purple-400">
                    <i class="fas fa-cube text-2xl"></i>
                </div>
                <h3 class="text-2xl font-bold mb-4">3D Aesthetics</h3>
                <p class="text-gray-400">Merging functional academic content with cutting-edge visual presentation styles.</p>
            </div>
        </div>
    </section>
    <section id="contact" class="py-24 px-6">
    <div class="max-w-6xl mx-auto">
        <div class="text-center mb-16">
            <h2 class="text-pink-500 font-mono tracking-widest text-sm mb-2">REACH OUT</h2>
            <h3 class="text-4xl font-black italic text-white">Contact Information</h3>
            <div class="h-1 w-20 bg-gradient-to-r from-pink-500 to-indigo-500 mx-auto mt-4"></div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
            
            <div class="glass-card p-10 flex flex-col justify-between border-l-4 border-indigo-500">
                <div>
                    <h4 class="text-2xl font-bold text-white mb-8">Let's Connect</h4>
                    
                    <div class="flex items-start mb-6 group">
                        <div class="w-12 h-12 bg-indigo-600/20 rounded-lg flex items-center justify-center text-indigo-400 group-hover:bg-indigo-600 group-hover:text-white transition-all">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div class="ml-4">
                            <p class="text-xs text-gray-500 uppercase font-bold">Location</p>
                            <p class="text-gray-200">Lahore, Punjab, Pakistan</p>
                        </div>
                    </div>

                    <div class="flex items-start mb-6 group">
                        <div class="w-12 h-12 bg-pink-600/20 rounded-lg flex items-center justify-center text-pink-400 group-hover:bg-pink-600 group-hover:text-white transition-all">
                            <i class="fas fa-phone-alt"></i>
                        </div>
                        <div class="ml-4">
                            <p class="text-xs text-gray-500 uppercase font-bold">Contact Number</p>
                            <p class="text-gray-200">+92 308 1505404</p>
                        </div>
                    </div>

                    <div class="flex items-start mb-6 group">
                        <div class="w-12 h-12 bg-purple-600/20 rounded-lg flex items-center justify-center text-purple-400 group-hover:bg-purple-600 group-hover:text-white transition-all">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div class="ml-4">
                            <p class="text-xs text-gray-500 uppercase font-bold">Email</p>
                            <p class="text-gray-200">shoaibmehdi21@gmail.com</p>
                        </div>
                    </div>

                    <div class="flex items-start group">
                        <div class="w-12 h-12 bg-cyan-600/20 rounded-lg flex items-center justify-center text-cyan-400 group-hover:bg-cyan-600 group-hover:text-white transition-all">
                            <i class="fas fa-globe"></i>
                        </div>
                        <div class="ml-4">
                            <p class="text-xs text-gray-500 uppercase font-bold">Official Website</p>
                            <p class="text-gray-200">www.smsm-portfolio.com</p>
                        </div>
                    </div>
                </div>

                <div class="mt-12">
                    <p class="text-xs text-gray-500 mb-4 uppercase tracking-widest font-bold">Follow Me</p>
                    <div class="flex space-x-4">
                        <a href="https://www.linkedin.com/in/syed-shoaib-8491ab3b4/" class="w-10 h-10 rounded-full bg-white/5 border border-white/10 flex items-center justify-center hover:bg-indigo-600 hover:-translate-y-2 transition-all"><i class="fab fa-linkedin-in text-white"></i></a>
                        <a href="https://www.facebook.com/shoaib.mehdi.716" class="w-10 h-10 rounded-full bg-white/5 border border-white/10 flex items-center justify-center hover:bg-blue-600 hover:-translate-y-2 transition-all"><i class="fab fa-facebook-f text-white"></i></a>
                        <a href="https://www.instagram.com/syed.shoaib_bukhari/" class="w-10 h-10 rounded-full bg-white/5 border border-white/10 flex items-center justify-center hover:bg-pink-600 hover:-translate-y-2 transition-all"><i class="fab fa-instagram text-white"></i></a>
                        <a href="https://github.com/syedshoaib50" class="w-10 h-10 rounded-full bg-white/5 border border-white/10 flex items-center justify-center hover:bg-gray-800 hover:-translate-y-2 transition-all"><i class="fab fa-github text-white"></i></a>
                    </div>
                </div>
            </div>

            <div class="glass-card p-10 border-r-4 border-pink-500">
                <form action="#" class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label class="text-xs text-gray-400 uppercase">Full Name</label>
                            <input type="text" placeholder="Syed Shoaib" class="w-full bg-white/5 border border-white/10 rounded-lg px-4 py-3 text-white focus:border-indigo-500 outline-none transition">
                        </div>
                        <div>
                            <label class="text-xs text-gray-400 uppercase">Email Address</label>
                            <input type="email" placeholder="shoaib@example.com" class="w-full bg-white/5 border border-white/10 rounded-lg px-4 py-3 text-white focus:border-indigo-500 outline-none transition">
                        </div>
                    </div>
                    <div>
                        <label class="text-xs text-gray-400 uppercase">Subject</label>
                        <input type="text" placeholder="Research Collaboration" class="w-full bg-white/5 border border-white/10 rounded-lg px-4 py-3 text-white focus:border-indigo-500 outline-none transition">
                    </div>
                    <div>
                        <label class="text-xs text-gray-400 uppercase">Message</label>
                        <textarea rows="4" placeholder="How can I help you?" class="w-full bg-white/5 border border-white/10 rounded-lg px-4 py-3 text-white focus:border-indigo-500 outline-none transition"></textarea>
                    </div>
                    <button class="w-full bg-gradient-to-r from-indigo-600 to-pink-600 py-4 rounded-xl font-bold uppercase tracking-widest hover:opacity-90 transition shadow-lg shadow-indigo-500/20">
                        Send Message
                    </button>
                </form>
            </div>

        </div>
    </div>
</section>

    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script>
        var swiper = new Swiper(".mySwiper", {
            effect: "coverflow",
            grabCursor: true,
            centeredSlides: true,
            slidesPerView: "auto",
            coverflowEffect: {
                rotate: 50,
                stretch: 0,
                depth: 100,
                modifier: 1,
                slideShadows: true,
            },
            pagination: {
                el: ".swiper-pagination",
            },
            autoplay: {
                delay: 2500,
                disableOnInteraction: false,
            },
        });
    </script>
</body>
</html>
