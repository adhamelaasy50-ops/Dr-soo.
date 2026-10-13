# Dr-soo.
​أهلاً بيك في أكاديمية دكتور سعاد – طريقك للتميز في المواد الطبية!​عملنالك المنصة دي مخصوص عشان نسهل عليك مشوار الدراسة والامتحانات. هدفنا نقدم محتوى طبي معتمد ومتنظم بأحدث الطرق التكنولوجية عشان توفر وقتك ومجهودك.
<!doctype html>
<html lang="ar" dir="rtl">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>دكتور سعاد - Dr. Soad Medical Academy</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Google Fonts: Cairo & Tajawal -->
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800;900&amp;family=Tajawal:wght@400;500;700;800&amp;display=swap" rel="stylesheet">
  <!-- FontAwesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        darkbg: '#070a13',
                        cardbg: 'rgba(15, 23, 42, 0.75)',
                        cyanaccent: '#06b6d4',
                        tealaccent: '#14b8a6',
                        emeraldaccent: '#10b981',
                        voda: '#e11d48'
                    },
                    fontFamily: {
                        cairo: ['Cairo', 'sans-serif'],
                        tajawal: ['Tajawal', 'sans-serif']
                    }
                }
            }
        }
    </script>
  <style>
        body {
            font-family: 'Cairo', 'Tajawal', sans-serif;
            background: radial-gradient(circle at top center, #0f172a 0%, #090d16 50%, #03060d 100%);
            color: #f8fafc;
            min-height: 100vh;
        }
        .glass-card {
            background: rgba(15, 23, 42, 0.7);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            box-shadow: 0 10px 30px -5px rgba(0, 0, 0, 0.5);
        }
        .glass-nav {
            background: rgba(9, 13, 22, 0.85);
            backdrop-filter: blur(16px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.08);
        }
        .glow-cyan {
            box-shadow: 0 0 30px -5px rgba(6, 182, 212, 0.25);
        }
        .glow-voda {
            box-shadow: 0 0 30px -5px rgba(225, 29, 72, 0.35);
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 6px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: rgba(9, 13, 22, 0.6);
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: #06b6d4;
            border-radius: 4px;
        }
    </style>
 </head>
 <body class="custom-scrollbar flex flex-col justify-between selection:bg-cyanaccent selection:text-slate-950">
  <!-- Sticky Navigation Header -->
  <header class="sticky top-0 z-50 glass-nav transition-all duration-300">
   <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
    <!-- Brand Logo & Title -->
    <div class="flex items-center space-x-3 space-x-reverse cursor-pointer" onclick="switchTab('home')">
     <div class="relative flex items-center justify-center w-12 h-12 rounded-2xl bg-gradient-to-tr from-cyan-500 via-teal-400 to-emerald-400 p-0.5 shadow-lg shadow-cyan-500/20">
      <div class="w-full h-full bg-slate-950 rounded-[14px] flex items-center justify-center">
       <i class="fa-solid fa-user-doctor text-2xl text-cyan-400"></i>
      </div>
     </div>
     <div>
      <h1 class="text-xl sm:text-2xl font-black bg-gradient-to-l from-cyan-400 via-teal-300 to-white bg-clip-text text-transparent">دكتور سعاد</h1>
      <p class="text-xs text-slate-400 font-medium">Dr. Soad Medical Academy</p>
     </div>
    </div>
    <!-- Desktop Navigation Tabs -->
    <nav class="hidden md:flex items-center space-x-1 space-x-reverse bg-slate-900/80 p-1.5 rounded-2xl border border-slate-800">
     <button onclick="switchTab('home')" id="nav-home" class="nav-btn active px-4 py-2 rounded-xl text-sm font-bold transition-all text-cyan-400 bg-slate-800 border border-slate-700/50"><i class="fa-solid fa-house ml-1.5"></i>الرئيسية</button>
     <button onclick="switchTab('years')" id="nav-years" class="nav-btn px-4 py-2 rounded-xl text-sm font-bold transition-all text-slate-300 hover:text-white hover:bg-slate-800/50"><i class="fa-solid fa-graduation-cap ml-1.5"></i>المناهج والسنوات</button>
     <button onclick="switchTab('activation')" id="nav-activation" class="nav-btn px-4 py-2 rounded-xl text-sm font-bold transition-all text-rose-400 hover:text-rose-300 hover:bg-rose-950/30"><i class="fa-solid fa-mobile-screen-button ml-1.5"></i>تفعيل الحساب (فودافون كاش)</button>
     <button onclick="switchTab('quiz')" id="nav-quiz" class="nav-btn px-4 py-2 rounded-xl text-sm font-bold transition-all text-emerald-400 hover:text-emerald-300 hover:bg-emerald-950/30"><i class="fa-solid fa-brain ml-1.5"></i>اختبارات تفاعلية</button>
    </nav>
    <!-- Quick Action Button -->
    <div class="hidden sm:flex items-center gap-3">
     <button onclick="switchTab('activation')" class="bg-gradient-to-r from-rose-600 to-rose-500 hover:from-rose-500 hover:to-rose-400 text-white px-4 py-2.5 rounded-xl font-bold text-sm shadow-lg shadow-rose-600/30 transition-all flex items-center gap-2"><i class="fa-solid fa-bolt"></i> <span>اشترك واشحن كاش</span></button>
    </div>
    <!-- Mobile Menu Toggle Button -->
    <button onclick="toggleMobileMenu()" class="md:hidden p-2.5 rounded-xl bg-slate-800 text-slate-300 hover:text-white border border-slate-700"><i class="fa-solid fa-bars text-xl" id="menu-icon"></i></button>
   </div>
   <!-- Mobile Dropdown Navigation -->
   <div id="mobile-menu" class="hidden md:hidden bg-slate-950/95 border-b border-slate-800 px-4 pt-3 pb-6 space-y-2">
    <button onclick="switchTab('home')" class="w-full text-right px-4 py-3 rounded-xl font-bold text-slate-200 hover:bg-slate-800 flex items-center"><i class="fa-solid fa-house ml-3 text-cyan-400"></i>الرئيسية</button>
    <button onclick="switchTab('years')" class="w-full text-right px-4 py-3 rounded-xl font-bold text-slate-200 hover:bg-slate-800 flex items-center"><i class="fa-solid fa-graduation-cap ml-3 text-teal-400"></i>المناهج والسنوات (1 - 5)</button>
    <button onclick="switchTab('activation')" class="w-full text-right px-4 py-3 rounded-xl font-bold text-rose-400 hover:bg-rose-950/40 flex items-center"><i class="fa-solid fa-mobile-screen-button ml-3 text-rose-400"></i>تفعيل الحساب عبر فودافون كاش</button>
    <button onclick="switchTab('quiz')" class="w-full text-right px-4 py-3 rounded-xl font-bold text-emerald-400 hover:bg-emerald-950/40 flex items-center"><i class="fa-solid fa-brain ml-3 text-emerald-400"></i>اختبارات وتحديات</button>
   </div>
  </header>
  <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 flex-1 w-full">
   <!-- ================= SECTION 1: HOME TAB ================= -->
   <section id="tab-home" class="space-y-10">
    <!-- Hero Banner -->
    <div class="relative rounded-3xl overflow-hidden glass-card p-8 md:p-12 border border-slate-800 glow-cyan">
     <div class="absolute -right-20 -top-20 w-80 h-80 bg-cyan-500/10 rounded-full blur-3xl pointer-events-none"></div>
     <div class="absolute -left-20 -bottom-20 w-80 h-80 bg-teal-500/10 rounded-full blur-3xl pointer-events-none"></div>
     <div class="relative z-10 grid md:grid-cols-12 gap-8 items-center">
      <div class="md:col-span-7 space-y-6">
       <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-cyan-950/80 border border-cyan-800/50 text-cyan-400 text-xs font-bold">
        <span class="w-2 h-2 rounded-full bg-cyan-400 animate-ping"></span> المنصة التعليمية المتكاملة لكليات الطب
       </div>
       <h2 class="text-3xl md:text-5xl font-black leading-tight">رحلتك الأكاديمية الشاملة في <span class="bg-gradient-to-r from-cyan-400 via-teal-300 to-emerald-400 bg-clip-text text-transparent">الطب البشري</span> مع دكتور سعاد</h2>
       <p class="text-slate-300 text-base md:text-lg leading-relaxed font-normal">شرح تفاعلي متطور لمناهج السنوات الأولى وحتى الخامسة. محاضرا فيديو عالية الجودة، مذكرات ملونة PDF، وبنك أسئلة واختبارات إكلينيكية مجابة بالكامل.</p>
       <div class="flex flex-wrap gap-4 pt-2">
        <button onclick="switchTab('years')" class="bg-gradient-to-r from-cyan-500 to-teal-500 hover:from-cyan-400 hover:to-teal-400 text-slate-950 font-black px-6 py-3.5 rounded-2xl shadow-lg shadow-cyan-500/20 transition-all flex items-center gap-2"><i class="fa-solid fa-book-open"></i> <span>استعراض المقررات والسنوات</span></button>
        <button onclick="switchTab('activation')" class="bg-slate-800/90 hover:bg-slate-800 text-white font-bold px-6 py-3.5 rounded-2xl border border-slate-700 transition-all flex items-center gap-2"><i class="fa-solid fa-key text-rose-400"></i> <span>خطوات التفعيل بفودافون كاش</span></button>
       </div>
      </div>
      <!-- Visual Quick Stat Cards -->
      <div class="md:col-span-5 grid grid-cols-2 gap-4">
       <div class="glass-card p-5 rounded-2xl border border-slate-800 flex flex-col items-center text-center hover:border-cyan-500/40 transition-all">
        <div class="w-12 h-12 rounded-xl bg-cyan-500/10 text-cyan-400 flex items-center justify-center text-xl mb-3">
         <i class="fa-solid fa-stethoscope"></i>
        </div>
        <span class="text-2xl font-black text-white">5 سنوات</span> <span class="text-xs text-slate-400 mt-1">تغطية كافة المراحل والسنوات</span>
       </div>
       <div class="glass-card p-5 rounded-2xl border border-slate-800 flex flex-col items-center text-center hover:border-teal-500/40 transition-all">
        <div class="w-12 h-12 rounded-xl bg-teal-500/10 text-teal-400 flex items-center justify-center text-xl mb-3">
         <i class="fa-solid fa-circle-play"></i>
        </div>
        <span class="text-2xl font-black text-white">+600 فيديو</span> <span class="text-xs text-slate-400 mt-1">شرح مبسط وعالي الجودة</span>
       </div>
       <div class="glass-card p-5 rounded-2xl border border-slate-800 flex flex-col items-center text-center hover:border-emerald-500/40 transition-all">
        <div class="w-12 h-12 rounded-xl bg-emerald-500/10 text-emerald-400 flex items-center justify-center text-xl mb-3">
         <i class="fa-solid fa-file-pdf"></i>
        </div>
        <span class="text-2xl font-black text-white">ملخصات PDF</span> <span class="text-xs text-slate-400 mt-1">مذكرات أطلس ورسومات ملونة</span>
       </div>
       <div class="glass-card p-5 rounded-2xl border border-slate-800 flex flex-col items-center text-center hover:border-amber-500/40 transition-all">
        <div class="w-12 h-12 rounded-xl bg-amber-500/10 text-amber-400 flex items-center justify-center text-xl mb-3">
         <i class="fa-solid fa-vial-circle-check"></i>
        </div>
        <span class="text-2xl font-black text-white">MCQs تفاعلية</span> <span class="text-xs text-slate-400 mt-1">اختبارات مع تفسير علمي</span>
       </div>
      </div>
     </div>
    </div>
    <!-- Prominent Vodafone Cash Banner -->
    <div class="glass-card p-6 rounded-2xl border-2 border-rose-500/40 bg-gradient-to-r from-rose-950/40 via-slate-950 to-slate-900 relative overflow-hidden glow-voda">
     <div class="flex flex-col md:flex-row items-center justify-between gap-6">
      <div class="flex items-center space-x-4 space-x-reverse">
       <div class="w-14 h-14 rounded-2xl bg-rose-600 flex items-center justify-center text-white text-2xl shrink-0 shadow-lg shadow-rose-600/50">
        <i class="fa-solid fa-wallet"></i>
       </div>
       <div>
        <span class="text-xs font-bold text-rose-400 uppercase tracking-wider">تفعيل مباشر وسريع</span>
        <h3 class="text-lg md:text-xl font-extrabold text-white">رقم تحويل فودافون كاش لتفعيل المنصة</h3>
        <p class="text-sm text-slate-300">حول الاشتراك فوراً إلى الرقم للبدء مباشرة في مشاهدة الكورسات</p>
       </div>
      </div>
      <div class="flex items-center gap-3 bg-slate-950 px-5 py-3 rounded-xl border border-rose-500/30 w-full md:w-auto justify-between">
       <span class="font-mono text-2xl font-black text-rose-400 tracking-widest" id="home-voda-num">01063415687</span>
       <button onclick="copyVodafoneNumber()" class="bg-rose-600 hover:bg-rose-500 text-white text-xs font-bold px-4 py-2.5 rounded-lg transition-all flex items-center gap-1.5 shadow-md"><i class="fa-regular fa-copy"></i> <span id="copy-text-home">نسخ الرقم</span></button>
      </div>
     </div>
    </div>
    <!-- Years Overview Cards Grid -->
    <div>
     <div class="text-center max-w-2xl mx-auto mb-8">
      <h3 class="text-2xl font-black text-white">اختر سنتك الدراسية للبدء</h3>
      <p class="text-slate-400 text-sm mt-1">تغطية دقيقة لجميع المواد والأقسام حسب كل سنة دراسية</p>
     </div>
     <div class="grid sm:grid-cols-2 lg:grid-cols-5 gap-4">
      <!-- Year 1 -->
      <div onclick="selectYearAndOpen(1)" class="glass-card rounded-2xl p-5 border border-slate-800 hover:border-cyan-400/60 cursor-pointer transition-all duration-300 transform hover:-translate-y-1 group">
       <div class="w-10 h-10 rounded-xl bg-cyan-500/10 text-cyan-400 flex items-center justify-center font-bold text-lg mb-4 group-hover:scale-110 transition-transform">١</div>
       <h4 class="font-bold text-lg text-white mb-1 group-hover:text-cyan-400 transition-colors">السنة الأولى</h4>
       <p class="text-xs text-slate-400 mb-3">التشريح، وظائف الأعضاء، الهستولوجي والبيوكيمياء</p>
       <span class="text-xs text-cyan-400 font-semibold inline-flex items-center gap-1"> تصفح المواد <i class="fa-solid fa-arrow-left text-[10px]"></i> </span>
      </div>
      <!-- Year 2 -->
      <div onclick="selectYearAndOpen(2)" class="glass-card rounded-2xl p-5 border border-slate-800 hover:border-teal-400/60 cursor-pointer transition-all duration-300 transform hover:-translate-y-1 group">
       <div class="w-10 h-10 rounded-xl bg-teal-500/10 text-teal-400 flex items-center justify-center font-bold text-lg mb-4 group-hover:scale-110 transition-transform">٢</div>
       <h4 class="font-bold text-lg text-white mb-1 group-hover:text-teal-400 transition-colors">السنة الثانية</h4>
       <p class="text-xs text-slate-400 mb-3">علم الأمراض، الفارماكولوجي، والأحياء الدقيقة</p>
       <span class="text-xs text-teal-400 font-semibold inline-flex items-center gap-1"> تصفح المواد <i class="fa-solid fa-arrow-left text-[10px]"></i> </span>
      </div>
      <!-- Year 3 -->
      <div onclick="selectYearAndOpen(3)" class="glass-card rounded-2xl p-5 border border-slate-800 hover:border-emerald-400/60 cursor-pointer transition-all duration-300 transform hover:-translate-y-1 group">
       <div class="w-10 h-10 rounded-xl bg-emerald-500/10 text-emerald-400 flex items-center justify-center font-bold text-lg mb-4 group-hover:scale-110 transition-transform">٣</div>
       <h4 class="font-bold text-lg text-white mb-1 group-hover:text-emerald-400 transition-colors">السنة الثالثة</h4>
       <p class="text-xs text-slate-400 mb-3">الباطنة العامة، والطب الشرعي وعلم السموم</p>
       <span class="text-xs text-emerald-400 font-semibold inline-flex items-center gap-1"> تصفح المواد <i class="fa-solid fa-arrow-left text-[10px]"></i> </span>
      </div>
      <!-- Year 4 -->
      <div onclick="selectYearAndOpen(4)" class="glass-card rounded-2xl p-5 border border-slate-800 hover:border-purple-400/60 cursor-pointer transition-all duration-300 transform hover:-translate-y-1 group">
       <div class="w-10 h-10 rounded-xl bg-purple-500/10 text-purple-400 flex items-center justify-center font-bold text-lg mb-4 group-hover:scale-110 transition-transform">٤</div>
       <h4 class="font-bold text-lg text-white mb-1 group-hover:text-purple-400 transition-colors">السنة الرابعة</h4>
       <p class="text-xs text-slate-400 mb-3">الجراحة العامة وطب وجراحة الأطفال</p>
       <span class="text-xs text-purple-400 font-semibold inline-flex items-center gap-1"> تصفح المواد <i class="fa-solid fa-arrow-left text-[10px]"></i> </span>
      </div>
      <!-- Year 5 -->
      <div onclick="selectYearAndOpen(5)" class="glass-card rounded-2xl p-5 border border-slate-800 hover:border-amber-400/60 cursor-pointer transition-all duration-300 transform hover:-translate-y-1 group">
       <div class="w-10 h-10 rounded-xl bg-amber-500/10 text-amber-400 flex items-center justify-center font-bold text-lg mb-4 group-hover:scale-110 transition-transform">٥</div>
       <h4 class="font-bold text-lg text-white mb-1 group-hover:text-amber-400 transition-colors">السنة الخامسة</h4>
       <p class="text-xs text-slate-400 mb-3">النساء والتوليد، طب العيون، والأنف والأذن</p>
       <span class="text-xs text-amber-400 font-semibold inline-flex items-center gap-1"> تصفح المواد <i class="fa-solid fa-arrow-left text-[10px]"></i> </span>
      </div>
     </div>
    </div>
   </section>
   <!-- ================= SECTION 2: ACADEMIC YEARS & COURSES TAB ================= -->
   <section id="tab-years" class="hidden space-y-8">
    <div class="flex flex-col md:flex-row md:items-center justify-between gap-4 pb-4 border-b border-slate-800">
     <div>
      <h2 class="text-2xl font-black text-white flex items-center gap-2"><i class="fa-solid fa-book-medical text-cyan-400"></i> المناهج والمقررات الطبية</h2>
      <p class="text-sm text-slate-400 mt-1">اختر السنة الدراسية لعرض المواد والمحاضرات المقررة</p>
     </div>
     <!-- Year Filter Tabs -->
     <div class="flex overflow-x-auto gap-2 py-1 custom-scrollbar">
      <button onclick="setAcademicYear(1)" id="year-btn-1" class="year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-cyan-500 text-slate-950 shadow-md">السنة الأولى</button>
      <button onclick="setAcademicYear(2)" id="year-btn-2" class="year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-slate-800 text-slate-300 hover:text-white">السنة الثانية</button>
      <button onclick="setAcademicYear(3)" id="year-btn-3" class="year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-slate-800 text-slate-300 hover:text-white">السنة الثالثة</button>
      <button onclick="setAcademicYear(4)" id="year-btn-4" class="year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-slate-800 text-slate-300 hover:text-white">السنة الرابعة</button>
      <button onclick="setAcademicYear(5)" id="year-btn-5" class="year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-slate-800 text-slate-300 hover:text-white">السنة الخامسة</button>
     </div>
    </div>
    <!-- Active Year Summary Header -->
    <div id="year-info-box" class="glass-card p-6 rounded-2xl border-r-4 border-r-cyan-400 flex flex-col md:flex-row items-start md:items-center justify-between gap-4">
     <div>
      <span id="year-badge" class="px-3 py-1 rounded-full bg-cyan-950 text-cyan-400 border border-cyan-800/60 text-xs font-bold">المرحلة الأولى</span>
      <h3 id="year-title" class="text-xl font-black text-white mt-2">السنة الأولى: الأساسيات والتشريح</h3>
      <p id="year-desc" class="text-sm text-slate-300 mt-1">التركيز على علم تشريح الإنسان والأنسجة ووظائف الأعضاء والتفاعلات الحيوية.</p>
     </div>
     <div class="flex items-center gap-3">
      <div class="text-left">
       <span class="text-xs text-slate-400 block">عدد المقررات المتاحة</span> <span id="year-course-count" class="text-lg font-bold text-cyan-400">4 مواد أساسية</span>
      </div>
     </div>
    </div>
    <!-- Search Bar -->
    <div class="relative">
     <i class="fa-solid fa-magnifying-glass absolute right-4 top-3.5 text-slate-500"></i> <input type="text" id="course-search-input" onkeyup="filterCourses()" placeholder="ابحث باسم المادة أو المحاضرة..." class="w-full pl-4 pr-11 py-3 bg-slate-900/90 border border-slate-700/80 rounded-xl text-slate-200 text-sm focus:outline-none focus:border-cyan-400 transition-colors">
    </div>
    <!-- Dynamic Course Cards Grid -->
    <div id="courses-grid" class="grid md:grid-cols-2 gap-6">
     <!-- Courses injected dynamically via JS -->
    </div>
   </section>
   <!-- ================= SECTION 3: VODAFONE CASH ACTIVATION TAB ================= -->
   <section id="tab-activation" class="hidden space-y-8">
    <div class="text-center max-w-3xl mx-auto space-y-3">
     <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-rose-950/80 border border-rose-800/50 text-rose-400 text-xs font-bold">
      <i class="fa-solid fa-shield-halved"></i> تفعيل الاشتراك المباشر
     </div>
     <h2 class="text-3xl font-black text-white">اشتراك كورسات دكتور سعاد التعليمية</h2>
     <p class="text-slate-300 text-sm leading-relaxed">قم بتحويل رسوم الاشتراك عبر فودافون كاش واملأ بيانات التحويل لتفعيل حسابك والوصول الكامل لجميع المواد والأطلسات فوراً.</p>
    </div>
    <div class="grid lg:grid-cols-12 gap-8 items-start">
     <!-- Left Column: Instructions and Vodafone Cash Banner -->
     <div class="lg:col-span-5 space-y-6">
      <div class="glass-card p-6 rounded-2xl border border-rose-500/40 relative overflow-hidden bg-slate-950/90 glow-voda">
       <div class="flex items-center justify-between border-b border-slate-800 pb-4 mb-4">
        <span class="text-xs font-extrabold text-rose-400 uppercase tracking-widest">رقم تحويل فودافون كاش</span> <i class="fa-solid fa-mobile-retro text-rose-500 text-xl"></i>
       </div>
       <div class="bg-slate-900 p-4 rounded-xl border border-rose-900/60 text-center mb-4">
        <span class="text-xs text-slate-400 block mb-1">الرقم المخصص لتلقي التحويلات</span> <span class="text-3xl font-mono font-black text-rose-500 tracking-widest select-all" id="activation-voda-num">01063415687</span>
       </div>
       <button onclick="copyVodafoneNumber()" class="w-full bg-rose-600 hover:bg-rose-500 text-white font-bold py-3.5 rounded-xl transition-all shadow-lg shadow-rose-600/30 flex items-center justify-center gap-2 text-sm"><i class="fa-regular fa-copy text-base"></i> <span id="copy-text-act">نسخ الرقم فوراً</span></button>
      </div>
      <!-- Steps -->
      <div class="glass-card p-6 rounded-2xl border border-slate-800 space-y-4">
       <h4 class="font-bold text-white text-base border-b border-slate-800 pb-3 flex items-center gap-2"><i class="fa-solid fa-list-check text-cyan-400"></i> خطوات تفعيل الاشتراك:</h4>
       <div class="space-y-3.5 text-sm text-slate-300">
        <div class="flex items-start gap-3">
         <span class="w-6 h-6 rounded-full bg-slate-800 text-cyan-400 font-bold flex items-center justify-center text-xs shrink-0 mt-0.5">١</span>
         <p>قم بتحويل المبلغ إلى الرقم المعلن أعلاه عبر تطبيق Ana Vodafone أو كود <code class="text-rose-400 font-mono">*9#</code>.</p>
        </div>
        <div class="flex items-start gap-3">
         <span class="w-6 h-6 rounded-full bg-slate-800 text-cyan-400 font-bold flex items-center justify-center text-xs shrink-0 mt-0.5">٢</span>
         <p>احتفظ برقم عملية التحويل أو قم بأخذ لقطة شاشة (Screenshot) لرسالة التحويل.</p>
        </div>
        <div class="flex items-start gap-3">
         <span class="w-6 h-6 rounded-full bg-slate-800 text-cyan-400 font-bold flex items-center justify-center text-xs shrink-0 mt-0.5">٣</span>
         <p>ادخل بياناتك في النموذج المجاور وقم بضغط "إرسال طلب التفعيل".</p>
        </div>
        <div class="flex items-start gap-3">
         <span class="w-6 h-6 rounded-full bg-slate-800 text-cyan-400 font-bold flex items-center justify-center text-xs shrink-0 mt-0.5">٤</span>
         <p>يتم مراجعة الطلب تلقائياً وتفعيل المحاضرات على حسابك في خلال دقائق.</p>
        </div>
       </div>
      </div>
     </div>
     <!-- Right Column: Interactive Activation Submission Form -->
     <div class="lg:col-span-7">
      <div class="glass-card p-6 sm:p-8 rounded-2xl border border-slate-700/80">
       <h3 class="text-xl font-bold text-white mb-6 flex items-center gap-2"><i class="fa-solid fa-paper-plane text-teal-400"></i> نموذج تأكيد وتحويل الاشتراك</h3>
       <form id="activation-form" onsubmit="handleActivationSubmit(event)" class="space-y-5">
        <!-- Student Name -->
        <div>
         <label class="block text-xs font-bold text-slate-300 mb-2">اسم الطالب ثلاثي *</label> <input type="text" id="student-name" required placeholder="أدخل اسمك بالكامل..." class="w-full px-4 py-3 bg-slate-900 border border-slate-700 rounded-xl text-slate-200 text-sm focus:outline-none focus:border-cyan-400">
        </div>
        <div class="grid md:grid-cols-2 gap-4">
         <!-- Phone -->
         <div>
          <label class="block text-xs font-bold text-slate-300 mb-2">رقم الموبايل (للتواصل والواتساب) *</label> <input type="tel" id="student-phone" required placeholder="01xxxxxxxxx" class="w-full px-4 py-3 bg-slate-900 border border-slate-700 rounded-xl text-slate-200 text-sm focus:outline-none focus:border-cyan-400 font-mono">
         </div>
         <!-- Academic Year -->
         <div>
          <label class="block text-xs font-bold text-slate-300 mb-2">السنة الدراسية *</label> <select id="student-year" required class="w-full px-4 py-3 bg-slate-900 border border-slate-700 rounded-xl text-slate-200 text-sm focus:outline-none focus:border-cyan-400"> <option value="">اختر سنتك الدراسية...</option> <option value="السنة الأولى">السنة الأولى (Anatomy &amp; Physio)</option> <option value="السنة الثانية">السنة الثانية (Patho &amp; Pharma)</option> <option value="السنة الثالثة">السنة الثالثة (Internal Med &amp; Forensic)</option> <option value="السنة الرابعة">السنة الرابعة (Surgery &amp; Pediatrics)</option> <option value="السنة الخامسة">السنة الخامسة (Obs/Gyn &amp; ENT/Opthalmo)</option> </select>
         </div>
        </div>
        <div class="grid md:grid-cols-2 gap-4">
         <!-- Vodafone Cash Sender Number -->
         <div>
          <label class="block text-xs font-bold text-slate-300 mb-2">رقم الموبايل المحول منه فودافون كاش *</label> <input type="tel" id="sender-number" required placeholder="الرقم الذي قمت بالتحويل منه..." class="w-full px-4 py-3 bg-slate-900 border border-slate-700 rounded-xl text-slate-200 text-sm focus:outline-none focus:border-cyan-400 font-mono">
         </div>
         <!-- Transaction Ref Code -->
         <div>
          <label class="block text-xs font-bold text-slate-300 mb-2">رقم العملية / الإشعار</label> <input type="text" id="trx-code" placeholder="مثال: TRX-884120" class="w-full px-4 py-3 bg-slate-900 border border-slate-700 rounded-xl text-slate-200 text-sm focus:outline-none focus:border-cyan-400 font-mono">
         </div>
        </div>
        <!-- Upload Receipt -->
        <div>
         <label class="block text-xs font-bold text-slate-300 mb-2">إرفاق صورة التحويل / الإشعار (اختياري)</label>
         <div class="border-2 border-dashed border-slate-700 hover:border-cyan-400/60 rounded-xl p-4 text-center cursor-pointer transition-colors bg-slate-900/50" onclick="document.getElementById('receipt-file').click()">
          <input type="file" id="receipt-file" class="hidden" accept="image/*" onchange="previewFile(event)"> <i class="fa-solid fa-cloud-arrow-up text-2xl text-slate-400 mb-1"></i> <span id="file-label" class="block text-xs text-slate-400">اضغط لإرفاق صورة إشعار التحويل</span>
         </div>
        </div>
        <!-- Submit Button -->
        <button type="submit" id="submit-act-btn" class="w-full bg-gradient-to-r from-teal-500 to-cyan-500 hover:from-teal-400 hover:to-cyan-400 text-slate-950 font-black py-4 rounded-xl shadow-lg shadow-teal-500/20 transition-all flex items-center justify-center gap-2 text-base"><i class="fa-solid fa-paper-plane"></i> <span>إرسال طلب التفعيل الآن</span></button>
       </form>
       <!-- Activation Alert Notification -->
       <div id="activation-status-box" class="hidden mt-6 p-4 rounded-xl bg-emerald-950/80 border border-emerald-500/50 text-emerald-300 space-y-2">
        <div class="flex items-center gap-2 font-bold text-sm">
         <i class="fa-solid fa-circle-check text-emerald-400 text-lg"></i> <span>تم استلام طلب التفعيل بنجاح!</span>
        </div>
        <p class="text-xs text-slate-300 leading-relaxed">جاري مراجعة طلبك ومطابقة رقم العملية والتحويل. سيتم تفعيل حسابك وتلقي إشعار التأكيد عبر الواتساب فوراً.</p>
       </div>
      </div>
     </div>
    </div>
   </section>
   <!-- ================= SECTION 4: INTERACTIVE QUIZ TAB ================= -->
   <section id="tab-quiz" class="hidden space-y-8">
    <div class="text-center max-w-2xl mx-auto">
     <span class="px-3 py-1 rounded-full bg-emerald-950 text-emerald-400 border border-emerald-800/60 text-xs font-bold">بنك الأسئلة التفاعلي</span>
     <h2 class="text-3xl font-black text-white mt-2">اختبارات إكلينيكية مجابة</h2>
     <p class="text-slate-400 text-sm mt-1">تدرب على نمط أسئلة الـ MCQs مع تقييم وتفسير علمي مباشر لكل إجابة.</p>
    </div>
    <div class="max-w-3xl mx-auto glass-card rounded-3xl p-6 sm:p-8 border border-slate-700/80">
     <!-- Quiz Progress Bar -->
     <div class="flex items-center justify-between text-xs text-slate-400 mb-2">
      <span id="quiz-question-number">السؤال 1 من 3</span> <span id="quiz-score" class="text-cyan-400 font-bold">النقاط: 0</span>
     </div>
     <div class="w-full bg-slate-800 h-2 rounded-full overflow-hidden mb-6">
      <div id="quiz-progress" class="bg-gradient-to-r from-cyan-400 to-emerald-400 h-full w-1/3 transition-all duration-300"></div>
     </div>
     <!-- Active Question Container -->
     <div id="quiz-content" class="space-y-6">
      <div class="inline-block px-3 py-1 rounded-md bg-slate-800 text-cyan-400 text-xs font-bold" id="quiz-category">السنة الثانية - علم الأدوية (Pharmacology)</div>
      <h3 class="text-lg sm:text-xl font-bold text-white leading-relaxed" id="quiz-question-text">أي من الأدوية التالية يعتبر الاختيار الأول (First-line) لعلاج ارتفاع ضغط الدم لمريض سكري للحفاظ على وظائف الكلى؟</h3>
      <!-- MCQ Options -->
      <div class="space-y-3" id="quiz-options-container">
       <!-- Injected via JS -->
      </div>
      <!-- Answer Explanation Box -->
      <div id="quiz-explanation" class="hidden p-4 rounded-xl bg-slate-900 border border-slate-700 text-sm space-y-1">
       <span class="font-bold text-cyan-400 block">التفسير العلمي للإجابة:</span>
       <p class="text-slate-300 text-xs leading-relaxed" id="explanation-text"></p>
      </div>
      <!-- Next Question Action -->
      <div class="flex justify-end pt-2">
       <button id="next-quiz-btn" onclick="nextQuizQuestion()" class="hidden bg-cyan-500 hover:bg-cyan-400 text-slate-950 font-black px-6 py-2.5 rounded-xl text-sm transition-all flex items-center gap-2"><span>السؤال التالي</span> <i class="fa-solid fa-arrow-left"></i></button>
      </div>
     </div>
    </div>
   </section>
  </main>
  <!-- Interactive Course & Video Modal -->
  <div id="course-modal" class="fixed inset-0 z-50 hidden bg-slate-950/80 backdrop-blur-md flex items-center justify-center p-4">
   <div class="glass-card w-full max-w-4xl rounded-3xl border border-slate-700 overflow-hidden shadow-2xl flex flex-col max-h-[90vh]">
    <!-- Modal Header -->
    <div class="p-5 border-b border-slate-800 flex items-center justify-between bg-slate-900/90">
     <div class="flex items-center space-x-3 space-x-reverse">
      <div class="w-10 h-10 rounded-xl bg-cyan-500/20 text-cyan-400 flex items-center justify-center font-bold">
       <i class="fa-solid fa-circle-play text-lg"></i>
      </div>
      <div>
       <h3 id="modal-course-title" class="text-base sm:text-lg font-black text-white">عنوان المقرر الطبي</h3>
       <span id="modal-course-year" class="text-xs text-slate-400">السنة الدراسية</span>
      </div>
     </div>
     <button onclick="closeCourseModal()" class="w-9 h-9 rounded-xl bg-slate-800 text-slate-400 hover:text-white flex items-center justify-center border border-slate-700"><i class="fa-solid fa-xmark text-lg"></i></button>
    </div>
    <!-- Modal Content (Player & Lessons) -->
    <div class="p-6 overflow-y-auto space-y-6 custom-scrollbar">
     <!-- Video Interactive Player Screen Placeholder -->
     <div class="relative aspect-video rounded-2xl bg-slate-950 border border-slate-800 overflow-hidden flex items-center justify-center group">
      <div class="text-center p-6 space-y-3">
       <div class="w-16 h-16 rounded-full bg-cyan-500/20 text-cyan-400 flex items-center justify-center text-2xl mx-auto group-hover:scale-110 transition-transform cursor-pointer border border-cyan-500/30">
        <i class="fa-solid fa-play ml-1"></i>
       </div>
       <h4 id="modal-video-title" class="font-bold text-white text-sm">المحاضرة الأولى: الشرح والأساسيات</h4>
       <p class="text-xs text-slate-400">مدة الفيديو: 45 دقيقة • جودة شاشة عالية HD</p>
      </div>
     </div>
     <!-- Lessons & PDF Downloads -->
     <div>
      <h4 class="font-bold text-white text-sm mb-3 flex items-center justify-between"><span>قائمة المحاضرات وملفات الـ PDF المرفقة</span> <span class="text-xs text-cyan-400">تحميل المذكرات الملونة</span></h4>
      <div id="modal-lessons-list" class="space-y-2">
       <!-- Dynamic Lesson Items -->
      </div>
     </div>
    </div>
    <!-- Modal Footer -->
    <div class="p-4 bg-slate-900/90 border-t border-slate-800 flex items-center justify-between">
     <span class="text-xs text-slate-400">منصة دكتور سعاد التعليمية - Dr. Soad Academy</span>
     <button onclick="switchTab('activation'); closeCourseModal();" class="bg-rose-600 hover:bg-rose-500 text-white text-xs font-bold px-4 py-2 rounded-xl transition-all flex items-center gap-1.5"><i class="fa-solid fa-key"></i> <span>تفعيل الكورس بفودافون كاش</span></button>
    </div>
   </div>
  </div>
  <!-- Footer -->
  <footer class="border-t border-slate-800/80 bg-slate-950/80 py-8 mt-12">
   <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center justify-between gap-4">
    <div class="flex items-center space-x-3 space-x-reverse">
     <div class="w-8 h-8 rounded-lg bg-cyan-500/20 text-cyan-400 flex items-center justify-center font-bold">
      <i class="fa-solid fa-user-doctor text-sm"></i>
     </div>
     <span class="font-bold text-sm text-slate-200">دكتور سعاد - Dr. Soad Medical Academy</span>
    </div>
    <div class="text-xs text-slate-400 text-center md:text-right">
     رقم تحويل فودافون كاش المعتمد: <span class="font-mono text-rose-400 font-bold text-sm">01063415687</span>
    </div>
    <p class="text-xs text-slate-500">© جميع الحقوق محفوظة لمنصة دكتور سعاد التعليمية.</p>
   </div>
  </footer>
  <script>
        /* ================= MEDICAL CURRICULUM DATA ================= */
        const curriculumData = {
            1: {
                badge: "السنة الأولى (الأساسيات)",
                title: "المناهج الطبية للسنة الأولى",
                desc: "دراسة شاملة لهيكل جسم الإنسان، وظائف الأعضاء والأنسجة والتفاعلات الحيوية.",
                courses: [
                    {
                        id: "c101",
                        title: "التشريح (Anatomy)",
                        desc: "شرح تشريح العظام، العضلات والأعصاب والأوعية الدموية للطرف العلوي والسفلي.",
                        lessonsCount: "18 محاضرة",
                        pdfNotes: "أطلس التشريح الملون PDF",
                        icon: "fa-bone",
                        lessons: ["Intro to Human Anatomy", "Upper Limb Muscle Anatomy", "Lower Limb Osteology", "Thorax & Abdomen Anatomy"]
                    },
                    {
                        id: "c102",
                        title: "وظائف الأعضاء (Physiology)",
                        desc: "فهم العمليات الحيوية للخلية، الجهاز العصبي، والدورة الدموية.",
                        lessonsCount: "16 محاضرة",
                        pdfNotes: "ملخص فيسيولوجي شامل",
                        icon: "fa-heart-pulse",
                        lessons: ["Cell & Membrane Physiology", "Autonomic Nervous System", "Blood & Plasma Physiology", "Cardiovascular Basics"]
                    },
                    {
                        id: "c103",
                        title: "علم الأنسجة والكيمياء الحيوية (Histology & Biochem)",
                        desc: "فحص الخلايا تحت المجهر وأيض الكربوهيدرات والبروتينات والإنزيمات.",
                        lessonsCount: "20 محاضرة",
                        pdfNotes: "شرائح المجهر والإنزيمات PDF",
                        icon: "fa-dna",
                        lessons: ["Epithelial Tissue Histology", "Enzymes & Metabolism", "Carbohydrate Metabolism", "Protein Structure & Synthesis"]
                    }
                ]
            },
            2: {
                badge: "السنة الثانية (المرض والأدوية)",
                title: "المناهج الطبية للسنة الثانية",
                desc: "دراسة علم الأمراض، ميكانيكية تأثير الأدوية، والأحياء الدقيقة الطبية.",
                courses: [
                    {
                        id: "c201",
                        title: "علم الأمراض (Pathology)",
                        desc: "دراسة تغيرات الأنسجة عند الإصابة بالتهابات، أورام وتلف الخلايا.",
                        lessonsCount: "22 محاضرة",
                        pdfNotes: "أطلس باثولوجي الأورام",
                        icon: "fa-microscope",
                        lessons: ["Cell Injury & Adaptation", "Acute & Chronic Inflammation", "Neoplasia & Tumor Markers", "Hemodynamic Pathology"]
                    },
                    {
                        id: "c202",
                        title: "علم الأدوية (Pharmacology)",
                        desc: "تأثير العقاقير الطبية والجرعات وديناميكية العلاج في أجهزة الجسم.",
                        lessonsCount: "24 محاضرة",
                        pdfNotes: "جداول تصنيف الأدوية PDF",
                        icon: "fa-pills",
                        lessons: ["Pharmacokinetics & Dynamics", "Autonomic Nervous System Drugs", "CVS Medications", "Antimicrobial Chemotherapy"]
                    },
                    {
                        id: "c203",
                        title: "الأحياء الدقيقة (Microbiology)",
                        desc: "البكتيريا، الفيروسات، الفطريات، والمناعة الطبية ضد الأمراض.",
                        lessonsCount: "16 محاضرة",
                        pdfNotes: "ملخص البكتيريا والفيروسات",
                        icon: "fa-bugs",
                        lessons: ["General Bacteriology", "Virology & Vaccines", "Medical Immunology", "Pathogenic Parasites"]
                    }
                ]
            },
            3: {
                badge: "السنة الثالثة (الإكلينيكي المبدئي)",
                title: "المناهج الطبية للسنة الثالثة",
                desc: "بداية التشخيص السريري، أخذ التاريخ المرضي، وعلم السموم والطب الشرعي.",
                courses: [
                    {
                        id: "c301",
                        title: "الباطنة العامة (Internal Medicine Intro)",
                        desc: "فحص أعراض الجهاز الدوري، التنفسي والهضمي وأخذ التاريخ المرضي.",
                        lessonsCount: "28 محاضرة",
                        pdfNotes: "دليل الفحص السريري والتاريخ المرضي",
                        icon: "fa-stethoscope",
                        lessons: ["Clinical History Taking", "Cardiology Examination", "Pulmonology Basics", "Gastrointestinal Assessment"]
                    },
                    {
                        id: "c302",
                        title: "الطب الشرعي وعلم السموم (Forensic & Toxicology)",
                        desc: "تشخيص حالات التسمم الحاد، الإصابات الجنائية والتقرير الطبي الشرعي.",
                        lessonsCount: "15 محاضرة",
                        pdfNotes: "مذكرة السموم الحادة والتقرير الشرعي",
                        icon: "fa-scale-balanced",
                        lessons: ["Death Signs & Identification", "Wounds & Mechanical Injuries", "Acute Heavy Metal Poisoning", "Drug Toxicity Management"]
                    }
                ]
            },
            4: {
                badge: "السنة الرابعة (الجراحة والأطفال)",
                title: "المناهج الطبية للسنة الرابعة",
                desc: "تقنيات الجراحة العامة، التقييم الجراحي، ورعاية وتطور الأطفال حديثي الولادة.",
                courses: [
                    {
                        id: "c401",
                        title: "الجراحة العامة (General Surgery)",
                        desc: "جراحة البطن، الأورام، الفتوق الجراحية والتعامل مع الطوارئ والحروق.",
                        lessonsCount: "30 محاضرة",
                        pdfNotes: "أطلس العمليات الجراحية PDF",
                        icon: "fa-scalpel",
                        lessons: ["Aseptic Techniques & Wounds", "Abdominal Wall & Hernia", "Gastrointestinal Surgery", "Trauma & Burn Care"]
                    },
                    {
                        id: "c402",
                        title: "طب الأطفال (Pediatrics)",
                        desc: "مراحل نمو الطفل، أمراض حديثي الولادة، التطعيمات وسوء التغذية.",
                        lessonsCount: "25 محاضرة",
                        pdfNotes: "جدول التطعيمات وجرعات الأطفال",
                        icon: "fa-baby",
                        lessons: ["Child Growth & Development", "Neonatology & Prematurity", "Pediatric Nutrition & Rickets", "Infectious Diseases in Children"]
                    }
                ]
            },
            5: {
                badge: "السنة الخامسة (التخصصات)",
                title: "المناهج الطبية للسنة الخامسة",
                desc: "أمراض النساء والتوليد، طب وجراحة العيون، والأنف والأذن والحنجرة.",
                courses: [
                    {
                        id: "c501",
                        title: "النساء والتوليد (Obstetrics & Gynecology)",
                        desc: "متابعة الحمل، الولادة الطبيعية والقيصرية، والأمراض النسائية المختلفة.",
                        lessonsCount: "26 محاضرة",
                        pdfNotes: "مذكرة التوليد والعمليات النسائية",
                        icon: "fa-person-pregnant",
                        lessons: ["Antenatal Care & Fetal Monitoring", "Normal & Abnormal Labor", "Gynecological Oncology", "Infertility Management"]
                    },
                    {
                        id: "c502",
                        title: "طب العيون والأنف والأذن (Ophthalmology & ENT)",
                        desc: "فحص العين وأمراض القرنية والشبكية، وأمراض الأذن الوسطى والحنجرة.",
                        lessonsCount: "22 محاضرة",
                        pdfNotes: "أطلس صور العيون والأنف والأذن",
                        icon: "fa-eye",
                        lessons: ["Refractive Errors & Cataract", "Glaucoma & Retinal Disorders", "Otitis Media & Hearing Loss", "Sinusitis & Tonsillitis"]
                    }
                ]
            }
        };

        /* ================= SAMPLE QUIZ DATA ================= */
        const quizQuestions = [
            {
                category: "السنة الثانية - علم الأدوية (Pharmacology)",
                question: "أي من الأدوية التالية يعتبر الاختيار الأول (First-line) لعلاج ارتفاع ضغط الدم لمريض سكري للحفاظ على وظائف الكلى؟",
                options: [
                    { text: "ACE Inhibitors (مثل Enalapril)", correct: true },
                    { text: "Beta Blockers (مثل Atenolol)", correct: false },
                    { text: "Loop Diuretics (مثل Furosemide)", correct: false },
                    { text: "Calcium Channel Blockers", correct: false }
                ],
                explanation: "تعتبر مثبطات ACE الاختيار الأول لأنها تحمي الكليتين من اعتلال السكري (Nephroprotective)."
            },
            {
                category: "السنة الأولى - التشريح (Anatomy)",
                question: "ما هي العضلة الرئيسية المسؤولة عن تنفس الإنسان وتفصل بين التجويف الصدري والبطني؟",
                options: [
                    { text: "Intercostal Muscles", correct: false },
                    { text: "Diaphragm (الحجاب الحاجز)", correct: true },
                    { text: "Rectus Abdominis", correct: false },
                    { text: "Pectoralis Major", correct: false }
                ],
                explanation: "الحجاب الحاجز هو العضلة الرئيسية للشهيق والزفير ويقسم التجويف الصدري عن البطني."
            },
            {
                category: "السنة الرابعة - الأطفال (Pediatrics)",
                question: "ما هو الفيتامين الموصى بإعطائه للوليد فور الولادة لمنع حالات النزيف الخاطف؟",
                options: [
                    { text: "فيتامين C", correct: false },
                    { text: "فيتامين D", correct: false },
                    { text: "فيتامين K", correct: true },
                    { text: "فيتامين B12", correct: false }
                ],
                explanation: "يُعطى فيتامين K للحديثي الولادة للوقاية من نزيف نقص عوامل التجلط المصاحبة لحديثي الولادة."
            }
        ];

        let currentQuizIndex = 0;
        let currentScore = 0;
        let activeYear = 1;

        /* ================= NAVIGATION & TAB SWITCHING ================= */
        function switchTab(tabId) {
            const tabs = ['home', 'years', 'activation', 'quiz'];
            tabs.forEach(t => {
                const el = document.getElementById(`tab-${t}`);
                if(el) el.classList.add('hidden');

                const navBtn = document.getElementById(`nav-${t}`);
                if(navBtn) {
                    navBtn.classList.remove('text-cyan-400', 'bg-slate-800', 'border', 'border-slate-700/50');
                    navBtn.classList.add('text-slate-300');
                }
            });

            const activeEl = document.getElementById(`tab-${tabId}`);
            if(activeEl) activeEl.classList.remove('hidden');

            const activeNavBtn = document.getElementById(`nav-${tabId}`);
            if(activeNavBtn) {
                activeNavBtn.classList.add('text-cyan-400', 'bg-slate-800', 'border', 'border-slate-700/50');
                activeNavBtn.classList.remove('text-slate-300');
            }

            document.getElementById('mobile-menu').classList.add('hidden');
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        function toggleMobileMenu() {
            document.getElementById('mobile-menu').classList.toggle('hidden');
        }

        /* ================= ACADEMIC YEARS MANAGEMENT ================= */
        function selectYearAndOpen(year) {
            switchTab('years');
            setAcademicYear(year);
        }

        function setAcademicYear(year) {
            activeYear = year;
            
            for(let i = 1; i <= 5; i++) {
                const btn = document.getElementById(`year-btn-${i}`);
                if(i === year) {
                    btn.className = "year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-cyan-500 text-slate-950 shadow-md";
                } else {
                    btn.className = "year-tab-btn px-4 py-2 rounded-xl text-xs font-bold whitespace-nowrap bg-slate-800 text-slate-300 hover:text-white";
                }
            }

            const data = curriculumData[year];
            if(!data) return;

            document.getElementById('year-badge').innerText = data.badge;
            document.getElementById('year-title').innerText = data.title;
            document.getElementById('year-desc').innerText = data.desc;
            document.getElementById('year-course-count').innerText = `${data.courses.length} مواد مخصصة`;

            renderCourses(data.courses);
        }

        function renderCourses(courses) {
            const grid = document.getElementById('courses-grid');
            grid.innerHTML = '';

            courses.forEach(course => {
                const card = document.createElement('div');
                card.className = "glass-card rounded-2xl p-6 border border-slate-800 hover:border-cyan-500/50 transition-all flex flex-col justify-between group";
                card.innerHTML = `
                    <div>
                        <div class="flex items-center justify-between mb-4">
                            <div class="w-12 h-12 rounded-2xl bg-cyan-500/10 text-cyan-400 flex items-center justify-center text-xl group-hover:scale-110 transition-transform">
                                <i class="fa-solid ${course.icon}"></i>
                            </div>
                            <span class="text-xs px-2.5 py-1 rounded-md bg-slate-800 text-slate-300 font-medium">${course.lessonsCount}</span>
                        </div>
                        <h4 class="text-lg font-black text-white mb-2 group-hover:text-cyan-400 transition-colors">${course.title}</h4>
                        <p class="text-xs text-slate-300 leading-relaxed mb-4">${course.desc}</p>
                        <div class="flex items-center gap-2 text-xs text-emerald-400 bg-emerald-950/40 px-3 py-1.5 rounded-lg border border-emerald-800/40 mb-6">
                            <i class="fa-solid fa-file-pdf"></i>
                            <span>${course.pdfNotes}</span>
                        </div>
                    </div>

                    <div class="flex items-center gap-3 pt-4 border-t border-slate-800">
                        <button onclick="openCourseModal('${course.id}')" class="flex-1 bg-slate-800 hover:bg-slate-700 text-white font-bold py-2.5 rounded-xl text-xs transition-all flex items-center justify-center gap-1.5">
                            <i class="fa-solid fa-play text-cyan-400"></i>
                            <span>عرض المحاضرات</span>
                        </button>
                        <button onclick="switchTab('activation')" class="bg-rose-600 hover:bg-rose-500 text-white font-bold px-4 py-2.5 rounded-xl text-xs transition-all flex items-center justify-center gap-1">
                            <i class="fa-solid fa-lock-open"></i>
                            <span>تفعيل</span>
                        </button>
                    </div>
                `;
                grid.appendChild(card);
            });
        }

        function filterCourses() {
            const query = document.getElementById('course-search-input').value.toLowerCase();
            const yearData = curriculumData[activeYear];
            if(!yearData) return;

            const filtered = yearData.courses.filter(c => 
                c.title.toLowerCase().includes(query) || c.desc.toLowerCase().includes(query)
            );
            renderCourses(filtered);
        }

        /* ================= COURSE MODAL ================= */
        function openCourseModal(courseId) {
            let foundCourse = null;
            let foundYear = "";

            Object.keys(curriculumData).forEach(y => {
                curriculumData[y].courses.forEach(c => {
                    if(c.id === courseId) {
                        foundCourse = c;
                        foundYear = curriculumData[y].title;
                    }
                });
            });

            if(!foundCourse) return;

            document.getElementById('modal-course-title').innerText = foundCourse.title;
            document.getElementById('modal-course-year').innerText = foundYear;
            document.getElementById('modal-video-title').innerText = `المحاضرة الأولى: ${foundCourse.title}`;

            const lessonsList = document.getElementById('modal-lessons-list');
            lessonsList.innerHTML = '';

            foundCourse.lessons.forEach((l, idx) => {
                const item = document.createElement('div');
                item.className = "flex items-center justify-between p-3 rounded-xl bg-slate-900 border border-slate-800 hover:border-slate-700 transition-colors";
                item.innerHTML = `
                    <div class="flex items-center space-x-3 space-x-reverse">
                        <span class="w-6 h-6 rounded-md bg-slate-800 text-slate-400 font-bold text-xs flex items-center justify-center">${idx + 1}</span>
                        <span class="text-xs font-bold text-slate-200">${l}</span>
                    </div>
                    <div class="flex items-center gap-2">
                        <span class="text-[10px] bg-slate-800 text-slate-400 px-2 py-0.5 rounded">PDF + فيديو</span>
                        <i class="fa-solid fa-lock text-slate-500 text-xs"></i>
                    </div>
                `;
                lessonsList.appendChild(item);
            });

            document.getElementById('course-modal').classList.remove('hidden');
        }

        function closeCourseModal() {
            document.getElementById('course-modal').classList.add('hidden');
        }

        /* ================= VODAFONE CASH COPY & FORM ================= */
        function copyVodafoneNumber() {
            const num = "01063415687";
            const tempInput = document.createElement("input");
            tempInput.value = num;
            document.body.appendChild(tempInput);
            tempInput.select();
            document.execCommand("copy");
            document.body.removeChild(tempInput);

            const homeBtn = document.getElementById('copy-text-home');
            const actBtn = document.getElementById('copy-text-act');
            
            if(homeBtn) homeBtn.innerText = "تم النسخ ✓";
            if(actBtn) actBtn.innerText = "تم النسخ بنجاح ✓";

            setTimeout(() => {
                if(homeBtn) homeBtn.innerText = "نسخ الرقم";
                if(actBtn) actBtn.innerText = "نسخ الرقم فوراً";
            }, 3000);
        }

        function previewFile(e) {
            const file = e.target.files[0];
            const label = document.getElementById('file-label');
            if(file) {
                label.innerText = `تم اختيار: ${file.name}`;
                label.classList.add('text-cyan-400');
            }
        }

        function handleActivationSubmit(e) {
            e.preventDefault();
            const btn = document.getElementById('submit-act-btn');
            const statusBox = document.getElementById('activation-status-box');

            btn.disabled = true;
            btn.innerHTML = `<i class="fa-solid fa-circle-notch animate-spin"></i> <span>جاري معالجة وإرسال الطلب...</span>`;

            setTimeout(() => {
                btn.disabled = false;
                btn.innerHTML = `<i class="fa-solid fa-check-circle"></i> <span>تم إرسال طلب التفعيل</span>`;
                btn.className = "w-full bg-emerald-600 text-white font-black py-4 rounded-xl shadow-lg transition-all flex items-center justify-center gap-2 text-base";
                
                statusBox.classList.remove('hidden');
                document.getElementById('activation-form').reset();
                document.getElementById('file-label').innerText = "اضغط لإرفاق صورة إشعار التحويل";
            }, 1200);
        }

        /* ================= INTERACTIVE QUIZ LOGIC ================= */
        function loadQuizQuestion() {
            const q = quizQuestions[currentQuizIndex];
            if(!q) return;

            document.getElementById('quiz-question-number').innerText = `السؤال ${currentQuizIndex + 1} من ${quizQuestions.length}`;
            document.getElementById('quiz-score').innerText = `النقاط: ${currentScore}`;
            document.getElementById('quiz-progress').style.width = `${((currentQuizIndex + 1) / quizQuestions.length) * 100}%`;
            
            document.getElementById('quiz-category').innerText = q.category;
            document.getElementById('quiz-question-text').innerText = q.question;

            const container = document.getElementById('quiz-options-container');
            container.innerHTML = '';

            document.getElementById('quiz-explanation').classList.add('hidden');
            document.getElementById('next-quiz-btn').classList.add('hidden');

            q.options.forEach((opt, idx) => {
                const btn = document.createElement('button');
                btn.className = "w-full text-right p-4 rounded-xl bg-slate-900 border border-slate-800 hover:border-cyan-500/50 font-bold text-sm text-slate-200 transition-all flex items-center justify-between group";
                btn.onclick = () => checkAnswer(idx);
                btn.innerHTML = `
                    <span class="flex items-center gap-3">
                        <span class="w-6 h-6 rounded-md bg-slate-800 text-slate-400 text-xs flex items-center justify-center group-hover:bg-cyan-500 group-hover:text-slate-950 font-bold">${String.fromCharCode(65 + idx)}</span>
                        <span>${opt.text}</span>
                    </span>
                    <i class="fa-regular fa-circle text-slate-600 group-hover:text-cyan-400"></i>
                `;
                container.appendChild(btn);
            });
        }

        function checkAnswer(selectedIndex) {
            const q = quizQuestions[currentQuizIndex];
            const container = document.getElementById('quiz-options-container');
            const buttons = container.querySelectorAll('button');

            buttons.forEach(b => b.disabled = true);

            if(q.options[selectedIndex].correct) {
                buttons[selectedIndex].className = "w-full text-right p-4 rounded-xl bg-emerald-950/80 border border-emerald-500 text-emerald-300 font-bold text-sm transition-all flex items-center justify-between";
                buttons[selectedIndex].querySelector('i').className = "fa-solid fa-circle-check text-emerald-400 text-lg";
                currentScore += 10;
            } else {
                buttons[selectedIndex].className = "w-full text-right p-4 rounded-xl bg-rose-950/80 border border-rose-500 text-rose-300 font-bold text-sm transition-all flex items-center justify-between";
                buttons[selectedIndex].querySelector('i').className = "fa-solid fa-circle-xmark text-rose-400 text-lg";

                q.options.forEach((opt, idx) => {
                    if(opt.correct) {
                        buttons[idx].className = "w-full text-right p-4 rounded-xl bg-emerald-950/50 border border-emerald-600/60 text-emerald-300 font-bold text-sm flex items-center justify-between";
                    }
                });
            }

            document.getElementById('quiz-score').innerText = `النقاط: ${currentScore}`;
            document.getElementById('explanation-text').innerText = q.explanation;
            document.getElementById('quiz-explanation').classList.remove('hidden');
            document.getElementById('next-quiz-btn').classList.remove('hidden');
        }

        function nextQuizQuestion() {
            currentQuizIndex++;
            if(currentQuizIndex < quizQuestions.length) {
                loadQuizQuestion();
            } else {
                const content = document.getElementById('quiz-content');
                content.innerHTML = `
                    <div class="text-center py-8 space-y-4">
                        <div class="w-20 h-20 bg-emerald-500/20 text-emerald-400 rounded-full flex items-center justify-center text-4xl mx-auto border border-emerald-500/30">
                            <i class="fa-solid fa-trophy"></i>
                        </div>
                        <h3 class="text-2xl font-black text-white">ممتاز! أنهيت كافة الأسئلة بنجاح</h3>
                        <p class="text-slate-300 text-sm">مجموع درجاتك النهائي: <span class="text-cyan-400 font-black text-lg">${currentScore} نقطة</span></p>
                        <button onclick="location.reload()" class="bg-gradient-to-r from-cyan-500 to-teal-500 text-slate-950 font-black px-6 py-3 rounded-xl text-sm shadow-lg">
                            إعادة الاختبار مرة أخرى
                        </button>
                    </div>
                `;
            }
        }

        // Initialize application when window is loaded
        window.addEventListener('DOMContentLoaded', () => {
            setAcademicYear(1);
            loadQuizQuestion();
        });
    </script>
 </body>
</html>
