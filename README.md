<!DOCTYPE html>
<html lang="th" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ProPaint Thailand | บริการรับทาสีบ้านครบวงจร รับประกันงานสูงสุด 5 ปี</title>
    <!-- Google Fonts: Prompt & Sarabun -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;400;500;600;700&family=Sarabun:wght@300;400;500;600&display=swap" rel="stylesheet">
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        navy: {
                            DEFAULT: '#0F2942',
                            light: '#1B3F63',
                            dark: '#091A2B',
                            soft: '#EEF3F8'
                        },
                        teal: {
                            DEFAULT: '#0D9488',
                            light: '#2DD4BF',
                            dark: '#0F766E',
                            soft: '#F0FDFA'
                        },
                        amber: {
                            DEFAULT: '#F59E0B',
                            hover: '#D97706',
                            soft: '#FFFBEB'
                        },
                        offwhite: '#F8FAFC',
                        slateText: '#334155'
                    },
                    fontFamily: {
                        prompt: ['Prompt', 'sans-serif'],
                        sarabun: ['Sarabun', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Sarabun', sans-serif;
            background-color: #F8FAFC;
            color: #334155;
            overflow-x: hidden;
        }
        h1, h2, h3, h4, h5, h6, .font-heading {
            font-family: 'Prompt', sans-serif;
        }
        .glass-header {
            background: rgba(255, 255, 255, 0.94);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
        }
        /* Custom Range Slider for Calculator & Before/After */
        input[type="range"].custom-slider {
            -webkit-appearance: none;
            appearance: none;
            height: 8px;
            border-radius: 999px;
            background: #E2E8F0;
            outline: none;
        }
        input[type="range"].custom-slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            background: #F59E0B;
            border: 3px solid #FFFFFF;
            box-shadow: 0 2px 6px rgba(15, 41, 66, 0.3);
            cursor: pointer;
            transition: transform 0.15s ease;
        }
        input[type="range"].custom-slider::-webkit-slider-thumb:hover {
            transform: scale(1.15);
        }
        /* Before After Interactive Slider */
        .ba-container {
            position: relative;
            overflow: hidden;
            user-select: none;
            touch-action: pan-y;
        }
        .ba-after-wrapper {
            position: absolute;
            top: 0;
            left: 0;
            bottom: 0;
            overflow: hidden;
        }
        .ba-divider {
            position: absolute;
            top: 0;
            bottom: 0;
            width: 3px;
            background: #FFFFFF;
            box-shadow: 0 0 10px rgba(0,0,0,0.4);
            cursor: ew-resize;
            z-index: 20;
        }
        .ba-handle {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 42px;
            height: 42px;
            border-radius: 9999px;
            background: #F59E0B;
            color: #0F2942;
            border: 3px solid #FFFFFF;
            box-shadow: 0 4px 12px rgba(0,0,0,0.3);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        @keyframes pulseRing {
            0% { transform: scale(0.95); opacity: 0.7; }
            70% { transform: scale(1.25); opacity: 0; }
            100% { transform: scale(1.25); opacity: 0; }
        }
        .animate-pulse-ring::before {
            content: '';
            position: absolute;
            inset: -4px;
            border-radius: 9999px;
            background: inherit;
            z-index: -1;
            animation: pulseRing 2s infinite;
        }
    </style>
</head>
<body class="antialiased selection:bg-amber selection:text-navy">

    <!-- Top Announcement Bar -->
    <div class="bg-navy text-white text-xs sm:text-sm py-2 px-4 text-center font-heading">
        <div class="max-w-7xl mx-auto flex flex-wrap items-center justify-center gap-x-5 gap-y-1">
            <span class="inline-flex items-center gap-1.5">
                <i data-lucide="badge-check" class="w-4 h-4 text-amber"></i>
                <strong>โปรโมชั่นพิเศษเดือนนี้:</strong> นัดสำรวจหน้างานและประเมินราคา <strong>ฟรี!</strong> ไม่มีค่าใช้จ่าย
            </span>
            <span class="hidden md:inline text-white/30">|</span>
            <span class="inline-flex items-center gap-1.5 text-teal-light font-medium">
                <i data-lucide="phone-call" class="w-3.5 h-3.5"></i>
                สายด่วนปรึกษาช่าง: 02-888-9944
            </span>
        </div>
    </div>

    <!-- 1. Header / Navigation Bar -->
    <header class="sticky top-0 z-40 glass-header border-b border-slate-200/80 shadow-sm">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16 sm:h-20">
                <!-- Logo -->
                <a href="#home" class="flex items-center gap-3 group">
                    <div class="w-10 h-10 sm:w-11 sm:h-11 rounded-xl bg-navy flex items-center justify-center text-amber shadow-md group-hover:bg-navy-light transition">
                        <i data-lucide="paint-roller" class="w-6 h-6"></i>
                    </div>
                    <div>
                        <span class="font-heading font-bold text-xl sm:text-2xl text-navy tracking-tight block leading-none">
                            ProPaint <span class="text-teal">TH</span>
                        </span>
                        <span class="text-[11px] font-heading text-slate-500 tracking-wider uppercase font-medium">
                            Expert House Painting
                        </span>
                    </div>
                </a>

                <!-- Desktop Navigation -->
                <nav class="hidden lg:flex items-center space-x-7 font-heading text-sm font-medium text-navy">
                    <a href="#services" class="hover:text-teal transition py-2">บริการของเรา</a>
                    <a href="#portfolio" class="hover:text-teal transition py-2">ผลงานที่ผ่านมา</a>
                    <a href="#calculator" class="hover:text-teal transition py-2 flex items-center gap-1">
                        <span class="w-2 h-2 rounded-full bg-amber"></span>
                        คำนวณราคาเบื้องต้น
                    </a>
                    <a href="#process" class="hover:text-teal transition py-2">ขั้นตอนการทำงาน</a>
                    <a href="#reviews" class="hover:text-teal transition py-2">รีวิวลูกค้า</a>
                    <a href="#faq" class="hover:text-teal transition py-2">คำถามที่พบบ่อย</a>
                </nav>

                <!-- CTA Button & Mobile Menu Toggle -->
                <div class="flex items-center gap-2.5 sm:gap-3">
                    <a href="#quote-form" class="hidden sm:inline-flex items-center gap-2 px-5 py-2.5 rounded-xl bg-amber hover:bg-amber-hover text-navy font-heading font-semibold text-sm shadow-md shadow-amber/25 transition transform hover:-translate-y-0.5">
                        <i data-lucide="message-circle" class="w-4 h-4"></i>
                        ประเมินราคาฟรี / แอดไลน์
                    </a>
                    <a href="#quote-form" class="sm:hidden inline-flex items-center gap-1.5 px-3.5 py-2 rounded-xl bg-amber text-navy font-heading font-semibold text-xs shadow-sm">
                        ประเมินฟรี
                    </a>
                    <button id="mobile-menu-btn" aria-label="เปิดเมนู" class="lg:hidden p-2 rounded-xl text-navy hover:bg-slate-100 transition">
                        <i data-lucide="menu" class="w-6 h-6"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Dropdown Menu -->
        <div id="mobile-menu" class="hidden lg:hidden bg-white border-b border-slate-200 px-4 pt-2 pb-5 space-y-1 font-heading text-sm">
            <a href="#services" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-xl hover:bg-navy-soft text-navy font-medium">บริการของเรา</a>
            <a href="#portfolio" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-xl hover:bg-navy-soft text-navy font-medium">ผลงานที่ผ่านมา (Before/After)</a>
            <a href="#calculator" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-xl bg-amber-soft text-navy font-semibold">คำนวณราคาทาสีเบื้องต้น</a>
            <a href="#process" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-xl hover:bg-navy-soft text-navy font-medium">ขั้นตอนการทำงาน</a>
            <a href="#reviews" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-xl hover:bg-navy-soft text-navy font-medium">รีวิวลูกค้า</a>
            <a href="#faq" onclick="closeMobileMenu()" class="block px-3 py-2.5 rounded-xl hover:bg-navy-soft text-navy font-medium">คำถามที่พบบ่อย</a>
            <div class="pt-2">
                <a href="#quote-form" onclick="closeMobileMenu()" class="w-full py-3 rounded-xl bg-navy text-white font-semibold flex items-center justify-center gap-2">
                    <i data-lucide="clipboard-check" class="w-4 h-4 text-amber"></i>
                    ขอใบเสนอราคาฟรี / แอดไลน์
                </a>
            </div>
        </div>
    </header>

    <!-- 2. Hero Section -->
    <section id="home" class="relative bg-gradient-to-br from-navy via-navy-light to-[#153B5E] text-white pt-12 pb-16 sm:pt-16 sm:pb-24 overflow-hidden">
        <!-- Subtle Architectural Grid Pattern -->
        <div class="absolute inset-0 opacity-10 pointer-events-none" style="background-image: radial-gradient(#FFFFFF 1px, transparent 1px); background-size: 28px 28px;"></div>
        <div class="absolute -bottom-24 -right-24 w-96 h-96 bg-teal/20 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 lg:gap-12 items-center">
                <!-- Left Copy -->
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-white/10 border border-white/20 backdrop-blur-sm text-amber text-xs sm:text-sm font-heading font-medium">
                        <i data-lucide="shield-check" class="w-4 h-4"></i>
                        บริการรับทาสีบ้าน คอนโด อาคาร ครบวงจร • รับประกันงานสูงสุด 5 ปี
                    </div>

                    <h1 class="text-3xl sm:text-4xl lg:text-[46px] font-bold leading-tight tracking-tight">
                        เปลี่ยนบ้านเก่าให้สวยเหมือนใหม่<br>
                        ด้วย<span class="text-amber">ช่างทาสีมืออาชีพ</span><br>
                        <span class="text-teal-light text-2xl sm:text-3xl lg:text-[38px]">เก็บงานเนี๊ยบ ไม่ทิ้งงาน รับประกันนาน 5 ปี</span>
                    </h1>

                    <p class="text-slate-200 text-base sm:text-lg leading-relaxed max-w-2xl mx-auto lg:mx-0">
                        หมดกังวลเรื่องสีลอกล่อน ช่างทิ้งงาน หรือบ้านเลอะเทอะ เราดูแลตั้งแต่การซ่อมรอยแตกร้าว ขัดเตรียมพื้นผิว คลุมป้องกันเฟอร์นิเจอร์อย่างดี พร้อมใช้สีแท้เกรดพรีเมียม 100%
                    </p>

                    <!-- Key Highlights Pills -->
                    <div class="flex flex-wrap items-center justify-center lg:justify-start gap-3 pt-1">
                        <span class="inline-flex items-center gap-1.5 px-3.5 py-1.5 rounded-xl bg-white/10 text-xs sm:text-sm font-heading">
                            <i data-lucide="check-circle-2" class="w-4 h-4 text-teal-light"></i> สีแท้ 100% มาตรฐาน TOA / Dulux / Beger
                        </span>
                        <span class="inline-flex items-center gap-1.5 px-3.5 py-1.5 rounded-xl bg-white/10 text-xs sm:text-sm font-heading">
                            <i data-lucide="check-circle-2" class="w-4 h-4 text-teal-light"></i> ไม่ทิ้งงาน ส่งมอบตรงเวลา
                        </span>
                        <span class="inline-flex items-center gap-1.5 px-3.5 py-1.5 rounded-xl bg-white/10 text-xs sm:text-sm font-heading">
                            <i data-lucide="check-circle-2" class="w-4 h-4 text-teal-light"></i> คลุมเฟอร์นิเจอร์ & ทำความสะอาดฟรี
                        </span>
                    </div>

                    <!-- Dual CTA Buttons -->
                    <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-4 pt-3">
                        <a href="#calculator" class="w-full sm:w-auto px-7 py-4 rounded-2xl bg-amber hover:bg-amber-hover text-navy font-heading font-bold text-base shadow-lg shadow-amber/25 transition transform hover:-translate-y-0.5 flex items-center justify-center gap-2">
                            <i data-lucide="calculator" class="w-5 h-5"></i>
                            คำนวณราคาเบื้องต้น
                        </a>
                        <a href="#quote-form" class="w-full sm:w-auto px-7 py-4 rounded-2xl bg-white/10 hover:bg-white/20 text-white border border-white/30 font-heading font-semibold text-base backdrop-blur-sm transition flex items-center justify-center gap-2">
                            <i data-lucide="file-text" class="w-5 h-5 text-teal-light"></i>
                            ขอใบเสนอราคาฟรี
                        </a>
                    </div>
                </div>

                <!-- Right Hero Illustration / Visual Card -->
                <div class="lg:col-span-5">
                    <div class="relative mx-auto max-w-md lg:max-w-none">
                        <div class="rounded-3xl bg-white p-4 sm:p-5 shadow-2xl text-navy">
                            <!-- Clean Modern House Painting Vector Scene -->
                            <div class="rounded-2xl overflow-hidden bg-gradient-to-b from-[#E0F2FE] to-[#F0FDFA] aspect-[4/3] relative flex items-center justify-center">
                                <svg viewBox="0 0 420 315" class="w-full h-full">
                                    <!-- Sky & Sun -->
                                    <circle cx="350" cy="55" r="28" fill="#FDE68A" opacity="0.8"/>
                                    <!-- Modern Two-Story House -->
                                    <!-- House Shadow -->
                                    <ellipse cx="210" cy="278" rx="165" ry="12" fill="#0F2942" opacity="0.12"/>
                                    <!-- Main Structure Left (Newly Painted Clean Off-White & Teal Accent) -->
                                    <rect x="65" y="125" width="165" height="148" rx="4" fill="#FFFFFF" stroke="#CBD5E1" stroke-width="2"/>
                                    <!-- Roof Left -->
                                    <polygon points="52,128 148,68 242,128" fill="#0F2942"/>
                                    <!-- Right Wing (Freshly Painted Navy/Teal Accent Wall) -->
                                    <rect x="220" y="148" width="135" height="125" rx="4" fill="#0D9488"/>
                                    <polygon points="212,150 288,100 365,150" fill="#1B3F63"/>
                                    <!-- Windows -->
                                    <rect x="92" y="148" width="44" height="42" rx="4" fill="#BAE6FD" stroke="#0F2942" stroke-width="2.5"/>
                                    <line x1="114" y1="148" x2="114" y2="190" stroke="#0F2942" stroke-width="2"/>
                                    <rect x="158" y="148" width="44" height="42" rx="4" fill="#BAE6FD" stroke="#0F2942" stroke-width="2.5"/>
                                    <line x1="180" y1="148" x2="180" y2="190" stroke="#0F2942" stroke-width="2"/>
                                    <!-- Door -->
                                    <rect x="128" y="210" width="38" height="63" rx="3" fill="#F59E0B" stroke="#0F2942" stroke-width="2.5"/>
                                    <circle cx="158" cy="243" r="3" fill="#0F2942"/>
                                    <!-- Right Wing Window -->
                                    <rect x="255" y="175" width="65" height="50" rx="4" fill="#E0F2FE" stroke="#FFFFFF" stroke-width="2.5"/>
                                    <line x1="287" y1="175" x2="287" y2="225" stroke="#FFFFFF" stroke-width="2"/>
                                    <!-- Paint Roller & Fresh Swatch Overlay -->
                                    <g transform="translate(275, 42) rotate(-12)">
                                        <rect x="0" y="0" width="76" height="26" rx="8" fill="#F59E0B" stroke="#0F2942" stroke-width="2.5"/>
                                        <path d="M76 13 H92 V36 H46 V55" fill="none" stroke="#0F2942" stroke-width="4" stroke-linecap="round" stroke-linejoin="round"/>
                                        <rect x="38" y="52" width="16" height="36" rx="6" fill="#0D9488" stroke="#0F2942" stroke-width="2.5"/>
                                    </g>
                                    <!-- Clean Bushes -->
                                    <circle cx="62" cy="264" r="16" fill="#10B981"/>
                                    <circle cx="80" cy="268" r="12" fill="#059669"/>
                                    <circle cx="355" cy="265" r="15" fill="#10B981"/>
                                </svg>

                                <!-- Official Paint Partner Badge inside image -->
                                <div class="absolute bottom-3 left-3 right-3 bg-white/95 backdrop-blur rounded-xl px-3.5 py-2.5 shadow-md flex items-center justify-between border border-slate-100">
                                    <div class="flex items-center gap-2">
                                        <span class="w-2.5 h-2.5 rounded-full bg-teal"></span>
                                        <span class="font-heading font-semibold text-xs text-navy">มาตรฐานสีแท้ 100%</span>
                                    </div>
                                    <div class="flex items-center gap-2 font-heading font-bold text-xs">
                                        <span class="px-2 py-0.5 rounded bg-red-50 text-red-600">TOA</span>
                                        <span class="px-2 py-0.5 rounded bg-blue-50 text-blue-700">Dulux</span>
                                        <span class="px-2 py-0.5 rounded bg-emerald-50 text-emerald-700">Beger</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Stats Bar below Hero Image -->
                            <div class="grid grid-cols-3 gap-2 pt-4 text-center divide-x divide-slate-200">
                                <div>
                                    <p class="font-heading font-bold text-xl sm:text-2xl text-navy">1,250+</p>
                                    <p class="text-xs text-slate-500">หลังคาเรือนที่ดูแล</p>
                                </div>
                                <div>
                                    <p class="font-heading font-bold text-xl sm:text-2xl text-teal">10+ ปี</p>
                                    <p class="text-xs text-slate-500">ประสบการณ์ทีมช่าง</p>
                                </div>
                                <div>
                                    <p class="font-heading font-bold text-xl sm:text-2xl text-amber-hover">5 ปี</p>
                                    <p class="text-xs text-slate-500">รับประกันผลงาน</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 3. Trust Badges / จุดเด่นบริการ (Why Choose Us) -->
    <section class="py-16 sm:py-20 bg-white border-b border-slate-200/70">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">WHY CHOOSE PROPAINT</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">ทำไมเจ้าของบ้านกว่า 1,250 หลัง ถึงเลือกเรา</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">เราทำงานด้วยมาตรฐานระดับวิศวกรรม ใส่ใจทุกรายละเอียดเสมือนทาสีบ้านของเราเอง</p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Card 1 -->
                <div class="p-6 rounded-2xl bg-offwhite border border-slate-200/80 hover:border-teal/50 hover:shadow-lg transition duration-300 group">
                    <div class="w-12 h-12 rounded-xl bg-navy text-amber flex items-center justify-center mb-4 group-hover:scale-110 transition">
                        <i data-lucide="hard-hat" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-heading font-semibold text-lg text-navy mb-2">ช่างชำนาญการประสบการณ์กว่า 10 ปี</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">ทีมช่างประจำของบริษัทผ่านการอบรมมาตรฐานการทาสีจากแบรนด์สีชั้นนำ ไม่ใช่ช่างรายวันทั่วไป</p>
                </div>

                <!-- Card 2 -->
                <div class="p-6 rounded-2xl bg-offwhite border border-slate-200/80 hover:border-teal/50 hover:shadow-lg transition duration-300 group">
                    <div class="w-12 h-12 rounded-xl bg-teal text-white flex items-center justify-center mb-4 group-hover:scale-110 transition">
                        <i data-lucide="award" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-heading font-semibold text-lg text-navy mb-2">ใช้วัสดุสีเกรดพรีเมียมแท้ 100%</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">เบิกสีใหม่จากศูนย์ตัวแทนจำหน่าย TOA, Dulux, Beger และ Jotun เปิดถังให้ลูกค้าตรวจสอบหน้างานทุกถัง</p>
                </div>

                <!-- Card 3 -->
                <div class="p-6 rounded-2xl bg-offwhite border border-slate-200/80 hover:border-teal/50 hover:shadow-lg transition duration-300 group">
                    <div class="w-12 h-12 rounded-xl bg-amber text-navy flex items-center justify-center mb-4 group-hover:scale-110 transition">
                        <i data-lucide="sparkles" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-heading font-semibold text-lg text-navy mb-2">คลุมเฟอร์นิเจอร์ & เก็บกวาดสะอาด</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">ปูพลาสติกและเทปป้องกันพื้น วงกบ และเฟอร์นิเจอร์ทุกชิ้น พร้อมทำความสะอาดคืนพื้นที่เรียบร้อยหลังจบงาน</p>
                </div>

                <!-- Card 4 -->
                <div class="p-6 rounded-2xl bg-offwhite border border-slate-200/80 hover:border-teal/50 hover:shadow-lg transition duration-300 group">
                    <div class="w-12 h-12 rounded-xl bg-navy text-teal-light flex items-center justify-center mb-4 group-hover:scale-110 transition">
                        <i data-lucide="file-check-2" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-heading font-semibold text-lg text-navy mb-2">รับประกันผลงานเป็นลายลักษณ์อักษร</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">ออกใบรับประกันผลงานสูงสุด 5 ปี หากเกิดปัญหาสีลอกล่อน พอง หรือซีดจางผิดปกติ ดูแลแก้ไขให้ฟรี</p>
                </div>

                <!-- Card 5 -->
                <div class="p-6 rounded-2xl bg-offwhite border border-slate-200/80 hover:border-teal/50 hover:shadow-lg transition duration-300 group">
                    <div class="w-12 h-12 rounded-xl bg-teal text-white flex items-center justify-center mb-4 group-hover:scale-110 transition">
                        <i data-lucide="ruler" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-heading font-semibold text-lg text-navy mb-2">ประเมินหน้างานฟรี ไม่มีค่าใช้จ่าย</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">ส่งทีมวิศวกรประเมินราคาเข้าวัดพื้นที่ ตรวจเช็กความชื้นผนัง และทำใบเสนอราคาละเอียดฟรี ไม่มัดมือชก</p>
                </div>

                <!-- Card 6 -->
                <div class="p-6 rounded-2xl bg-offwhite border border-slate-200/80 hover:border-teal/50 hover:shadow-lg transition duration-300 group">
                    <div class="w-12 h-12 rounded-xl bg-amber text-navy flex items-center justify-center mb-4 group-hover:scale-110 transition">
                        <i data-lucide="calendar-check" class="w-6 h-6"></i>
                    </div>
                    <h3 class="font-heading font-semibold text-lg text-navy mb-2">สัญญาระบุวันเสร็จชัดเจน ไม่ทิ้งงาน</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">แบ่งชำระเงินเป็นงวดตามความคืบหน้าของงานจริง มีโฟร์แมนรายงานความคืบหน้าผ่าน LINE ทุกวัน</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. บริการของเรา (Our Services) -->
    <section id="services" class="py-16 sm:py-20 bg-offwhite">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">OUR SERVICES</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">บริการรับทาสีและซ่อมแซมครบวงจร</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">ครอบคลุมทุกความต้องการ ทั้งบ้านอยู่อาศัย คอนโดมิเนียม อาคารพาณิชย์ และโรงงาน</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Service 1: Indoor -->
                <div class="bg-white rounded-3xl overflow-hidden border border-slate-200/80 shadow-sm hover:shadow-xl transition flex flex-col justify-between group">
                    <div>
                        <div class="h-40 bg-gradient-to-br from-navy-soft to-teal-soft p-6 flex items-center justify-between relative">
                            <div>
                                <span class="px-3 py-1 rounded-full bg-white text-navy font-heading text-xs font-semibold shadow-sm">ยอดนิยม</span>
                                <p class="font-heading font-bold text-navy text-lg mt-3">เริ่มต้น 45 บ./ตร.ม.</p>
                            </div>
                            <div class="w-16 h-16 rounded-2xl bg-white shadow-md flex items-center justify-center text-teal group-hover:scale-110 transition">
                                <i data-lucide="sofa" class="w-8 h-8"></i>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="font-heading font-bold text-xl text-navy mb-2">ทาสีภายใน (Indoor Painting)</h3>
                            <p class="text-sm text-slate-600 leading-relaxed mb-4">
                                ทาสีผนังและฝ้าเพดานภายในบ้าน คอนโด ออฟฟิศ ใช้สีสูตรน้ำไร้กลิ่นฉุน (Low VOCs) เข้าอยู่ได้ทันทีหลังทาสีเสร็จ
                            </p>
                            <ul class="space-y-2 text-xs sm:text-sm text-slate-700">
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> สีเช็ดล้างทำความสะอาดง่าย</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> ยับยั้งแบคทีเรียและเชื้อรา</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> คลุมเฟอร์นิเจอร์และพื้นทุกจุด</li>
                            </ul>
                        </div>
                    </div>
                    <div class="px-6 pb-6">
                        <button onclick="selectServiceAndScroll('ทาสีภายใน (Indoor)')" class="w-full py-3 rounded-xl bg-navy-soft hover:bg-navy text-navy hover:text-white font-heading font-semibold text-sm transition flex items-center justify-center gap-2">
                            ขอประเมินราคางานนี้ <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>

                <!-- Service 2: Exterior -->
                <div class="bg-white rounded-3xl overflow-hidden border border-slate-200/80 shadow-sm hover:shadow-xl transition flex flex-col justify-between group">
                    <div>
                        <div class="h-40 bg-gradient-to-br from-amber-soft to-navy-soft p-6 flex items-center justify-between relative">
                            <div>
                                <span class="px-3 py-1 rounded-full bg-amber text-navy font-heading text-xs font-semibold shadow-sm">ทนแดด ทนฝน</span>
                                <p class="font-heading font-bold text-navy text-lg mt-3">เริ่มต้น 55 บ./ตร.ม.</p>
                            </div>
                            <div class="w-16 h-16 rounded-2xl bg-white shadow-md flex items-center justify-center text-navy group-hover:scale-110 transition">
                                <i data-lucide="home" class="w-8 h-8"></i>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="font-heading font-bold text-xl text-navy mb-2">ทาสีภายนอกอาคาร & บ้าน</h3>
                            <p class="text-sm text-slate-600 leading-relaxed mb-4">
                                ทาสีบ้านเดี่ยว ทาวน์โฮม อาคารพาณิชย์ พร้อมฉีดล้างทำความสะอาดตะไคร่น้ำด้วยเครื่องแรงดันสูงก่อนลงสีรองพื้น
                            </p>
                            <ul class="space-y-2 text-xs sm:text-sm text-slate-700">
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> สะท้อนความร้อน ลดอุณหภูมิบ้าน</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> ฟิล์มสีทนทานสูงสุด 10-15 ปี</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> มีนั่งร้านมาตรฐานปลอดภัยครบชุด</li>
                            </ul>
                        </div>
                    </div>
                    <div class="px-6 pb-6">
                        <button onclick="selectServiceAndScroll('ทาสีภายนอก (Exterior)')" class="w-full py-3 rounded-xl bg-navy-soft hover:bg-navy text-navy hover:text-white font-heading font-semibold text-sm transition flex items-center justify-center gap-2">
                            ขอประเมินราคางานนี้ <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>

                <!-- Service 3: Roof / Fence / Metal & Wood -->
                <div class="bg-white rounded-3xl overflow-hidden border border-slate-200/80 shadow-sm hover:shadow-xl transition flex flex-col justify-between group">
                    <div>
                        <div class="h-40 bg-gradient-to-br from-teal-soft to-slate-100 p-6 flex items-center justify-between relative">
                            <div>
                                <span class="px-3 py-1 rounded-full bg-white text-teal-dark font-heading text-xs font-semibold shadow-sm">งานเฉพาะทาง</span>
                                <p class="font-heading font-bold text-navy text-lg mt-3">ประเมินตามพื้นที่</p>
                            </div>
                            <div class="w-16 h-16 rounded-2xl bg-white shadow-md flex items-center justify-center text-amber-hover group-hover:scale-110 transition">
                                <i data-lucide="fence" class="w-8 h-8"></i>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="font-heading font-bold text-xl text-navy mb-2">ทาสีหลังคา รั้ว เหล็ก และไม้</h3>
                            <p class="text-sm text-slate-600 leading-relaxed mb-4">
                                คืนความสวยงามให้หลังคากระเบื้อง เมทัลชีท ประตูรั้วเหล็กดัด ระแนงไม้ และพื้นลานจอดรถ ด้วยสีเฉพาะทางยึดเกาะสูง
                            </p>
                            <ul class="space-y-2 text-xs sm:text-sm text-slate-700">
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> ขัดสนิมและทารองพื้นกันสนิม</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> สีย้อมไม้ / สีทาหลังคากันเชื้อรา</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> สีทาพื้นอีพ็อกซี่ / พื้นปูนลานจอด</li>
                            </ul>
                        </div>
                    </div>
                    <div class="px-6 pb-6">
                        <button onclick="selectServiceAndScroll('ทาสีรั้ว/หลังคา/งานเหล็ก-ไม้')" class="w-full py-3 rounded-xl bg-navy-soft hover:bg-navy text-navy hover:text-white font-heading font-semibold text-sm transition flex items-center justify-center gap-2">
                            ขอประเมินราคางานนี้ <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>

                <!-- Service 4: Waterproofing & Crack Repair -->
                <div class="bg-white rounded-3xl overflow-hidden border border-slate-200/80 shadow-sm hover:shadow-xl transition flex flex-col justify-between group">
                    <div>
                        <div class="h-40 bg-gradient-to-br from-navy-soft to-slate-200 p-6 flex items-center justify-between relative">
                            <div>
                                <span class="px-3 py-1 rounded-full bg-navy text-white font-heading text-xs font-semibold shadow-sm">แก้ปัญหาตรงจุด</span>
                                <p class="font-heading font-bold text-navy text-lg mt-3">งานซ่อม & กันซึม</p>
                            </div>
                            <div class="w-16 h-16 rounded-2xl bg-white shadow-md flex items-center justify-center text-navy group-hover:scale-110 transition">
                                <i data-lucide="droplets" class="w-8 h-8"></i>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="font-heading font-bold text-xl text-navy mb-2">ซ่อมรอยแตกร้าว & กันซึมดาดฟ้า</h3>
                            <p class="text-sm text-slate-600 leading-relaxed mb-4">
                                แก้ไขปัญหารอยร้าวผนัง รอยรั่วซึมขอบหน้าต่าง ดาดฟ้า และผนังชื้นลอกล่อน ด้วยวัสดุอะคริลิกและโพลียูรีเทนเกรดอุตสาหกรรม
                            </p>
                            <ul class="space-y-2 text-xs sm:text-sm text-slate-700">
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> โป๊วเก็บทุกรอยร้าวด้วย PU Sealant</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> ระบบกันซึมดาดฟ้า 3-5 ชั้น</li>
                                <li class="flex items-center gap-2"><i data-lucide="check" class="w-4 h-4 text-teal shrink-0"></i> ฉาบแต่งผิวเรียบเนียน (Skim Coat)</li>
                            </ul>
                        </div>
                    </div>
                    <div class="px-6 pb-6">
                        <button onclick="selectServiceAndScroll('ซ่อมรอยแตกร้าวและกันซึม')" class="w-full py-3 rounded-xl bg-navy-soft hover:bg-navy text-navy hover:text-white font-heading font-semibold text-sm transition flex items-center justify-center gap-2">
                            ขอประเมินราคางานนี้ <i data-lucide="arrow-right" class="w-4 h-4"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 5. ระบบคำนวณราคาทาสีเบื้องต้นแบบ Interactive (Cost Estimator Calculator) -->
    <section id="calculator" class="py-16 sm:py-24 bg-navy text-white relative overflow-hidden">
        <div class="absolute top-0 right-0 w-96 h-96 bg-teal/15 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute bottom-0 left-0 w-96 h-96 bg-amber/10 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="text-center max-w-2xl mx-auto mb-12">
                <span class="inline-flex items-center gap-1.5 px-3.5 py-1 rounded-full bg-amber/20 text-amber font-heading text-xs font-semibold mb-2">
                    <i data-lucide="calculator" class="w-3.5 h-3.5"></i> INTERACTIVE COST ESTIMATOR
                </span>
                <h2 class="text-2xl sm:text-4xl font-bold mt-1">คำนวณราคาทาสีบ้านเบื้องต้นได้ทันที</h2>
                <p class="text-slate-300 mt-2 text-sm sm:text-base">เลือกสเปกงานและขนาดพื้นที่ของคุณ ระบบจะคำนวณงบประมาณเบื้องต้น (รวมค่าแรงช่าง + ค่าสีและอุปกรณ์ครบชุด)</p>
            </div>

            <div class="bg-white text-navy rounded-3xl shadow-2xl overflow-hidden border border-white/20">
                <div class="grid grid-cols-1 lg:grid-cols-12">
                    <!-- Left Controls (7 Cols) -->
                    <div class="lg:col-span-7 p-6 sm:p-10 space-y-7">
                        <!-- Step 1: Scope of Work -->
                        <div>
                            <label class="block font-heading font-semibold text-base text-navy mb-3">
                                1. เลือกประเภทพื้นที่ที่ต้องการทาสี
                            </label>
                            <div class="grid grid-cols-3 gap-3" id="calc-scope-group">
                                <button type="button" onclick="setCalcOption('scope', 'indoor', this)" class="calc-scope-btn p-3.5 rounded-2xl border-2 border-teal bg-teal-soft text-navy font-heading font-semibold text-xs sm:text-sm text-center transition">
                                    <i data-lucide="sofa" class="w-5 h-5 mx-auto mb-1.5 text-teal"></i>
                                    ทาสีภายใน
                                </button>
                                <button type="button" onclick="setCalcOption('scope', 'outdoor', this)" class="calc-scope-btn p-3.5 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-slate-600 font-heading font-medium text-xs sm:text-sm text-center transition">
                                    <i data-lucide="sun" class="w-5 h-5 mx-auto mb-1.5 text-amber-hover"></i>
                                    ทาสีภายนอก
                                </button>
                                <button type="button" onclick="setCalcOption('scope', 'both', this)" class="calc-scope-btn p-3.5 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-slate-600 font-heading font-medium text-xs sm:text-sm text-center transition">
                                    <i data-lucide="home" class="w-5 h-5 mx-auto mb-1.5 text-navy"></i>
                                    ทาสีทั้งหลัง
                                </button>
                            </div>
                        </div>

                        <!-- Step 2: Property Type -->
                        <div>
                            <label class="block font-heading font-semibold text-base text-navy mb-3">
                                2. เลือกประเภทที่อยู่อาศัย
                            </label>
                            <div class="grid grid-cols-3 gap-3" id="calc-property-group">
                                <button type="button" onclick="setCalcOption('property', 'condo', this)" class="calc-prop-btn p-3 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-slate-600 font-heading font-medium text-xs sm:text-sm text-center transition">
                                    คอนโดมิเนียม
                                </button>
                                <button type="button" onclick="setCalcOption('property', 'townhome', this)" class="calc-prop-btn p-3 rounded-2xl border-2 border-teal bg-teal-soft text-navy font-heading font-semibold text-xs sm:text-sm text-center transition">
                                    ทาวน์โฮม
                                </button>
                                <button type="button" onclick="setCalcOption('property', 'detached', this)" class="calc-prop-btn p-3 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-slate-600 font-heading font-medium text-xs sm:text-sm text-center transition">
                                    บ้านเดี่ยว
                                </button>
                            </div>
                        </div>

                        <!-- Step 3: Area Size Slider & Input -->
                        <div>
                            <div class="flex items-center justify-between mb-2">
                                <label for="area-input" class="font-heading font-semibold text-base text-navy">
                                    3. พื้นที่ใช้สอยโดยประมาณ (ตร.ม.)
                                </label>
                                <div class="flex items-center gap-2">
                                    <input type="number" id="area-input" value="120" min="20" max="1000" oninput="syncAreaFromInput(this.value)" class="w-24 px-3 py-1.5 rounded-xl border border-slate-300 text-right font-heading font-bold text-navy focus:outline-none focus:border-teal">
                                    <span class="text-sm font-heading text-slate-500">ตร.ม.</span>
                                </div>
                            </div>
                            <input type="range" id="area-slider" min="20" max="600" step="5" value="120" oninput="syncAreaFromSlider(this.value)" class="w-full custom-slider my-2">
                            <div class="flex justify-between text-xs text-slate-400 font-heading">
                                <span>20 ตร.ม. (คอนโดเล็ก)</span>
                                <span>150 ตร.ม. (ทาวน์โฮม)</span>
                                <span>300+ ตร.ม. (บ้านเดี่ยว)</span>
                            </div>
                        </div>

                        <!-- Step 4: Paint Grade -->
                        <div>
                            <label class="block font-heading font-semibold text-base text-navy mb-3">
                                4. เลือกเกรดสีที่ต้องการ
                            </label>
                            <div class="space-y-2.5" id="calc-grade-group">
                                <button type="button" onclick="setCalcOption('grade', 'standard', this)" class="calc-grade-btn w-full p-3.5 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-left flex items-center justify-between transition">
                                    <div>
                                        <span class="font-heading font-semibold text-sm text-navy block">เกรดมาตรฐาน (Standard Shield)</span>
                                        <span class="text-xs text-slate-500">สีน้ำอะคริลิกแท้ 100% ทนทาน 5-7 ปี (รับประกันงาน 2 ปี)</span>
                                    </div>
                                    <span class="font-heading font-bold text-xs px-2.5 py-1 rounded-lg bg-slate-100 text-slate-700">ประหยัด</span>
                                </button>

                                <button type="button" onclick="setCalcOption('grade', 'premium', this)" class="calc-grade-btn w-full p-3.5 rounded-2xl border-2 border-teal bg-teal-soft text-left flex items-center justify-between transition">
                                    <div>
                                        <span class="font-heading font-semibold text-sm text-navy block">เกรดพรีเมียมเช็ดล้างได้ (Ultra Clean / SuperShield)</span>
                                        <span class="text-xs text-slate-600">เช็ดล้างคราบสกปรกง่าย ไร้กลิ่นฉุน ทนทาน 10 ปี (รับประกันงาน 3 ปี)</span>
                                    </div>
                                    <span class="font-heading font-bold text-xs px-2.5 py-1 rounded-lg bg-teal text-white">แนะนำ</span>
                                </button>

                                <button type="button" onclick="setCalcOption('grade', 'flagship', this)" class="calc-grade-btn w-full p-3.5 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-left flex items-center justify-between transition">
                                    <div>
                                        <span class="font-heading font-semibold text-sm text-navy block">เกรดสูงสุดกันความร้อน 15 ปี (Flagship Heat-Reflect)</span>
                                        <span class="text-xs text-slate-500">สะท้อนความร้อนสูงสุด ลดอุณหภูมิในบ้าน ฟิล์มสีแกร่ง 15 ปี (รับประกันงาน 5 ปี)</span>
                                    </div>
                                    <span class="font-heading font-bold text-xs px-2.5 py-1 rounded-lg bg-amber-soft text-amber-hover">พรีเมียมสุด</span>
                                </button>
                            </div>
                        </div>
                    </div>

                    <!-- Right Result Summary (5 Cols) -->
                    <div class="lg:col-span-5 bg-gradient-to-br from-navy-soft via-[#E6EEF6] to-teal-soft p-6 sm:p-10 flex flex-col justify-between border-t lg:border-t-0 lg:border-l border-slate-200">
                        <div>
                            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-white text-teal-dark font-heading text-xs font-semibold shadow-sm mb-4">
                                <i data-lucide="sparkles" class="w-3.5 h-3.5"></i> ผลการประเมินเบื้องต้น
                            </div>

                            <h3 class="font-heading font-bold text-lg text-navy">งบประมาณโดยประมาณการ</h3>
                            <p class="text-xs text-slate-500 mt-0.5">รวมค่าแรงช่าง + ค่าสีจริง + สีรองพื้น + อุปกรณ์คลุมกันเปื้อน</p>

                            <!-- Estimated Price Box -->
                            <div class="my-6 p-6 rounded-2xl bg-white shadow-md border border-slate-200/80 text-center">
                                <p class="text-xs font-heading text-slate-500 uppercase tracking-wider mb-1">ช่วงราคาประเมินสุทธิ</p>
                                <div class="font-heading font-bold text-2xl sm:text-3xl text-navy" id="calc-price-display">
                                    18,500 - 22,000 บาท
                                </div>
                                <div class="mt-3 pt-3 border-t border-slate-100 flex items-center justify-center gap-4 text-xs text-slate-600">
                                    <span class="flex items-center gap-1">
                                        <i data-lucide="clock" class="w-3.5 h-3.5 text-teal"></i>
                                        ระยะเวลา: <strong id="calc-days-display">3-4 วัน</strong>
                                    </span>
                                    <span class="flex items-center gap-1">
                                        <i data-lucide="shield" class="w-3.5 h-3.5 text-amber-hover"></i>
                                        ประกัน: <strong id="calc-warranty-display">3 ปี</strong>
                                    </span>
                                </div>
                            </div>

                            <!-- Selected Specs Breakdown -->
                            <div class="space-y-2.5 text-sm bg-white/70 rounded-2xl p-4 border border-white">
                                <div class="flex justify-between">
                                    <span class="text-slate-500">ประเภทงาน:</span>
                                    <span class="font-heading font-semibold text-navy" id="summary-scope">ทาสีภายใน</span>
                                </div>
                                <div class="flex justify-between">
                                    <span class="text-slate-500">ที่อยู่อาศัย:</span>
                                    <span class="font-heading font-semibold text-navy" id="summary-property">ทาวน์โฮม (120 ตร.ม.)</span>
                                </div>
                                <div class="flex justify-between">
                                    <span class="text-slate-500">เกรดสี:</span>
                                    <span class="font-heading font-semibold text-teal-dark" id="summary-grade">เกรดพรีเมียมเช็ดล้างได้</span>
                                </div>
                            </div>
                        </div>

                        <div class="mt-6 space-y-3">
                            <button type="button" onclick="transferEstimateToForm()" class="w-full py-4 px-6 rounded-2xl bg-amber hover:bg-amber-hover text-navy font-heading font-bold text-base shadow-lg shadow-amber/25 transition transform hover:-translate-y-0.5 flex items-center justify-center gap-2">
                                <i data-lucide="send" class="w-5 h-5"></i>
                                ส่งข้อมูลนี้เพื่อขอใบเสนอราคาจริง
                            </button>
                            <p class="text-[11px] text-center text-slate-500">
                                *ราคาอาจปรับเพิ่ม-ลดตามสภาพพื้นผิวและรอยแตกร้าวจริง นัดสำรวจหน้างานฟรี!
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. แกลเลอรีผลงานที่ผ่านมา (Portfolio & Before/After) -->
    <section id="portfolio" class="py-16 sm:py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-10">
                <div>
                    <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">PORTFOLIO & BEFORE/AFTER</span>
                    <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">ผลงานความประทับใจที่ผ่านมา</h2>
                    <p class="text-slate-600 mt-1 text-sm sm:text-base">เลื่อนแถบเปรียบเทียบ ก่อนทาสี (Before) และ หลังทาสี (After) เพื่อเห็นความเปลี่ยนแปลง</p>
                </div>

                <!-- Category Filter Buttons -->
                <div class="inline-flex flex-wrap p-1.5 rounded-2xl bg-offwhite border border-slate-200 self-start md:self-auto">
                    <button onclick="filterPortfolio('all', this)" class="port-filter-btn px-4 py-2 rounded-xl font-heading text-xs sm:text-sm font-semibold bg-navy text-white transition">
                        ทั้งหมด
                    </button>
                    <button onclick="filterPortfolio('detached', this)" class="port-filter-btn px-4 py-2 rounded-xl font-heading text-xs sm:text-sm font-medium text-slate-600 hover:text-navy transition">
                        บ้านเดี่ยว
                    </button>
                    <button onclick="filterPortfolio('townhome', this)" class="port-filter-btn px-4 py-2 rounded-xl font-heading text-xs sm:text-sm font-medium text-slate-600 hover:text-navy transition">
                        ทาวน์โฮม
                    </button>
                    <button onclick="filterPortfolio('condo', this)" class="port-filter-btn px-4 py-2 rounded-xl font-heading text-xs sm:text-sm font-medium text-slate-600 hover:text-navy transition">
                        คอนโด/อาคาร
                    </button>
                </div>
            </div>

            <!-- Interactive Before/After Showcase Spotlight -->
            <div class="mb-12 bg-offwhite rounded-3xl p-5 sm:p-8 border border-slate-200/80 shadow-sm">
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                    <div class="lg:col-span-7">
                        <!-- Interactive Slider Box -->
                        <div id="ba-slider-box" class="ba-container rounded-2xl aspect-[16/10] shadow-lg border-2 border-white">
                            <!-- BEFORE LAYER (Base) -->
                            <div class="w-full h-full bg-[#CBD5E1] relative flex items-center justify-center">
                                <svg viewBox="0 0 600 375" class="w-full h-full object-cover">
                                    <!-- Dull Old Sky -->
                                    <rect width="600" height="375" fill="#CBD5E1"/>
                                    <!-- Old Peeling/Stained House -->
                                    <rect x="90" y="135" width="420" height="220" fill="#D6D3D1"/>
                                    <polygon points="70,138 300,45 530,138" fill="#57534E"/>
                                    <!-- Stains & Cracks on Old Wall -->
                                    <path d="M130 160 Q145 190 125 225" stroke="#78716C" stroke-width="3" fill="none"/>
                                    <path d="M430 180 Q415 215 445 250" stroke="#78716C" stroke-width="3" fill="none"/>
                                    <ellipse cx="160" cy="315" rx="45" ry="25" fill="#78716C" opacity="0.35"/>
                                    <ellipse cx="450" cy="320" rx="55" ry="22" fill="#78716C" opacity="0.35"/>
                                    <!-- Old Windows -->
                                    <rect x="145" y="175" width="75" height="70" fill="#64748B" stroke="#475569" stroke-width="4"/>
                                    <rect x="380" y="175" width="75" height="70" fill="#64748B" stroke="#475569" stroke-width="4"/>
                                    <!-- Old Door -->
                                    <rect x="265" y="235" width="70" height="120" fill="#78716C" stroke="#44403C" stroke-width="4"/>
                                </svg>
                                <span class="absolute top-4 right-4 bg-slate-800/80 text-white font-heading text-xs font-semibold px-3 py-1.5 rounded-lg backdrop-blur-sm">
                                    BEFORE (ก่อนทาสี)
                                </span>
                            </div>

                            <!-- AFTER LAYER (Clipped by width) -->
                            <div id="ba-after-layer" class="ba-after-wrapper" style="width: 50%;">
                                <div class="w-full h-full relative" style="width: 100%;">
                                    <svg viewBox="0 0 600 375" preserveAspectRatio="xMinYMid slice" class="h-full" style="width: var(--ba-full-width, 600px); max-width: none;">
                                        <!-- Bright Clear Sky -->
                                        <rect width="600" height="375" fill="#E0F2FE"/>
                                        <!-- Newly Painted Modern House -->
                                        <rect x="90" y="135" width="420" height="220" fill="#FFFFFF"/>
                                        <!-- Teal Accent Center Pillar -->
                                        <rect x="245" y="135" width="110" height="220" fill="#0D9488"/>
                                        <!-- Crisp Navy Roof -->
                                        <polygon points="70,138 300,45 530,138" fill="#0F2942"/>
                                        <!-- Clean Windows -->
                                        <rect x="145" y="175" width="75" height="70" fill="#BAE6FD" stroke="#0F2942" stroke-width="4"/>
                                        <line x1="182" y1="175" x2="182" y2="245" stroke="#0F2942" stroke-width="3"/>
                                        <rect x="380" y="175" width="75" height="70" fill="#BAE6FD" stroke="#0F2942" stroke-width="4"/>
                                        <line x1="417" y1="175" x2="417" y2="245" stroke="#0F2942" stroke-width="3"/>
                                        <!-- Warm Amber Modern Door -->
                                        <rect x="265" y="235" width="70" height="120" fill="#F59E0B" stroke="#0F2942" stroke-width="4"/>
                                        <circle cx="322" cy="295" r="5" fill="#0F2942"/>
                                    </svg>
                                </div>
                                <span class="absolute top-4 left-4 bg-teal text-white font-heading text-xs font-semibold px-3 py-1.5 rounded-lg shadow-sm whitespace-nowrap">
                                    AFTER (หลังทาสีใหม่)
                                </span>
                            </div>

                            <!-- Draggable Divider -->
                            <div id="ba-divider" class="ba-divider" style="left: 50%;">
                                <div class="ba-handle">
                                    <i data-lucide="move-horizontal" class="w-5 h-5"></i>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="lg:col-span-5 space-y-4">
                        <span class="px-3 py-1 rounded-full bg-teal-soft text-teal-dark font-heading text-xs font-semibold">
                            เคสรีโนเวทบ้านเดี่ยว 2 ชั้น • หมู่บ้านมัณฑนา บางนา
                        </span>
                        <h3 class="font-heading font-bold text-xl sm:text-2xl text-navy">
                            รีโนเวทสีภายนอกบ้านเดี่ยวอายุ 12 ปี แก้ปัญหารอยแตกลายงาและคราบตะไคร่น้ำ
                        </h3>
                        <p class="text-sm text-slate-600 leading-relaxed">
                            เจ้าของบ้านพบปัญหาสีเดิมซีดจางและมีรอยร้าวเส้นเล็กทั่วผนัง ทีมงาน ProPaint เข้าฉีดล้างด้วยเครื่องแรงดันสูง โป๊วเก็บทุกรอยร้าวด้วย PU Sealant ลงรองพื้นปูนเก่าสูตรน้ำมัน และทาทับหน้าด้วยสี <strong>TOA SuperShield</strong> 2 เที่ยว
                        </p>
                        <div class="grid grid-cols-2 gap-3 pt-2">
                            <div class="p-3 rounded-xl bg-white border border-slate-200">
                                <span class="text-xs text-slate-500 block">พื้นที่ทาสีรวม</span>
                                <span class="font-heading font-bold text-navy text-sm">280 ตร.ม.</span>
                            </div>
                            <div class="p-3 rounded-xl bg-white border border-slate-200">
                                <span class="text-xs text-slate-500 block">ระยะเวลาดำเนินการ</span>
                                <span class="font-heading font-bold text-teal text-sm">5 วันเสร็จสมบูรณ์</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Portfolio Grid (Rendered by JS) -->
            <div id="portfolio-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Items injected by JS -->
            </div>
        </div>
    </section>

    <!-- 7. ขั้นตอนการทำงาน (4-Step Process) -->
    <section id="process" class="py-16 sm:py-20 bg-offwhite border-y border-slate-200/80">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-2xl mx-auto mb-14">
                <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">OUR 4-STEP PROCESS</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">ขั้นตอนการทำงานมาตรฐาน ProPaint</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">โปร่งใส ตรวจสอบได้ทุกขั้นตอน เพื่อผลลัพธ์ที่สวยงามและติดทนนานที่สุด</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 relative">
                <!-- Step 1 -->
                <div class="bg-white p-6 rounded-3xl border border-slate-200 shadow-sm relative">
                    <div class="w-12 h-12 rounded-2xl bg-navy text-amber font-heading font-bold text-xl flex items-center justify-center mb-5 shadow-md">
                        01
                    </div>
                    <h3 class="font-heading font-bold text-lg text-navy mb-2">นัดสำรวจหน้างาน & ประเมินราคาฟรี</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">
                        ทีมงานเข้าวัดพื้นที่จริง ตรวจเช็กความชื้นและรอยร้าวของผนัง พร้อมแนะนำเฉดสีและส่งใบเสนอราคาชัดเจนภายใน 24 ชม.
                    </p>
                </div>

                <!-- Step 2 -->
                <div class="bg-white p-6 rounded-3xl border border-slate-200 shadow-sm relative">
                    <div class="w-12 h-12 rounded-2xl bg-teal text-white font-heading font-bold text-xl flex items-center justify-center mb-5 shadow-md">
                        02
                    </div>
                    <h3 class="font-heading font-bold text-lg text-navy mb-2">เตรียมพื้นผิว ซ่อมรอยร้าว & คลุมป้องกัน</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">
                        ปูพลาสติกคลุมพื้นและเฟอร์นิเจอร์ ขัดล้างคราบสีเก่า โป๊วซ่อมรอยแตกร้าวให้เรียบเนียนก่อนเริ่มลงสีจริง
                    </p>
                </div>

                <!-- Step 3 -->
                <div class="bg-white p-6 rounded-3xl border border-slate-200 shadow-sm relative">
                    <div class="w-12 h-12 rounded-2xl bg-amber text-navy font-heading font-bold text-xl flex items-center justify-center mb-5 shadow-md">
                        03
                    </div>
                    <h3 class="font-heading font-bold text-lg text-navy mb-2">ลงสีรองพื้นและสีจริงตามมาตรฐาน</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">
                        ทาสีรองพื้น 1 เที่ยวเพื่อการยึดเกาะสูงสุด และทาสีทับหน้า 2-3 เที่ยวด้วยสีแท้ 100% ไม่เจือจางน้ำเกินมาตรฐาน
                    </p>
                </div>

                <!-- Step 4 -->
                <div class="bg-white p-6 rounded-3xl border border-slate-200 shadow-sm relative">
                    <div class="w-12 h-12 rounded-2xl bg-navy text-teal-light font-heading font-bold text-xl flex items-center justify-center mb-5 shadow-md">
                        04
                    </div>
                    <h3 class="font-heading font-bold text-lg text-navy mb-2">ตรวจรับงาน ทำความสะอาด & รับประกัน</h3>
                    <p class="text-sm text-slate-600 leading-relaxed">
                        เก็บรายละเอียดความเรียบร้อย ทำความสะอาดพื้นที่ให้สะอาดเอี่ยม พร้อมส่งมอบใบรับประกันผลงานสูงสุด 5 ปี
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- 8. รีวิวจากลูกค้าจริง (Testimonials) & คำถามที่พบบ่อย (FAQ Accordion) -->
    <section id="reviews" class="py-16 sm:py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <!-- Testimonials -->
            <div class="text-center max-w-2xl mx-auto mb-12">
                <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">CLIENT TESTIMONIALS</span>
                <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">เสียงยืนยันจากเจ้าของบ้านที่ใช้บริการจริง</h2>
                <p class="text-slate-600 mt-2 text-sm sm:text-base">ความพึงพอใจ 4.9/5 ดาว จากลูกค้าทั่วกรุงเทพฯ ปริมณฑล และต่างจังหวัด</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-20">
                <!-- Review 1 -->
                <div class="p-6 sm:p-7 rounded-3xl bg-offwhite border border-slate-200/80 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-4">
                            <div class="flex text-amber gap-0.5">
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                            </div>
                            <span class="text-xs font-heading px-2.5 py-1 rounded-full bg-teal-soft text-teal-dark font-semibold">บ้านเดี่ยว 2 ชั้น</span>
                        </div>
                        <p class="text-slate-700 text-sm leading-relaxed italic">
                            "ประทับใจมากครับ ทีมช่างมาตรงเวลาทุกวัน คลุมเฟอร์นิเจอร์ในบ้านมิดชิดมาก ไม่มีสีหยดเลอะพื้นเลย โฟร์แมนส่งรูปอัปเดตงานในกลุ่มไลน์ทุกเย็น งานเสร็จไวกว่ากำหนด 1 วัน บ้านดูใหม่ขึ้นเยอะเลยครับ"
                        </p>
                    </div>
                    <div class="flex items-center gap-3 mt-6 pt-4 border-t border-slate-200">
                        <div class="w-10 h-10 rounded-full bg-navy text-white font-heading font-bold flex items-center justify-center">ธ</div>
                        <div>
                            <h4 class="font-heading font-semibold text-sm text-navy">คุณธนวัฒน์ รัตนไพศาล</h4>
                            <p class="text-xs text-slate-500">หมู่บ้านลัดดารมย์ ราชพฤกษ์</p>
                        </div>
                    </div>
                </div>

                <!-- Review 2 -->
                <div class="p-6 sm:p-7 rounded-3xl bg-offwhite border border-slate-200/80 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-4">
                            <div class="flex text-amber gap-0.5">
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                            </div>
                            <span class="text-xs font-heading px-2.5 py-1 rounded-full bg-amber-soft text-amber-hover font-semibold">ทาสีภายในคอนโด</span>
                        </div>
                        <p class="text-slate-700 text-sm leading-relaxed italic">
                            "รีโนเวททาสีคอนโด 2 ห้องนอนก่อนย้ายเข้าอยู่ ช่างเก็บขอบบัวและฝ้าเพดานคมกริบมากค่ะ ใช้สี TOA SuperShield ไร้กลิ่นฉุนจริงๆ ตอนเย็นเข้าไปตรวจงานไม่มีกลิ่นเหม็นสีเลย ราคายุติธรรมไม่บานปลายค่ะ"
                        </p>
                    </div>
                    <div class="flex items-center gap-3 mt-6 pt-4 border-t border-slate-200">
                        <div class="w-10 h-10 rounded-full bg-teal text-white font-heading font-bold flex items-center justify-center">ศ</div>
                        <div>
                            <h4 class="font-heading font-semibold text-sm text-navy">คุณศิริพร วรโชติ</h4>
                            <p class="text-xs text-slate-500">คอนโด Life Asoke - Rama 9</p>
                        </div>
                    </div>
                </div>

                <!-- Review 3 -->
                <div class="p-6 sm:p-7 rounded-3xl bg-offwhite border border-slate-200/80 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center justify-between mb-4">
                            <div class="flex text-amber gap-0.5">
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                                <i data-lucide="star" class="w-4 h-4 fill-amber"></i>
                            </div>
                            <span class="text-xs font-heading px-2.5 py-1 rounded-full bg-navy-soft text-navy font-semibold">ทาวน์โฮม & กันซึม</span>
                        </div>
                        <p class="text-slate-700 text-sm leading-relaxed italic">
                            "เคยเจอช่างทิ้งงานมาก่อน เลยระวังมาก แต่พอเจอ ProPaint สบายใจเลยครับ มีสัญญาชัดเจน ตรวจเช็กความชื้นผนังให้ก่อนทาสี และแก้ปัญหารอยร้าวรั่วซึมข้างบ้านจบในที่เดียว แนะนำเลยครับ"
                        </p>
                    </div>
                    <div class="flex items-center gap-3 mt-6 pt-4 border-t border-slate-200">
                        <div class="w-10 h-10 rounded-full bg-amber text-navy font-heading font-bold flex items-center justify-center">ก</div>
                        <div>
                            <h4 class="font-heading font-semibold text-sm text-navy">คุณกิตติพงษ์ เจริญสุข</h4>
                            <p class="text-xs text-slate-500">ทาวน์โฮม พลีโน่ รามอินทรา</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- FAQ Accordion -->
            <div id="faq" class="max-w-3xl mx-auto">
                <div class="text-center mb-10">
                    <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">FREQUENTLY ASKED QUESTIONS</span>
                    <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">คำถามที่พบบ่อย</h2>
                </div>

                <div class="space-y-3" id="faq-container">
                    <!-- FAQ 1 -->
                    <div class="border border-slate-200 rounded-2xl overflow-hidden bg-offwhite">
                        <button type="button" onclick="toggleFaq(0)" class="w-full px-6 py-4 text-left flex items-center justify-between font-heading font-semibold text-navy text-sm sm:text-base hover:bg-slate-100/70 transition">
                            <span>1. ทาสีบ้านช่วงหน้าฝนได้ไหม สีจะลอกล่อนหรือเปล่า?</span>
                            <i data-lucide="chevron-down" id="faq-icon-0" class="w-5 h-5 text-teal transition-transform duration-200 shrink-0"></i>
                        </button>
                        <div id="faq-content-0" class="hidden px-6 pb-5 text-sm text-slate-600 leading-relaxed border-t border-slate-200/60 pt-3">
                            <strong>สามารถทาสีได้ครับ</strong> หากเป็นการทาสีภายในสามารถทำได้ตามปกติ 100% ส่วนงานทาสีภายนอก ทีมช่างของเราจะใช้เครื่องวัดความชื้นผนัง (Moisture Meter) ตรวจสอบให้แน่ใจว่าค่าความชื้นต่ำกว่า 14% ก่อนลงสี และหยุดพักทาทันทีหากมีฝนตก เพื่อป้องกันสีพองหรือลอกล่อนในอนาคตครับ
                        </div>
                    </div>

                    <!-- FAQ 2 -->
                    <div class="border border-slate-200 rounded-2xl overflow-hidden bg-offwhite">
                        <button type="button" onclick="toggleFaq(1)" class="w-full px-6 py-4 text-left flex items-center justify-between font-heading font-semibold text-navy text-sm sm:text-base hover:bg-slate-100/70 transition">
                            <span>2. ลูกค้าต้องขนย้ายเฟอร์นิเจอร์ออกจากบ้านเองหรือไม่?</span>
                            <i data-lucide="chevron-down" id="faq-icon-1" class="w-5 h-5 text-teal transition-transform duration-200 shrink-0"></i>
                        </button>
                        <div id="faq-content-1" class="hidden px-6 pb-5 text-sm text-slate-600 leading-relaxed border-t border-slate-200/60 pt-3">
                            <strong>ไม่จำเป็นต้องขนย้ายออกครับ</strong> ทีมช่างของเราจะช่วยเลื่อนเฟอร์นิเจอร์มารวมไว้บริเวณกึ่งกลางห้อง และคลุมด้วยแผ่นพลาสติกใสกันฝุ่นและละอองสีอย่างมิดชิดทุกชิ้น พร้อมปูแผ่นรองพื้นกันเปื้อนตลอดแนวทางเดิน และจัดวางกลับเข้าที่เดิมหลังเสร็จงานครับ (แนะนำให้เก็บของมีค่าหรือของแตกหักง่ายไว้ในที่ปลอดภัย)
                        </div>
                    </div>

                    <!-- FAQ 3 -->
                    <div class="border border-slate-200 rounded-2xl overflow-hidden bg-offwhite">
                        <button type="button" onclick="toggleFaq(2)" class="w-full px-6 py-4 text-left flex items-center justify-between font-heading font-semibold text-navy text-sm sm:text-base hover:bg-slate-100/70 transition">
                            <span>3. ใช้เวลาทาสีบ้านกี่วัน และระหว่างทาสีสามารถพักอาศัยอยู่ในบ้านได้ไหม?</span>
                            <i data-lucide="chevron-down" id="faq-icon-2" class="w-5 h-5 text-teal transition-transform duration-200 shrink-0"></i>
                        </button>
                        <div id="faq-content-2" class="hidden px-6 pb-5 text-sm text-slate-600 leading-relaxed border-t border-slate-200/60 pt-3">
                            โดยทั่วไป คอนโดมิเนียมใช้เวลา <strong>2-3 วัน</strong>, ทาวน์โฮมใช้เวลา <strong>3-5 วัน</strong> และบ้านเดี่ยวทั้งหลังใช้เวลา <strong>5-10 วัน</strong> ขึ้นอยู่กับขนาดพื้นที่และงานซ่อมแซมพื้นผิว ระหว่างทาสีลูกค้าสามารถพักอาศัยอยู่ในบ้านได้ตามปกติ เพราะเราใช้สีสูตรน้ำเกรดพรีเมียมที่ไร้กลิ่นฉุน (Low VOCs) และปลอดภัยต่อเด็กและสัตว์เลี้ยงครับ
                        </div>
                    </div>

                    <!-- FAQ 4 -->
                    <div class="border border-slate-200 rounded-2xl overflow-hidden bg-offwhite">
                        <button type="button" onclick="toggleFaq(3)" class="w-full px-6 py-4 text-left flex items-center justify-between font-heading font-semibold text-navy text-sm sm:text-base hover:bg-slate-100/70 transition">
                            <span>4. การรับประกันผลงานสูงสุด 5 ปี ครอบคลุมอะไรบ้าง?</span>
                            <i data-lucide="chevron-down" id="faq-icon-3" class="w-5 h-5 text-teal transition-transform duration-200 shrink-0"></i>
                        </button>
                        <div id="faq-content-3" class="hidden px-6 pb-5 text-sm text-slate-600 leading-relaxed border-t border-slate-200/60 pt-3">
                            เรามอบใบรับประกันผลงานเป็นลายลักษณ์อักษร (2-5 ปี ตามแพ็กเกจเกรดสีที่เลือก) ครอบคลุมปัญหาสีพอง สีลอกล่อน สีหลุดร่อนเป็นฝุ่นผง หรือเชื้อราขึ้นผิดปกติอันเกิดจากกระบวนการเตรียมพื้นผิวและการทาสี โดยทีมช่างจะเข้าแก้ไขให้ฟรีไม่มีค่าใช้จ่ายเพิ่มเติมครับ
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 9. แบบฟอร์มขอใบเสนอราคา / นัดสำรวจหน้างาน (Lead Capture Form) -->
    <section id="quote-form" class="py-16 sm:py-24 bg-gradient-to-br from-navy-soft via-offwhite to-teal-soft border-t border-slate-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-start">
                <!-- Left Contact Info & Quick Channels -->
                <div class="lg:col-span-5 space-y-6">
                    <div>
                        <span class="text-teal font-heading font-semibold text-sm tracking-wider uppercase">FREE SITE SURVEY & QUOTE</span>
                        <h2 class="text-2xl sm:text-3xl font-bold text-navy mt-1">ขอใบเสนอราคาฟรี หรือนัดประเมินหน้างาน</h2>
                        <p class="text-slate-600 mt-2 text-sm sm:text-base leading-relaxed">
                            กรอกข้อมูลเบื้องต้นเพื่อให้ทีมวิศวกรประเมินราคาติดต่อกลับภายใน 30 นาที หรือแอดไลน์ส่งรูปถ่ายหน้างานเพื่อประเมินราคาเบื้องต้นได้ทันที
                        </p>
                    </div>

                    <!-- Direct Contact Cards -->
                    <div class="space-y-3.5">
                        <a href="tel:028889944" class="p-4 rounded-2xl bg-white border border-slate-200 shadow-sm hover:border-navy transition flex items-center gap-4 group">
                            <div class="w-12 h-12 rounded-xl bg-navy text-amber flex items-center justify-center shrink-0 group-hover:scale-105 transition">
                                <i data-lucide="phone-call" class="w-6 h-6"></i>
                            </div>
                            <div>
                                <p class="text-xs font-heading text-slate-500">สายด่วนปรึกษาช่าง (ทุกวัน 08:00 - 20:00 น.)</p>
                                <p class="font-heading font-bold text-lg text-navy">02-888-9944 / 089-456-7890</p>
                            </div>
                        </a>

                        <a href="#line-chat" onclick="openLineModal(event)" class="p-4 rounded-2xl bg-[#06C755] text-white shadow-md hover:bg-[#05B34C] transition flex items-center gap-4 group">
                            <div class="w-12 h-12 rounded-xl bg-white/20 flex items-center justify-center shrink-0 font-heading font-bold text-lg">
                                LINE
                            </div>
                            <div>
                                <p class="text-xs font-heading text-white/90">แอดไลน์ส่งรูปหน้างาน ประเมินไวใน 15 นาที</p>
                                <p class="font-heading font-bold text-lg">@propaint.th</p>
                            </div>
                        </a>

                        <div class="p-4 rounded-2xl bg-white border border-slate-200 shadow-sm flex items-center gap-4">
                            <div class="w-12 h-12 rounded-xl bg-blue-600 text-white flex items-center justify-center shrink-0">
                                <i data-lucide="facebook" class="w-6 h-6"></i>
                            </div>
                            <div>
                                <p class="text-xs font-heading text-slate-500">ติดตามผลงานอัปเดตทุกวัน</p>
                                <p class="font-heading font-bold text-base text-navy">ProPaint Thailand รับทาสีบ้านครบวงจร</p>
                            </div>
                        </div>
                    </div>

                    <!-- Service Area Badge -->
                    <div class="p-5 rounded-2xl bg-navy text-white">
                        <div class="flex items-center gap-2 font-heading font-semibold text-amber text-sm mb-1.5">
                            <i data-lucide="map-pin" class="w-4 h-4"></i> พื้นที่ให้บริการ
                        </div>
                        <p class="text-xs sm:text-sm text-slate-200 leading-relaxed">
                            กรุงเทพมหานคร, นนทบุรี, ปทุมธานี, สมุทรปราการ, สมุทรสาคร, นครปฐม, ชลบุรี, ระยอง และจังหวัดใกล้เคียง
                        </p>
                    </div>
                </div>

                <!-- Right Lead Capture Form -->
                <div class="lg:col-span-7">
                    <div class="bg-white rounded-3xl p-6 sm:p-10 shadow-xl border border-slate-200/80">
                        <form id="lead-capture-form" onsubmit="handleQuoteSubmit(event)" class="space-y-5">
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-5">
                                <div>
                                    <label for="lead-name" class="block font-heading font-medium text-sm text-navy mb-1.5">
                                        ชื่อ - นามสกุล <span class="text-red-500">*</span>
                                    </label>
                                    <input type="text" id="lead-name" required placeholder="เช่น คุณสมชาย ใจดี" class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:border-teal focus:ring-2 focus:ring-teal/20">
                                </div>
                                <div>
                                    <label for="lead-phone" class="block font-heading font-medium text-sm text-navy mb-1.5">
                                        เบอร์โทรศัพท์ติดต่อ <span class="text-red-500">*</span>
                                    </label>
                                    <input type="tel" id="lead-phone" required placeholder="เช่น 081-234-5678" class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:border-teal focus:ring-2 focus:ring-teal/20">
                                </div>
                            </div>

                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-5">
                                <div>
                                    <label for="lead-line" class="block font-heading font-medium text-sm text-navy mb-1.5">
                                        LINE ID (ถ้ามี)
                                    </label>
                                    <input type="text" id="lead-line" placeholder="เช่น somchai.line" class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:border-teal focus:ring-2 focus:ring-teal/20">
                                </div>
                                <div>
                                    <label for="lead-province" class="block font-heading font-medium text-sm text-navy mb-1.5">
                                        พื้นที่ / จังหวัด <span class="text-red-500">*</span>
                                    </label>
                                    <select id="lead-province" required class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm bg-white focus:outline-none focus:border-teal focus:ring-2 focus:ring-teal/20">
                                        <option value="กรุงเทพมหานคร">กรุงเทพมหานคร</option>
                                        <option value="นนทบุรี">นนทบุรี</option>
                                        <option value="ปทุมธานี">ปทุมธานี</option>
                                        <option value="สมุทรปราการ">สมุทรปราการ</option>
                                        <option value="สมุทรสาคร">สมุทรสาคร</option>
                                        <option value="นครปฐม">นครปฐม</option>
                                        <option value="ชลบุรี / ระยอง">ชลบุรี / ระยอง</option>
                                        <option value="จังหวัดอื่นๆ">จังหวัดอื่นๆ</option>
                                    </select>
                                </div>
                            </div>

                            <div>
                                <label for="lead-service" class="block font-heading font-medium text-sm text-navy mb-1.5">
                                    ประเภทงานที่สนใจ <span class="text-red-500">*</span>
                                </label>
                                <select id="lead-service" required class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm bg-white focus:outline-none focus:border-teal focus:ring-2 focus:ring-teal/20">
                                    <option value="ทาสีภายใน (Indoor)">ทาสีภายใน (Indoor Painting)</option>
                                    <option value="ทาสีภายนอก (Exterior)">ทาสีภายนอกอาคาร / บ้าน (Exterior Painting)</option>
                                    <option value="ทาสีทั้งหลัง (ภายใน + ภายนอก)">ทาสีทั้งหลัง (ภายใน + ภายนอก)</option>
                                    <option value="ทาสีรั้ว/หลังคา/งานเหล็ก-ไม้">ทาสีรั้ว / หลังคา / งานเหล็กและไม้</option>
                                    <option value="ซ่อมรอยแตกร้าวและกันซึม">ซ่อมรอยแตกร้าวและกันซึมดาดฟ้า</option>
                                </select>
                            </div>

                            <div>
                                <label for="lead-details" class="block font-heading font-medium text-sm text-navy mb-1.5">
                                    รายละเอียดเพิ่มเติม / ผลการคำนวณราคาเบื้องต้น
                                </label>
                                <textarea id="lead-details" rows="3" placeholder="ระบุขนาดพื้นที่โดยประมาณ ประเภทบ้าน หรือช่วงเวลาที่สะดวกให้เข้าสำรวจหน้างาน..." class="w-full px-4 py-3 rounded-xl border border-slate-300 text-sm focus:outline-none focus:border-teal focus:ring-2 focus:ring-teal/20"></textarea>
                            </div>

                            <button type="submit" class="w-full py-4 px-6 rounded-2xl bg-amber hover:bg-amber-hover text-navy font-heading font-bold text-base shadow-lg shadow-amber/25 transition transform hover:-translate-y-0.5 flex items-center justify-center gap-2">
                                <i data-lucide="check-circle" class="w-5 h-5"></i>
                                ส่งข้อมูลขอใบเสนอราคาฟรี
                            </button>

                            <p class="text-xs text-center text-slate-500 flex items-center justify-center gap-1.5">
                                <i data-lucide="lock" class="w-3.5 h-3.5 text-teal"></i>
                                ข้อมูลของท่านจะถูกเก็บเป็นความลับ และใช้เพื่อการติดต่อประเมินราคาเท่านั้น
                            </p>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-navy-dark text-slate-300 pt-14 pb-24 sm:pb-14 border-t border-white/10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 pb-10 border-b border-white/10">
                <!-- Brand -->
                <div class="space-y-4">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 rounded-xl bg-teal flex items-center justify-center text-white">
                            <i data-lucide="paint-roller" class="w-6 h-6"></i>
                        </div>
                        <div>
                            <span class="font-heading font-bold text-xl text-white block leading-none">ProPaint <span class="text-amber">TH</span></span>
                            <span class="text-[10px] font-heading text-slate-400 tracking-wider uppercase">Expert House Painting</span>
                        </div>
                    </div>
                    <p class="text-xs sm:text-sm text-slate-400 leading-relaxed">
                        บริษัท โปรเพ้นท์ ไทยแลนด์ จำกัด ผู้เชี่ยวชาญด้านบริการรับทาสีบ้าน คอนโด อาคาร และระบบกันซึมครบวงจร โดยทีมช่างมืออาชีพประสบการณ์กว่า 10 ปี
                    </p>
                </div>

                <!-- Services Links -->
                <div>
                    <h4 class="font-heading font-semibold text-white text-base mb-4">บริการของเรา</h4>
                    <ul class="space-y-2.5 text-xs sm:text-sm text-slate-400">
                        <li><a href="#services" class="hover:text-amber transition">รับทาสีภายในบ้านและคอนโด</a></li>
                        <li><a href="#services" class="hover:text-amber transition">รับทาสีภายนอกอาคารและบ้านเดี่ยว</a></li>
                        <li><a href="#services" class="hover:text-amber transition">รับทาสีหลังคา รั้ว งานเหล็กและไม้</a></li>
                        <li><a href="#services" class="hover:text-amber transition">ซ่อมรอยแตกร้าวและระบบกันซึม</a></li>
                    </ul>
                </div>

                <!-- Quick Links -->
                <div>
                    <h4 class="font-heading font-semibold text-white text-base mb-4">เมนูลัด</h4>
                    <ul class="space-y-2.5 text-xs sm:text-sm text-slate-400">
                        <li><a href="#calculator" class="hover:text-amber transition">คำนวณราคาทาสีเบื้องต้น</a></li>
                        <li><a href="#portfolio" class="hover:text-amber transition">ผลงาน Before & After</a></li>
                        <li><a href="#process" class="hover:text-amber transition">ขั้นตอนการทำงาน 4 ขั้นตอน</a></li>
                        <li><a href="#faq" class="hover:text-amber transition">คำถามที่พบบ่อย (FAQ)</a></li>
                    </ul>
                </div>

                <!-- Office Contact -->
                <div>
                    <h4 class="font-heading font-semibold text-white text-base mb-4">ติดต่อสำนักงาน</h4>
                    <ul class="space-y-2.5 text-xs sm:text-sm text-slate-400">
                        <li class="flex items-start gap-2">
                            <i data-lucide="map-pin" class="w-4 h-4 text-amber shrink-0 mt-0.5"></i>
                            <span>88/19 ถนนพระราม 2 แขวงแสมดำ เขตบางขุนเทียน กรุงเทพฯ 10150</span>
                        </li>
                        <li class="flex items-center gap-2">
                            <i data-lucide="phone" class="w-4 h-4 text-amber shrink-0"></i>
                            <span>02-888-9944, 089-456-7890</span>
                        </li>
                        <li class="flex items-center gap-2">
                            <i data-lucide="clock" class="w-4 h-4 text-amber shrink-0"></i>
                            <span>เปิดทำการทุกวัน 08:00 - 20:00 น.</span>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="pt-6 flex flex-col sm:flex-row items-center justify-between text-xs text-slate-500 gap-3">
                <p>© 2026 ProPaint Thailand Co., Ltd. สงวนลิขสิทธิ์ทั้งหมด</p>
                <p>มาตรฐานสีแท้ 100% ร่วมกับ TOA • Dulux • Beger • Jotun</p>
            </div>
        </div>
    </footer>

    <!-- Floating Action Buttons (Bottom Right: LINE & Quick Call) -->
    <div class="fixed bottom-5 right-5 z-50 flex flex-col items-end gap-3">
        <!-- Quick Call Button -->
        <a href="tel:028889944" aria-label="โทรด่วนหาช่าง" class="group flex items-center gap-2 bg-navy hover:bg-navy-light text-white px-4 py-3 rounded-full shadow-xl border border-white/15 transition transform hover:scale-105">
            <i data-lucide="phone-call" class="w-5 h-5 text-amber"></i>
            <span class="font-heading font-semibold text-xs sm:text-sm">โทรด่วน</span>
        </a>

        <!-- LINE Chat Button -->
        <button type="button" onclick="openLineModal(event)" aria-label="แชท LINE ประเมินราคา" class="relative animate-pulse-ring flex items-center gap-2 bg-[#06C755] hover:bg-[#05B34C] text-white px-4 py-3.5 rounded-full shadow-xl transition transform hover:scale-105">
            <span class="font-heading font-extrabold text-xs bg-white text-[#06C755] px-1.5 py-0.5 rounded">LINE</span>
            <span class="font-heading font-semibold text-xs sm:text-sm">แชทประเมินฟรี</span>
        </button>
    </div>

    <!-- Custom Notification / Confirmation Modal (No alert()) -->
    <div id="custom-modal" class="hidden fixed inset-0 z-50 bg-navy/60 backdrop-blur-sm flex items-center justify-center p-4">
        <div class="bg-white rounded-3xl max-w-md w-full p-6 sm:p-8 shadow-2xl text-center space-y-4 transform transition-all">
            <div id="modal-icon-box" class="w-16 h-16 rounded-2xl bg-teal-soft text-teal mx-auto flex items-center justify-center">
                <i data-lucide="check-circle-2" class="w-9 h-9"></i>
            </div>
            <h3 id="modal-title" class="font-heading font-bold text-xl text-navy">ส่งข้อมูลเรียบร้อยแล้ว!</h3>
            <p id="modal-message" class="text-sm text-slate-600 leading-relaxed">
                ขอบคุณที่ไว้วางใจ ProPaint Thailand ทีมวิศวกรประเมินราคาจะติดต่อกลับภายใน 30 นาทีครับ
            </p>
            <div id="modal-extra" class="hidden p-3.5 rounded-2xl bg-offwhite border border-slate-200 text-xs font-heading text-navy">
                LINE Official: <strong>@propaint.th</strong>
            </div>
            <button type="button" onclick="closeModal()" class="w-full py-3.5 rounded-xl bg-navy hover:bg-navy-light text-white font-heading font-semibold text-sm transition">
                ตกลง / ปิดหน้าต่าง
            </button>
        </div>
    </div>

    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        function closeMobileMenu() {
            mobileMenu.classList.add('hidden');
        }

        // ==========================================
        // 1. INTERACTIVE COST ESTIMATOR CALCULATOR
        // ==========================================
        const calcState = {
            scope: 'indoor',      // indoor, outdoor, both
            property: 'townhome', // condo, townhome, detached
            area: 120,
            grade: 'premium'      // standard, premium, flagship
        };

        const scopeLabels = {
            indoor: 'ทาสีภายใน',
            outdoor: 'ทาสีภายนอก',
            both: 'ทาสีทั้งหลัง (ภายใน + ภายนอก)'
        };

        const propertyLabels = {
            condo: 'คอนโดมิเนียม',
            townhome: 'ทาวน์โฮม',
            detached: 'บ้านเดี่ยว'
        };

        const gradeConfig = {
            standard: {
                label: 'เกรดมาตรฐาน (Standard Shield)',
                ratePerSqm: 115,
                warranty: '2 ปี'
            },
            premium: {
                label: 'เกรดพรีเมียมเช็ดล้างได้',
                ratePerSqm: 155,
                warranty: '3 ปี'
            },
            flagship: {
                label: 'เกรดสูงสุดกันความร้อน 15 ปี',
                ratePerSqm: 195,
                warranty: '5 ปี'
            }
        };

        function setCalcOption(type, value, btnElement) {
            calcState[type] = value;

            // Update UI button styles
            if (type === 'scope') {
                document.querySelectorAll('.calc-scope-btn').forEach(btn => {
                    btn.className = 'calc-scope-btn p-3.5 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-slate-600 font-heading font-medium text-xs sm:text-sm text-center transition';
                });
                btnElement.className = 'calc-scope-btn p-3.5 rounded-2xl border-2 border-teal bg-teal-soft text-navy font-heading font-semibold text-xs sm:text-sm text-center transition';
            } else if (type === 'property') {
                document.querySelectorAll('.calc-prop-btn').forEach(btn => {
                    btn.className = 'calc-prop-btn p-3 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-slate-600 font-heading font-medium text-xs sm:text-sm text-center transition';
                });
                btnElement.className = 'calc-prop-btn p-3 rounded-2xl border-2 border-teal bg-teal-soft text-navy font-heading font-semibold text-xs sm:text-sm text-center transition';
                
                // Suggest realistic default area when switching property type
                const defaultAreas = { condo: 45, townhome: 120, detached: 220 };
                calcState.area = defaultAreas[value];
                document.getElementById('area-input').value = calcState.area;
                document.getElementById('area-slider').value = calcState.area;
            } else if (type === 'grade') {
                document.querySelectorAll('.calc-grade-btn').forEach(btn => {
                    btn.className = 'calc-grade-btn w-full p-3.5 rounded-2xl border-2 border-slate-200 hover:border-teal/50 text-left flex items-center justify-between transition';
                });
                btnElement.className = 'calc-grade-btn w-full p-3.5 rounded-2xl border-2 border-teal bg-teal-soft text-left flex items-center justify-between transition';
            }

            updateCalculatorResult();
        }

        function syncAreaFromSlider(val) {
            calcState.area = parseInt(val) || 20;
            document.getElementById('area-input').value = calcState.area;
            updateCalculatorResult();
        }

        function syncAreaFromInput(val) {
            let num = parseInt(val);
            if (isNaN(num) || num < 10) num = 10;
            if (num > 2000) num = 2000;
            calcState.area = num;
            document.getElementById('area-slider').value = Math.min(num, 600);
            updateCalculatorResult();
        }

        function updateCalculatorResult() {
            const scopeMultiplier = calcState.scope === 'both' ? 1.75 : (calcState.scope === 'outdoor' ? 1.15 : 1.0);
            const propMultiplier = calcState.property === 'detached' ? 1.08 : (calcState.property === 'condo' ? 0.95 : 1.0);
            const baseRate = gradeConfig[calcState.grade].ratePerSqm;

            const rawEstimate = calcState.area * baseRate * scopeMultiplier * propMultiplier;
            const minPrice = Math.round((rawEstimate * 0.92) / 500) * 500;
            const maxPrice = Math.round((rawEstimate * 1.08) / 500) * 500;

            // Calculate estimated working days
            let days = '2-3 วัน';
            const effectiveArea = calcState.area * scopeMultiplier;
            if (effectiveArea > 350) days = '7-10 วัน';
            else if (effectiveArea > 200) days = '5-7 วัน';
            else if (effectiveArea > 90) days = '3-5 วัน';

            document.getElementById('calc-price-display').textContent = `${minPrice.toLocaleString()} - ${maxPrice.toLocaleString()} บาท`;
            document.getElementById('calc-days-display').textContent = days;
            document.getElementById('calc-warranty-display').textContent = gradeConfig[calcState.grade].warranty;

            document.getElementById('summary-scope').textContent = scopeLabels[calcState.scope];
            document.getElementById('summary-property').textContent = `${propertyLabels[calcState.property]} (${calcState.area} ตร.ม.)`;
            document.getElementById('summary-grade').textContent = gradeConfig[calcState.grade].label;
        }

        function transferEstimateToForm() {
            const priceText = document.getElementById('calc-price-display').textContent;
            const serviceSelect = document.getElementById('lead-service');
            if (calcState.scope === 'indoor') serviceSelect.value = 'ทาสีภายใน (Indoor)';
            else if (calcState.scope === 'outdoor') serviceSelect.value = 'ทาสีภายนอก (Exterior)';
            else serviceSelect.value = 'ทาสีทั้งหลัง (ภายใน + ภายนอก)';

            document.getElementById('lead-details').value = `[ข้อมูลจากเครื่องคำนวณราคา] ประเภท: ${propertyLabels[calcState.property]} พื้นที่ประมาณ ${calcState.area} ตร.ม. | งาน: ${scopeLabels[calcState.scope]} | เกรดสี: ${gradeConfig[calcState.grade].label} | ราคาประเมินเบื้องต้น: ${priceText}`;
            
            document.getElementById('quote-form').scrollIntoView({ behavior: 'smooth' });
            setTimeout(() => {
                document.getElementById('lead-name').focus();
            }, 600);
        }

        function selectServiceAndScroll(serviceName) {
            document.getElementById('lead-service').value = serviceName;
            document.getElementById('quote-form').scrollIntoView({ behavior: 'smooth' });
            setTimeout(() => {
                document.getElementById('lead-name').focus();
            }, 600);
        }

        // ==========================================
        // 2. BEFORE / AFTER INTERACTIVE SLIDER
        // ==========================================
        const baBox = document.getElementById('ba-slider-box');
        const baAfter = document.getElementById('ba-after-layer');
        const baDivider = document.getElementById('ba-divider');
        let isDraggingBA = false;

        function updateBASlider(clientX) {
            const rect = baBox.getBoundingClientRect();
            baBox.style.setProperty('--ba-full-width', `${rect.width}px`);
            let offsetX = clientX - rect.left;
            offsetX = Math.max(0, Math.min(offsetX, rect.width));
            const percent = (offsetX / rect.width) * 100;
            baAfter.style.width = `${percent}%`;
            baDivider.style.left = `${percent}%`;
        }

        window.addEventListener('resize', () => {
            if (baBox) {
                baBox.style.setProperty('--ba-full-width', `${baBox.getBoundingClientRect().width}px`);
            }
        });
        // Set initial SVG width properly
        setTimeout(() => {
            if (baBox) baBox.style.setProperty('--ba-full-width', `${baBox.getBoundingClientRect().width}px`);
        }, 100);

        baBox.addEventListener('mousedown', (e) => { isDraggingBA = true; updateBASlider(e.clientX); });
        window.addEventListener('mouseup', () => { isDraggingBA = false; });
        window.addEventListener('mousemove', (e) => { if (isDraggingBA) updateBASlider(e.clientX); });

        baBox.addEventListener('touchstart', (e) => { isDraggingBA = true; updateBASlider(e.touches[0].clientX); }, { passive: true });
        window.addEventListener('touchend', () => { isDraggingBA = false; });
        window.addEventListener('touchmove', (e) => { if (isDraggingBA) updateBASlider(e.touches[0].clientX); }, { passive: true });

        // ==========================================
        // 3. PORTFOLIO FILTERING & RENDERING
        // ==========================================
        const portfolioData = [
            {
                category: 'detached',
                categoryLabel: 'บ้านเดี่ยว',
                title: 'ทาสีทั้งหลัง หมู่บ้านเศรษฐสิริ พัฒนาการ',
                paint: 'Dulux Weathershield Powerflexx',
                area: '310 ตร.ม. • 6 วัน',
                bgGradient: 'from-navy-soft to-teal-soft',
                accentColor: '#0F2942'
            },
            {
                category: 'townhome',
                categoryLabel: 'ทาวน์โฮม',
                title: 'รีโนเวททาสีภายนอก-ภายใน บ้านกลางเมือง',
                paint: 'TOA SuperShield & Ultra Clean',
                area: '145 ตร.ม. • 4 วัน',
                bgGradient: 'from-amber-soft to-offwhite',
                accentColor: '#0D9488'
            },
            {
                category: 'condo',
                categoryLabel: 'คอนโด/อาคาร',
                title: 'ทาสีภายในห้องชุด Rhythm สุขุมวิท 50',
                paint: 'Beger Shield AirFresh Anti-Virus',
                area: '68 ตร.ม. • 2 วัน',
                bgGradient: 'from-teal-soft to-navy-soft',
                accentColor: '#F59E0B'
            },
            {
                category: 'detached',
                categoryLabel: 'บ้านเดี่ยว',
                title: 'ซ่อมกันซึมดาดฟ้า & ทาสีภายนอก นนทบุรี',
                paint: 'TOA 201 Roofseal + SuperShield',
                area: '260 ตร.ม. • 5 วัน',
                bgGradient: 'from-slate-100 to-teal-soft',
                accentColor: '#0F2942'
            },
            {
                category: 'townhome',
                categoryLabel: 'ทาวน์โฮม',
                title: 'ทาสีโฮมออฟฟิศ 3 ชั้น ย่านลาดพร้าว',
                paint: 'Jotun Majestic True Beauty',
                area: '190 ตร.ม. • 4 วัน',
                bgGradient: 'from-navy-soft to-amber-soft',
                accentColor: '#0D9488'
            },
            {
                category: 'condo',
                categoryLabel: 'คอนโด/อาคาร',
                title: 'ทาสีอาคารพาณิชย์ 4 คูหา พระราม 2',
                paint: 'TOA 4Seasons ภายนอก',
                area: '480 ตร.ม. • 8 วัน',
                bgGradient: 'from-teal-soft to-slate-100',
                accentColor: '#0F2942'
            }
        ];

        function renderPortfolio(filter = 'all') {
            const grid = document.getElementById('portfolio-grid');
            const filtered = filter === 'all' ? portfolioData : portfolioData.filter(item => item.category === filter);

            grid.innerHTML = filtered.map(item => `
                <div class="rounded-3xl bg-offwhite border border-slate-200/80 overflow-hidden shadow-sm hover:shadow-md transition group">
                    <div class="h-44 bg-gradient-to-br ${item.bgGradient} p-5 relative flex items-center justify-center">
                        <span class="absolute top-3.5 left-3.5 bg-white/95 text-navy font-heading text-xs font-semibold px-3 py-1 rounded-full shadow-sm">
                            ${item.categoryLabel}
                        </span>
                        <span class="absolute bottom-3 right-3 bg-navy/85 text-white font-heading text-[11px] px-2.5 py-1 rounded-lg">
                            ${item.area}
                        </span>
                        <!-- Architectural Illustration Icon -->
                        <div class="w-20 h-20 rounded-2xl bg-white shadow-md flex items-center justify-center group-hover:scale-110 transition" style="color: ${item.accentColor}">
                            <i data-lucide="building-2" class="w-10 h-10"></i>
                        </div>
                    </div>
                    <div class="p-5">
                        <h4 class="font-heading font-bold text-base text-navy group-hover:text-teal transition">${item.title}</h4>
                        <p class="text-xs text-slate-500 mt-1.5 flex items-center gap-1.5">
                            <i data-lucide="paint-bucket" class="w-3.5 h-3.5 text-amber-hover"></i>
                            ใช้สี: <strong class="text-slate-700">${item.paint}</strong>
                        </p>
                    </div>
                </div>
            `).join('');
            lucide.createIcons();
        }

        function filterPortfolio(category, btn) {
            document.querySelectorAll('.port-filter-btn').forEach(b => {
                b.className = 'port-filter-btn px-4 py-2 rounded-xl font-heading text-xs sm:text-sm font-medium text-slate-600 hover:text-navy transition';
            });
            btn.className = 'port-filter-btn px-4 py-2 rounded-xl font-heading text-xs sm:text-sm font-semibold bg-navy text-white transition';
            renderPortfolio(category);
        }

        // ==========================================
        // 4. FAQ ACCORDION
        // ==========================================
        function toggleFaq(index) {
            const content = document.getElementById(`faq-content-${index}`);
            const icon = document.getElementById(`faq-icon-${index}`);
            const isHidden = content.classList.contains('hidden');

            // Close all first
            for (let i = 0; i < 4; i++) {
                document.getElementById(`faq-content-${i}`).classList.add('hidden');
                document.getElementById(`faq-icon-${i}`).style.transform = 'rotate(0deg)';
            }

            if (isHidden) {
                content.classList.remove('hidden');
                icon.style.transform = 'rotate(180deg)';
            }
        }

        // ==========================================
        // 5. FORM SUBMISSION & CUSTOM MODALS
        // ==========================================
        function handleQuoteSubmit(e) {
            e.preventDefault();
            const name = document.getElementById('lead-name').value;
            const phone = document.getElementById('lead-phone').value;
            const service = document.getElementById('lead-service').value;

            document.getElementById('modal-icon-box').className = 'w-16 h-16 rounded-2xl bg-teal-soft text-teal mx-auto flex items-center justify-center';
            document.getElementById('modal-icon-box').innerHTML = '<i data-lucide="check-circle-2" class="w-9 h-9"></i>';
            document.getElementById('modal-title').textContent = 'ส่งคำขอใบเสนอราคาสำเร็จ!';
            document.getElementById('modal-message').innerHTML = `ขอบคุณ <strong>${name}</strong> สำหรับข้อมูลบริการ <strong>${service}</strong><br>ทีมวิศวกรประเมินราคาจะติดต่อกลับที่เบอร์ <strong>${phone}</strong> ภายใน 30 นาทีครับ`;
            document.getElementById('modal-extra').classList.remove('hidden');
            
            document.getElementById('custom-modal').classList.remove('hidden');
            lucide.createIcons();
            e.target.reset();
        }

        function openLineModal(e) {
            e.preventDefault();
            document.getElementById('modal-icon-box').className = 'w-16 h-16 rounded-2xl bg-[#06C755]/15 text-[#06C755] mx-auto flex items-center justify-center font-heading font-extrabold text-xl';
            document.getElementById('modal-icon-box').textContent = 'LINE';
            document.getElementById('modal-title').textContent = 'แอดไลน์ประเมินราคาด่วน';
            document.getElementById('modal-message').textContent = 'สามารถค้นหา LINE ID: @propaint.th เพื่อส่งรูปถ่ายบ้านหรือแปลนพื้นที่ ให้ทีมช่างประเมินราคาเบื้องต้นฟรีได้ทันทีครับ';
            document.getElementById('modal-extra').classList.remove('hidden');
            document.getElementById('custom-modal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('custom-modal').classList.add('hidden');
        }

        // Initialize Page
        updateCalculatorResult();
        renderPortfolio('all');
    </script>
</body>
</html>
