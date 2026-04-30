
  
  <div class="bg-primary text-primary-foreground text-center py-2 text-sm font-medium">
    🎉 新用户首单立减 ¥50 | 全场满 ¥299 包邮
  </div>

  
  <header class="sticky top-0 z-50 bg-background/95 backdrop-blur border-b border-border">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        
        <div class="flex items-center gap-2">
          <img aria-hidden="true" alt="logo" src="http://localhost:5173/openui/32x32.svg?text=🛍️" class="w-8 h-8">
          <span class="text-xl font-bold bg-gradient-to-r from-primary to-accent bg-clip-text text-transparent">ShopEase</span>
        </div>

        
        <div class="hidden md:flex flex-1 max-w-xl mx-8">
          <div class="relative w-full">
            <input type="text" placeholder="搜索商品、品牌或类别..." class="w-full h-10 pl-10 pr-4 rounded-lg bg-secondary border border-border focus:outline-none focus:ring-2 focus:ring-ring text-foreground placeholder:text-muted-foreground">
            <img aria-hidden="true" alt="search" src="http://localhost:5173/openui/20x20.svg?text=🔍" class="absolute left-3 top-1/2 -translate-y-1/2 w-5 h-5 opacity-50">
          </div>
        </div>

        
        <div class="flex items-center gap-2 sm:gap-4">
          <button class="md:hidden p-2 rounded-lg hover:bg-secondary transition-colors" onclick="toggleSearch()">
            <img aria-hidden="true" alt="search" src="http://localhost:5173/openui/24x24.svg?text=🔍" class="w-6 h-6">
          </button>
          <button class="hidden sm:flex items-center gap-1 p-2 rounded-lg hover:bg-secondary transition-colors">
            <img aria-hidden="true" alt="user" src="http://localhost:5173/openui/24x24.svg?text=👤" class="w-6 h-6">
            <span class="text-sm font-medium">登录</span>
          </button>
          <button class="relative p-2 rounded-lg hover:bg-secondary transition-colors" onclick="toggleCart()">
            <img aria-hidden="true" alt="cart" src="http://localhost:5173/openui/24x24.svg?text=🛒" class="w-6 h-6">
            <span id="cart-badge" class="absolute -top-1 -right-1 w-5 h-5 bg-destructive text-destructive-foreground text-xs rounded-full flex items-center justify-center font-bold">3</span>
          </button>
          <button class="sm:hidden p-2 rounded-lg hover:bg-secondary transition-colors" onclick="toggleMenu()">
            <img aria-hidden="true" alt="menu" src="http://localhost:5173/openui/24x24.svg?text=☰" class="w-6 h-6">
          </button>
        </div>
      </div>

      
      <div id="mobile-search" class="hidden md:hidden pb-4">
        <div class="relative w-full">
          <input type="text" placeholder="搜索商品..." class="w-full h-10 pl-10 pr-4 rounded-lg bg-secondary border border-border focus:outline-none focus:ring-2 focus:ring-ring text-foreground placeholder:text-muted-foreground">
          <img aria-hidden="true" alt="search" src="http://localhost:5173/openui/20x20.svg?text=🔍" class="absolute left-3 top-1/2 -translate-y-1/2 w-5 h-5 opacity-50">
        </div>
      </div>

      
      <nav id="main-nav" class="hidden sm:flex items-center gap-6 py-3 text-sm font-medium text-muted-foreground overflow-x-auto">
        <a href="#" class="text-foreground hover:text-primary whitespace-nowrap">首页</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">新品上市</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">热销商品</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">电子产品</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">服饰鞋包</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">家居生活</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">美妆护肤</a>
        <a href="#" class="hover:text-primary whitespace-nowrap">限时特惠</a>
      </nav>
    </div>
  </header>

  
  <div id="mobile-menu" class="fixed inset-0 z-50 hidden">
    <div class="absolute inset-0 bg-black/50" onclick="toggleMenu()"></div>
    <div class="absolute right-0 top-0 h-full w-72 bg-background border-l border-border p-6 overflow-y-auto">
      <div class="flex justify-between items-center mb-6">
        <span class="text-lg font-bold">菜单</span>
        <button onclick="toggleMenu()" class="p-2 rounded-lg hover:bg-secondary">
          <img aria-hidden="true" alt="close" src="http://localhost:5173/openui/24x24.svg?text=✕" class="w-6 h-6">
        </button>
      </div>
      <nav class="flex flex-col gap-4">
        <a href="#" class="py-2 border-b border-border text-foreground font-medium">首页</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">新品上市</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">热销商品</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">电子产品</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">服饰鞋包</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">家居生活</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">美妆护肤</a>
        <a href="#" class="py-2 border-b border-border hover:text-primary">限时特惠</a>
        <a href="#" class="py-2 text-primary font-medium">登录 / 注册</a>
      </nav>
    </div>
  </div>

  
  <div id="cart-sidebar" class="fixed inset-0 z-50 hidden">
    <div class="absolute inset-0 bg-black/50" onclick="toggleCart()"></div>
    <div class="absolute right-0 top-0 h-full w-full max-w-md bg-background border-l border-border flex flex-col">
      <div class="flex justify-between items-center p-4 border-b border-border">
        <span class="text-lg font-bold">购物车 (3)</span>
        <button onclick="toggleCart()" class="p-2 rounded-lg hover:bg-secondary">
          <img aria-hidden="true" alt="close" src="http://localhost:5173/openui/24x24.svg?text=✕" class="w-6 h-6">
        </button>
      </div>
      <div class="flex-1 overflow-y-auto p-4 space-y-4">
        
        <div class="flex gap-4 p-3 rounded-lg bg-card">
          <img src="https://placehold.co/80x80/e2e8f0/475569?text=耳机" alt="无线蓝牙耳机" class="w-20 h-20 rounded-lg object-cover">
          <div class="flex-1">
            <h4 class="font-medium text-sm">无线蓝牙耳机 Pro</h4>
            <p class="text-muted-foreground text-xs mt-1">黑色 / 标准版</p>
            <div class="flex justify-between items-center mt-2">
              <span class="font-bold text-primary">¥299</span>
              <div class="flex items-center gap-2">
                <button class="w-6 h-6 rounded bg-secondary flex items-center justify-center text-sm">-</button>
                <span class="text-sm w-4 text-center">1</span>
                <button class="w-6 h-6 rounded bg-secondary flex items-center justify-center text-sm">+</button>
              </div>
            </div>
          </div>
        </div>
        
        <div class="flex gap-4 p-3 rounded-lg bg-card">
          <img src="https://placehold.co/80x80/e2e8f0/475569?text=手表" alt="智能手表" class="w-20 h-20 rounded-lg object-cover">
          <div class="flex-1">
            <h4 class="font-medium text-sm">智能手表 Series 5</h4>
            <p class="text-muted-foreground text-xs mt-1">银色 / 42mm</p>
            <div class="flex justify-between items-center mt-2">
              <span class="font-bold text-primary">¥1,299</span>
              <div class="flex items-center gap-2">
                <button class="w-6 h-6 rounded bg-secondary flex items-center justify-center text-sm">-</button>
                <span class="text-sm w-4 text-center">1</span>
                <button class="w-6 h-6 rounded bg-secondary flex items-center justify-center text-sm">+</button>
              </div>
            </div>
          </div>
        </div>
        
        <div class="flex gap-4 p-3 rounded-lg bg-card">
          <img src="https://placehold.co/80x80/e2e8f0/475569?text=背包" alt="双肩背包" class="w-20 h-20 rounded-lg object-cover">
          <div class="flex-1">
            <h4 class="font-medium text-sm">商务双肩背包</h4>
            <p class="text-muted-foreground text-xs mt-1">深灰色 / 15.6寸</p>
            <div class="flex justify-between items-center mt-2">
              <span class="font-bold text-primary">¥199</span>
              <div class="flex items-center gap-2">
                <button class="w-6 h-6 rounded bg-secondary flex items-center justify-center text-sm">-</button>
                <span class="text-sm w-4 text-center">1</span>
                <button class="w-6 h-6 rounded bg-secondary flex items-center justify-center text-sm">+</button>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="border-t border-border p-4 space-y-4">
        <div class="flex justify-between items-center">
          <span class="text-muted-foreground">合计</span>
          <span class="text-2xl font-bold text-primary">¥1,797</span>
        </div>
        <button class="w-full py-3 bg-primary text-primary-foreground rounded-lg font-semibold hover:bg-primary/90 transition-colors">
          去结算
        </button>
      </div>
    </div>
  </div>

  
  <section class="relative overflow-hidden">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 lg:py-12">
      <div class="grid lg:grid-cols-3 gap-4 lg:gap-6">
        
        <div class="lg:col-span-2 relative rounded-2xl overflow-hidden bg-gradient-to-br from-primary/20 via-accent/10 to-background group cursor-pointer">
          <img src="https://placehold.co/800x400/1e293b/94a3b8?text=🎧+新品首发" alt="新品首发" class="w-full h-64 sm:h-80 lg:h-96 object-cover">
          <div class="absolute inset-0 bg-gradient-to-r from-black/60 via-black/30 to-transparent flex flex-col justify-center px-6 sm:px-10">
            <span class="inline-block w-fit px-3 py-1 bg-primary text-primary-foreground text-xs font-bold rounded-full mb-3">限时特惠</span>
            <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-white mb-2">新品首发</h2>
            <p class="text-white/80 text-sm sm:text-base mb-4 max-w-md">探索最新科技产品，享受前所未有的智能体验</p>
            <button class="w-fit px-6 py-2.5 bg-white text-black font-semibold rounded-lg hover:bg-white/90 transition-colors text-sm">
              立即选购 →
            </button>
          </div>
        </div>

        
        <div class="flex flex-col gap-4 lg:gap-6">
          <div class="relative rounded-2xl overflow-hidden bg-gradient-to-br from-secondary to-background group cursor-pointer flex-1">
            <img src="https://placehold.co/400x200/f1f5f9/475569?text=👟+运动季" alt="运动季" class="w-full h-32 sm:h-40 object-cover">
            <div class="absolute inset-0 bg-gradient-to-r from-black/50 to-transparent flex flex-col justify-center px-5">
              <h3 class="text-lg sm:text-xl font-bold text-white">运动季</h3>
              <p class="text-white/70 text-xs sm:text-sm">低至 5 折</p>
            </div>
          </div>
          <div class="relative rounded-2xl overflow-hidden bg-gradient-to-br from-accent/20 to-background group cursor-pointer flex-1">
            <img src="https://placehold.co/400x200/fef3c7/92400e?text=🏠+家居焕新" alt="家居焕新" class="w-full h-32 sm:h-40 object-cover">
            <div class="absolute inset-0 bg-gradient-to-r from-black/50 to-transparent flex flex-col justify-center px-5">
              <h3 class="text-lg sm:text-xl font-bold text-white">家居焕新</h3>
              <p class="text-white/70 text-xs sm:text-sm">满 ¥500 减 ¥100</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  
  <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
    <div class="grid grid-cols-4 sm:grid-cols-6 md:grid-cols-8 lg:grid-cols-10 gap-3 sm:gap-4">
      <a href="#" class="flex flex-col items-center gap-2 group">
        <div class="w-14 h-14 sm:w-16 sm:h-16 rounded-xl bg-secondary flex items-center justify-center group-hover:bg-primary/10 transition-colors">
          <img aria-hidden="true" alt="手机" src="http://localhost:5173/openui/32x32.svg?text=📱" class="w-8 h-8">
        </div>
        <span class="text-xs text-muted-foreground group-hover:text-foreground transition-colors">手机</span>
      </a>
      <a href="#" class="flex flex-col items-center gap-2 group">
        <div class="w-14 h-14 sm:w-16 sm:h-16 rounded-xl bg-secondary flex items-center justify-center group-hover:bg-primary/10 transition-colors">
          <img aria-hidden="true" alt="电脑" src="http://localhost:5173/openui/32x32.svg?text=💻" class="w-8 h-8">
        </div>
        <span class="text-xs text-muted-foreground group-hover:text-foreground transition-colors">电脑</span>
      </a>
      <a href="#" class="flex flex-col items-center gap-2 group">
        <div class="w-14 h-14 sm:w-16 sm:h-16 rounded-xl bg-secondary flex items-center justify-center group-hover:bg-primary/10 transition-colors">
          <img aria-hidden="true" alt="耳机" src="http://localhost:5173/openui/32x32.svg?text=🎧" class="w-8 h-8">
        </div>
        <span class="text-xs text-muted-foreground group-hover:text-foreground transition-colors">耳机</span>
      </a>
      <a href="#" class="flex flex-col items-center gap-2 group">
        </a></div></section>