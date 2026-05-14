<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>呂氏家庭生活資訊網 3.0</title>

  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" />
  <link href="https://unpkg.com/aos@2.3.4/dist/aos.css" rel="stylesheet" />

  <style>
    @import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@400;500;700;900&display=swap');
    body { font-family: "Noto Sans TC", sans-serif; background: #f8fafc; scroll-behavior: smooth; }
    .hero-bg { background: linear-gradient(135deg, rgba(255,255,255,0.9), rgba(240,244,255,0.95)); }
    .glass-card { backdrop-filter: blur(16px); background: rgba(255,255,255,0.8); border: 1px solid rgba(255,255,255,0.5); }
    .soft-shadow { box-shadow: 0 20px 40px rgba(15, 23, 42, 0.05); }
    .hover-float { transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); }
    .hover-float:hover { transform: translateY(-8px); box-shadow: 0 25px 50px rgba(15, 23, 42, 0.1); }
    .gradient-text { background: linear-gradient(to right, #6366f1, #0ea5e9); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    .no-scrollbar::-webkit-scrollbar { display: none; }
    video { border-radius: 2rem; width: 100%; height: auto; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
  </style>
</head>

<body class="text-slate-700">

  <nav class="bg-white/80 backdrop-blur-md sticky top-0 z-50 border-b border-slate-100">
    <div class="max-w-7xl mx-auto px-6 py-4 flex justify-between items-center">
      <div class="flex items-center gap-3">
        <div class="w-11 h-11 rounded-2xl bg-indigo-600 flex items-center justify-center text-white shadow-lg shadow-indigo-200">
          <i class="fa-solid fa-house"></i>
        </div>
        <div>
          <h1 class="font-bold text-lg text-slate-800 leading-tight">呂氏家庭資訊網<span class="text-indigo-600 text-sm ml-1">3.0</span></h1>
          <p class="text-[10px] uppercase tracking-widest text-slate-400 font-bold">Family Hub</p>
        </div>
      </div>
      
      <div class="hidden md:flex items-center gap-6 text-sm font-bold">
        <a href="#home" class="text-slate-500 hover:text-indigo-600 transition-colors">首頁</a>
        <a href="#members" class="text-slate-500 hover:text-indigo-600 transition-colors">幕僚團隊</a>
        <a href="#notice" class="text-slate-500 hover:text-indigo-600 transition-colors">公告與活動</a>
        <button onclick="openHistoryModal()" class="flex items-center gap-2 px-4 py-2 rounded-xl bg-indigo-50 text-indigo-600 hover:bg-indigo-600 hover:text-white transition-all shadow-sm border border-indigo-100">
          <i class="fa-solid fa-clock-rotate-left"></i> 歷史回顧
        </button>
      </div>
    </div>
  </nav>

  <section id="home" class="hero-bg min-h-[85vh] flex items-center overflow-hidden">
    <div class="max-w-7xl mx-auto px-6 py-16 grid lg:grid-cols-2 gap-16 items-center">
      <div data-aos="fade-right">
        <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-indigo-50 text-indigo-600 text-xs font-bold mb-6 border border-indigo-100">
          <i class="fa-solid fa-heart-pulse"></i> 溫馨家族數位空間
        </div>
        <h2 class="text-5xl md:text-7xl font-black leading-[1.1] text-slate-800">分享生活<br><span class="gradient-text">紀錄家庭日常</span></h2>
        <p class="mt-8 text-lg leading-relaxed text-slate-500 max-w-lg">呂氏家族 13 位成員的溫馨港灣，紀錄平凡生活中的不平凡。</p>
      </div>
      <div class="relative" data-aos="fade-left">
        <div class="glass-card rounded-[40px] p-10 soft-shadow border-white text-center max-w-sm mx-auto">
           <div class="w-20 h-20 rounded-full bg-emerald-50 flex items-center justify-center mx-auto mb-6 shadow-inner">
             <i class="fa-solid fa-shield-heart text-3xl text-emerald-500"></i>
           </div>
           <h3 class="text-2xl font-black text-slate-800 tracking-tight">LU FAMILY 3.0</h3>
           <p class="text-slate-400 mt-2 font-bold uppercase tracking-widest text-xs">版本 2026.05 正式上線</p>
        </div>
      </div>
    </div>
  </section>

  <section class="py-24 bg-white overflow-hidden">
    <div class="max-w-7xl mx-auto px-6">
      <div class="text-center mb-16" data-aos="fade-up">
        <h2 class="text-4xl font-black text-slate-800">近期活動回顧</h2>
        <div class="w-16 h-1.5 bg-pink-500 mx-auto mt-4 rounded-full"></div>
      </div>
      
      <div class="grid lg:grid-cols-12 gap-12 items-center">
        <div class="lg:col-span-6" data-aos="fade-right">
          <div class="rounded-[3rem] overflow-hidden shadow-2xl hover:scale-[1.02] transition-transform duration-500 border-8 border-white">
            <img src="S__23732244.jpg" alt="2026母親節活動合照" class="w-full h-auto">
          </div>
          <p class="mt-6 text-center text-slate-400 font-bold italic tracking-wide">2026母親節活動合照</p>
        </div>
        
        <div class="lg:col-span-6" data-aos="fade-left">
          <div class="glass-card p-8 rounded-[3.5rem] shadow-xl border-white">
            <video controls poster="video_poster.jpg">
              <source src="母親節MV.mp4" type="video/mp4">
            </video>
            <div class="mt-8 px-2 text-center lg:text-left">
              <h4 class="text-2xl font-black text-slate-800">2026 溫馨母親節慶生活動</h4>
              <p class="text-slate-500 mt-3 font-medium leading-relaxed">紀錄與家人相聚的每一刻喜悅與感人歌聲，愛在呂氏。</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="members" class="py-24 bg-slate-50">
    <div class="max-w-7xl mx-auto px-6 text-center">
      <div class="mb-20" data-aos="fade-up">
        <h2 class="text-4xl font-black text-slate-800">幕僚團隊</h2>
        <div class="w-16 h-1.5 bg-indigo-600 mx-auto mt-4 rounded-full"></div>
        <p class="text-slate-400 mt-4 font-bold italic text-sm">點擊成員卡片查看詳細介紹</p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <div onclick="openMemberModal('member1')" class="glass-card rounded-[35px] p-8 hover-float soft-shadow group cursor-pointer border-2 border-transparent hover:border-indigo-200">
          <div class="w-24 h-24 rounded-3xl bg-slate-200 flex items-center justify-center text-slate-400 text-4xl mb-6 mx-auto group-hover:bg-indigo-50 group-hover:text-indigo-400 transition-colors">
            <i class="fa-solid fa-user"></i>
          </div>
          <h3 class="text-2xl font-black text-slate-800">呂陳英妹</h3>
          <p class="text-indigo-600 font-bold text-sm mb-4">家庭長 / Decision Maker</p>
        </div>

        <div onclick="openMemberModal('member2')" class="glass-card rounded-[35px] p-8 hover-float soft-shadow group cursor-pointer border-2 border-transparent hover:border-emerald-200">
          <div class="w-24 h-24 rounded-3xl bg-emerald-50 mb-6 overflow-hidden shadow-md mx-auto border-4 border-white group-hover:scale-105 transition-transform">
            <img src="110417006.jpg" class="w-full h-full object-cover" alt="呂佳寯">
          </div>
          <h3 class="text-2xl font-black text-slate-800">呂佳寯</h3>
          <p class="text-emerald-600 font-bold text-sm mb-4">行政管理 / Operations</p>
        </div>

        <div onclick="openMemberModal('member3')" class="glass-card rounded-[35px] p-8 hover-float soft-shadow group cursor-pointer border-2 border-transparent hover:border-pink-200">
          <div class="w-24 h-24 rounded-3xl bg-slate-200 flex items-center justify-center text-slate-400 text-4xl mb-6 mx-auto group-hover:bg-pink-50 group-hover:text-pink-400 transition-colors">
            <i class="fa-solid fa-user"></i>
          </div>
          <h3 class="text-2xl font-black text-slate-800">呂佳芯</h3>
          <p class="text-pink-600 font-bold text-sm mb-4">分隊長 / Atmosphere</p>
        </div>
      </div>
    </div>
  </section>

  <section id="notice" class="py-24 bg-white">
    <div class="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-12">
      <div data-aos="fade-up">
        <div class="flex items-center gap-4 mb-8">
          <div class="w-12 h-12 rounded-2xl bg-orange-500 text-white flex items-center justify-center shadow-lg"><i class="fa-solid fa-bullhorn text-xl"></i></div>
          <h2 class="text-3xl font-black text-slate-800">最新公告</h2>
        </div>
        <div class="bg-slate-50 rounded-[40px] p-10 soft-shadow border border-white">
          <div class="flex justify-between mb-4">
            <span class="bg-red-500 text-white text-[10px] font-black px-4 py-1.5 rounded-full uppercase tracking-widest">Urgent</span>
            <span class="text-xs font-bold text-slate-400 italic">2026-05-15</span>
          </div>
          <h3 class="text-2xl font-black text-slate-800">114年度所得稅申報</h3>
          <p class="mt-4 text-slate-500 font-medium leading-relaxed">請成員儘早申報，申報期至 2026/06/01 止。</p>
        </div>
      </div>

      <div data-aos="fade-up" data-aos-delay="100">
        <div class="flex items-center gap-4 mb-8">
          <div class="w-12 h-12 rounded-2xl bg-emerald-500 text-white flex items-center justify-center shadow-lg"><i class="fa-solid fa-calendar-check text-xl"></i></div>
          <h2 class="text-3xl font-black text-slate-800">活動進度</h2>
        </div>
        <div class="bg-slate-50 rounded-[40px] p-10 soft-shadow border border-white space-y-8">
          <div class="flex items-center gap-5">
            <div class="w-4 h-4 rounded-full bg-slate-300"></div>
            <p class="text-lg font-black text-slate-800">母親節晚宴慶祝 <span class="text-slate-400 font-bold ml-3 text-sm">已結束</span></p>
          </div>
          <div class="flex items-center gap-5">
            <div class="w-4 h-4 rounded-full bg-indigo-600 ring-4 ring-indigo-50"></div>
            <p class="text-lg font-black text-slate-800 italic">中秋家族烤肉大會 <span class="text-indigo-500 font-bold ml-3 text-sm">規劃中</span></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <div id="historyModal" class="fixed inset-0 z-[110] flex items-center justify-center p-6 bg-slate-900/60 backdrop-blur-sm hidden" onclick="closeHistoryModal()">
    <div class="bg-white rounded-[40px] w-full max-w-xl shadow-2xl transition-all scale-95 opacity-0 duration-300" id="historyModalContainer" onclick="event.stopPropagation()">
      <div class="p-10 text-center">
        <div class="w-16 h-16 bg-indigo-50 text-indigo-600 rounded-2xl flex items-center justify-center text-2xl mx-auto mb-6 shadow-inner">
          <i class="fa-solid fa-clock-rotate-left"></i>
        </div>
        <h3 class="text-3xl font-black text-slate-800 mb-8 tracking-tight">歷史訊息回顧</h3>
        <div class="space-y-4 max-h-[40vh] overflow-y-auto pr-2 no-scrollbar text-left">
          <div class="p-6 rounded-3xl bg-slate-50 border border-slate-100">
            <span class="text-[10px] font-bold text-slate-400 uppercase tracking-widest">Archive | 2026.05.15</span>
            <h4 class="font-bold text-slate-800 mt-1">本單位3.0網頁已正式上線</h4>
          </div>
        </div>
        <button onclick="closeHistoryModal()" class="mt-10 px-10 py-3 rounded-2xl bg-indigo-600 text-white font-black hover:bg-indigo-700 transition shadow-lg shadow-indigo-100">關閉視窗</button>
      </div>
    </div>
  </div>

  <div id="memberModal" class="fixed inset-0 z-[100] flex items-center justify-center p-6 bg-slate-900/60 backdrop-blur-sm hidden" onclick="closeModal()">
    <div class="bg-white rounded-[50px] w-full max-w-md shadow-2xl transition-all scale-95 opacity-0 duration-300 overflow-hidden" id="modalContainer" onclick="event.stopPropagation()">
      <div class="relative h-32 bg-slate-100" id="modalTheme"></div>
      <div class="px-10 pb-10 text-center relative">
        <div id="modalAvatarBox" class="w-28 h-28 rounded-3xl mx-auto -mt-14 mb-6 overflow-hidden flex items-center justify-center text-4xl shadow-xl border-4 border-white bg-white"></div>
        <h3 id="modalName" class="text-3xl font-black text-slate-800 tracking-tight"></h3>
        <p id="modalNick" class="text-slate-400 font-bold text-sm mt-1 mb-6"></p>
        
        <div class="bg-slate-50 rounded-3xl p-6 text-left border border-slate-100">
          <div class="mb-4">
            <span class="text-[10px] font-black text-indigo-500 uppercase tracking-widest">職稱 Position</span>
            <p id="modalTitle" class="font-black text-slate-700 mt-1"></p>
          </div>
          <div>
            <span class="text-[10px] font-black text-indigo-500 uppercase tracking-widest">想要說什麼</span>
            <p id="modalBusiness" class="text-slate-500 text-sm font-medium leading-relaxed mt-1"></p>
          </div>
        </div>
        
        <button onclick="closeModal()" class="mt-8 w-full py-4 rounded-2xl bg-white border-2 border-slate-100 font-black text-slate-400 hover:bg-slate-50 hover:text-slate-800 transition-all">關閉詳細資訊</button>
      </div>
    </div>
  </div>

  <footer class="bg-white py-12 text-center border-t border-slate-100">
    <p class="text-[10px] font-black text-slate-300 uppercase tracking-[0.3em]">© 2026 LU FAMILY. ALL RIGHTS RESERVED.</p>
  </footer>

  <script src="https://unpkg.com/aos@2.3.4/dist/aos.js"></script>
  <script>
    AOS.init({ duration: 1000, once: true, easing: 'ease-out-quint' });

    // 歷史 Modal
    function openHistoryModal() {
      const modal = document.getElementById('historyModal');
      const container = document.getElementById('historyModalContainer');
      modal.classList.remove('hidden');
      setTimeout(() => { container.classList.remove('scale-95', 'opacity-0'); container.classList.add('scale-100', 'opacity-100'); }, 10);
    }
    function closeHistoryModal() {
      const modal = document.getElementById('historyModal');
      const container = document.getElementById('historyModalContainer');
      container.classList.add('scale-95', 'opacity-0');
      setTimeout(() => modal.classList.add('hidden'), 300);
    }

    // 幹部數據庫
    const memberData = {
      member1: { 
        name: "呂陳英妹", 
        nick: "家族最強指揮官", 
        title: "家庭長 / Decision Maker", 
        business: "雖然是家族最強指揮官，但很多事還是會問其他主管。", 
        theme: "bg-indigo-500", 
        isPhoto: false, 
        icon: "fa-crown" 
      },
      member2: { 
        name: "呂佳寯", 
        nick: "國防和政戰是我的專業", 
        title: "行政管理 / Operations", 
        business: "雖然是負責單位行政，但主要專長是政戰。", 
        theme: "bg-emerald-500", 
        isPhoto: true, 
        photo: "110417006.jpg" 
      },
      member3: { 
        name: "呂佳芯", 
        nick: "氣氛製造機", 
        title: "分隊長 / Atmosphere", 
        business: "突然就被叫來擔任。", 
        theme: "bg-pink-500", 
        isPhoto: false, 
        icon: "fa-wand-magic-sparkles" 
      }
    };

    function openMemberModal(id) {
      const data = memberData[id];
      const modal = document.getElementById('memberModal');
      const container = document.getElementById('modalContainer');
      const avatarBox = document.getElementById('modalAvatarBox');
      
      document.getElementById('modalTheme').className = `h-32 ${data.theme} opacity-20`;
      document.getElementById('modalName').innerText = data.name;
      document.getElementById('modalNick').innerText = `「 ${data.nick} 」`;
      document.getElementById('modalTitle').innerText = data.title;
      document.getElementById('modalBusiness').innerText = data.business;
      
      avatarBox.innerHTML = data.isPhoto ? `<img src="${data.photo}" class="w-full h-full object-cover">` : `<i class="fa-solid ${data.icon} ${data.theme.replace('bg-', 'text-')}"></i>`;
      
      modal.classList.remove('hidden');
      setTimeout(() => { container.classList.remove('scale-95', 'opacity-0'); container.classList.add('scale-100', 'opacity-100'); }, 10);
    }

    function closeModal() {
      const modal = document.getElementById('memberModal');
      const container = document.getElementById('modalContainer');
      container.classList.add('scale-95', 'opacity-0');
      setTimeout(() => modal.classList.add('hidden'), 300);
    }
  </script>
</body>
</html>
