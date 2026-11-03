# Commercial-Website
Modern Web
AIM
To design and develop a commercial website using HTML and CSS to promote business products/services, showcase company information, display product details, provide customer support, and enable online interaction with customers.
ALGORITHM
1. Start the program.
2. Open Visual Studio Code and create a project folder for the commercial website.
3. Create necessary files such as:
   - index.html for webpage structure.
   - style.css for webpage design and styling.
   - Images folder to store product and company images.
4. Write the HTML code to design the commercial website layout.
5. Create important sections of the website such as:
   - Home page.
   - About Us section.
   - Products/Services section.
   - Pricing details.
   - Customer reviews.
   - Contact information.
   - Footer section.
6. Add company logo, product images, business information, and service descriptions.
7. Apply CSS styling to improve website appearance, including:
   - Colors.
   - Fonts.
   - Navigation bar.
   - Buttons.
   - Responsive design.
8. Save all HTML and CSS files.
9. Test the website by opening the index.html file in a web browser.
10. Create a GitHub account and log in.
11. Create a new repository named commercial-website.
12. Upload all website files including HTML, CSS, and image files to the repository.
13. Open repository settings and select GitHub Pages.
14. Choose the main branch and / (root) folder as the deployment source.
15. Click Save to publish the commercial website.
16. Open the generated GitHub Pages URL to view the live website.
17. Stop the program.


#HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Nilgiri Leaf | Fresh Hill-Grown Tea</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- HEADER + NAVIGATION -->
  <header class="site-header">
    <a href="#home" class="logo">Nilgiri Leaf</a>
    <nav class="navbar">
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#products">Products</a></li>
        <li><a href="#about">About Us</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a href="#account" class="nav-cta">My Account</a></li>
        <li><button type="button" id="cart-btn" class="icon-btn" aria-label="Cart">Cart <span id="cart-count" class="badge">0</span></button></li>
        <li><button type="button" id="theme-btn" class="icon-btn" aria-label="Toggle dark mode">Dark</button></li>
      </ul>
    </nav>
  </header>

  <main>
    <!-- HOME -->
    <section id="home" class="hero">
      <div class="hero-text">
        <h1>Tea picked on the hills, packed within 48 hours.</h1>
        <p>Single-estate teas from the Nilgiris, shipped fresh to your door across India.</p>
        <a href="#products" class="btn">Shop teas</a>
      </div>
      <div class="hero-img">
        <img src="https://picsum.photos/seed/teagarden/700/480" alt="Tea garden on a hillside">
      </div>
    </section>

    <!-- PRODUCTS -->
    <section id="products" class="section">
      <h2>Our Products</h2>
      <div class="cards">
        <article class="card">
          <img src="https://picsum.photos/seed/blacktea/400/260" alt="Black tea">
          <div class="card-body">
            <h3>Estate Black Tea</h3>
            <p>Bold and malty. Good with or without milk.</p>
            <span class="price">₹250 / 250 g</span>
            <button type="button" class="btn small add-btn">Add to cart</button>
          </div>
        </article>
        <article class="card">
          <img src="https://picsum.photos/seed/greentea/400/260" alt="Green tea">
          <div class="card-body">
            <h3>Mountain Green Tea</h3>
            <p>Light, grassy and gentle on an empty stomach.</p>
            <span class="price">₹320 / 100 g</span>
            <button type="button" class="btn small add-btn">Add to cart</button>
          </div>
        </article>
        <article class="card">
          <img src="https://picsum.photos/seed/masalatea/400/260" alt="Masala chai blend">
          <div class="card-body">
            <h3>Masala Chai Blend</h3>
            <p>Black tea with cardamom, ginger and clove.</p>
            <span class="price">₹280 / 250 g</span>
            <button type="button" class="btn small add-btn">Add to cart</button>
          </div>
        </article>
        <article class="card">
          <img src="https://picsum.photos/seed/giftbox/400/260" alt="Tea gift box">
          <div class="card-body">
            <h3>Tasting Gift Box</h3>
            <p>Four small tins, one for each of our best sellers.</p>
            <span class="price">₹799</span>
            <button type="button" class="btn small add-btn">Add to cart</button>
          </div>
        </article>
      </div>
    </section>

    <!-- STEEP TIMER (unique feature) -->
    <section id="steep" class="section steep">
      <div class="steep-intro">
        <h2>Steep Timer</h2>
        <p>Pick your tea and we count down the perfect brew time and tell you the water temperature to use.</p>
      </div>
      <div class="steep-box">
        <div class="tea-options">
          <button type="button" class="tea-opt active" data-name="Black Tea" data-sec="240" data-temp="95">Black</button>
          <button type="button" class="tea-opt" data-name="Green Tea" data-sec="120" data-temp="80">Green</button>
          <button type="button" class="tea-opt" data-name="Masala Chai" data-sec="300" data-temp="100">Chai</button>
        </div>
        <div class="timer-display" id="timer-display">04:00</div>
        <p id="timer-info">Black Tea: water at 95&deg;C</p>
        <div class="progress"><div id="progress-bar"></div></div>
        <div class="timer-actions">
          <button type="button" class="btn" id="timer-start">Start brewing</button>
          <button type="button" class="btn outline" id="timer-reset">Reset</button>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" class="section about">
      <div class="about-img">
        <img src="https://picsum.photos/seed/teapickers/600/400" alt="Tea pickers at work">
      </div>
      <div class="about-text">
        <h2>About Us</h2>
        <p>We began in 2015 with one small estate and a simple rule: buy directly from growers and pay them fairly.</p>
        <p>Today we work with 12 family farms. Every pack lists the estate, the pick date and the grower.</p>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="section contact">
      <div class="contact-info">
        <h2>Contact Details</h2>
        <p><strong>Address:</strong> 12, Market Road, Coonoor, Tamil Nadu 643101</p>
        <p><strong>Phone:</strong> +91 98765 43210</p>
        <p><strong>Email:</strong> hello@nilgirileaf.example</p>
        <p><strong>Hours:</strong> Mon to Sat, 9 am to 6 pm</p>
      </div>
      <form class="contact-form">
        <label for="msg-name">Your name</label>
        <input type="text" id="msg-name" placeholder="Full name">
        <label for="msg-text">Message</label>
        <textarea id="msg-text" rows="4" placeholder="What would you like to order or ask?"></textarea>
        <button type="button" class="btn">Send message</button>
      </form>
    </section>

    <!-- USER ACCOUNT -->
    <section id="account" class="section account">
      <h2>User Account</h2>
      <div class="account-box">
        <form class="login-form">
          <label for="email">Email</label>
          <input type="email" id="email" placeholder="you@example.com">
          <label for="password">Password</label>
          <input type="password" id="password" placeholder="Password">
          <button type="button" class="btn">Log in</button>
        </form>
        <div class="account-links">
          <h3>New here?</h3>
          <p>Create an account to track orders and save your favourite teas.</p>
          <a href="#account" class="btn outline">Create account</a>
        </div>
      </div>
    </section>
  </main>

  <!-- FOOTER -->
  <footer class="site-footer">
    <div class="footer-top">
      <div class="footer-col">
        <h3>Nilgiri Leaf</h3>
        <p>Fresh hill-grown tea, straight from the estate.</p>
      </div>
      <div class="footer-col">
        <h3>Quick links</h3>
        <a href="#products">Products</a>
        <a href="#about">About Us</a>
        <a href="#steep">Steep Timer</a>
        <a href="#contact">Contact</a>
      </div>
      <div class="footer-col">
        <h3>Follow us</h3>
        <div class="social">
          <a href="https://facebook.com" target="_blank" rel="noopener">Facebook</a>
          <a href="https://instagram.com" target="_blank" rel="noopener">Instagram</a>
          <a href="https://x.com" target="_blank" rel="noopener">X</a>
          <a href="https://youtube.com" target="_blank" rel="noopener">YouTube</a>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2026 Nilgiri Leaf. All rights reserved.</p>
      <p>Name: YOUR NAME &nbsp;|&nbsp; Register Number: YOUR REGISTER NUMBER</p>
    </div>
  </footer>

  <div id="toast" class="toast" role="status" aria-live="polite"></div>
  <script src="script.js"></script>
</body>
</html>
```

#CSS
```
/* ---------- GLOBAL STYLES ---------- */
:root {
  --green: #17402f;
  --mint: #e3f0e6;
  --saffron: #f2a93b;
  --ink: #222a26;
  --white: #ffffff;
}

* { margin: 0; padding: 0; box-sizing: border-box; }

html { scroll-behavior: smooth; }

body {
  font-family: "Inter", "Segoe UI", Arial, sans-serif;
  color: var(--ink);
  line-height: 1.6;
  background: var(--white);
}

h1, h2, h3 { font-family: "Fraunces", Georgia, serif; line-height: 1.2; }
h2 { font-size: 2rem; margin-bottom: 1.5rem; color: var(--green); }
img { max-width: 100%; display: block; }
a { color: inherit; text-decoration: none; }

/* ---------- BUTTONS ---------- */
.btn {
  display: inline-block;
  background: var(--saffron);
  color: var(--ink);
  font-weight: 600;
  padding: 0.7rem 1.4rem;
  border: 2px solid var(--saffron);
  border-radius: 6px;
  cursor: pointer;
  font-size: 1rem;
  transition: background 0.3s, transform 0.2s;
}
.btn:hover { background: #e19621; transform: translateY(-2px); }
.btn.small { padding: 0.4rem 1rem; font-size: 0.9rem; }
.btn.outline { background: transparent; border-color: var(--green); color: var(--green); }
.btn.outline:hover { background: var(--green); color: var(--white); }

/* ---------- HEADER / NAVBAR (Flexbox) ---------- */
.site-header {
  display: flex;
  justify-content: space-between;   /* logo left, nav right */
  align-items: center;
  flex-wrap: wrap;
  gap: 1rem;
  padding: 1rem 5%;
  background: var(--green);
  color: var(--white);
  position: sticky;
  top: 0;
  z-index: 10;
}
.logo { font-family: "Fraunces", Georgia, serif; font-size: 1.6rem; font-weight: 700; }

.nav-links {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5rem;
  list-style: none;
  align-items: center;
}
.nav-links a { padding: 0.3rem 0; border-bottom: 2px solid transparent; transition: border-color 0.3s; }
.nav-links a:hover { border-color: var(--saffron); }
.nav-links .nav-cta {
  background: var(--saffron);
  color: var(--ink);
  padding: 0.4rem 1rem;
  border-radius: 6px;
  border: none;
  font-weight: 600;
}

/* ---------- SECTIONS ---------- */
.section { padding: 4rem 5%; }

/* ---------- HERO ---------- */
.hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 3rem;
  padding: 4rem 5%;
  background: var(--mint);
}
.hero-text { flex: 1 1 340px; }
.hero-text h1 { font-size: 2.8rem; color: var(--green); margin-bottom: 1rem; }
.hero-text p { font-size: 1.15rem; margin-bottom: 1.5rem; max-width: 46ch; }
.hero-img { flex: 1 1 340px; }
.hero-img img { border-radius: 12px; width: 100%; }

/* ---------- PRODUCT CARDS ---------- */
.cards {
  display: flex;
  flex-wrap: wrap;                  /* cards wrap onto new rows */
  gap: 1.5rem;
}
.card {
  flex: 1 1 240px;                  /* grow, shrink, min width 240px */
  display: flex;
  flex-direction: column;
  border: 1px solid #d5e2d8;
  border-radius: 10px;
  overflow: hidden;
  background: var(--white);
  transition: transform 0.3s, box-shadow 0.3s;
}
.card:hover { transform: translateY(-6px); box-shadow: 0 10px 24px rgba(23, 64, 47, 0.18); }
.card img { width: 100%; height: 180px; object-fit: cover; }
.card-body {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  padding: 1rem;
  flex: 1;
}
.card-body h3 { color: var(--green); font-size: 1.2rem; }
.card-body p { flex: 1; }          /* pushes price and button to the bottom */
.price { font-weight: 700; }
.card-body .btn { align-self: flex-start; }

/* ---------- ABOUT ---------- */
.about {
  display: flex;
  align-items: center;
  gap: 3rem;
  background: var(--mint);
}
.about-img { flex: 1 1 320px; }
.about-img img { border-radius: 12px; width: 100%; }
.about-text { flex: 1 1 320px; }
.about-text p { margin-bottom: 1rem; max-width: 55ch; }

/* ---------- CONTACT ---------- */
.contact { display: flex; flex-wrap: wrap; gap: 3rem; }
.contact-info, .contact-form { flex: 1 1 320px; }
.contact-info p { margin-bottom: 0.8rem; }

/* ---------- FORMS ---------- */
form { display: flex; flex-direction: column; gap: 0.6rem; }
label { font-weight: 600; }
input, textarea {
  padding: 0.7rem;
  border: 1px solid #b9c9bd;
  border-radius: 6px;
  font: inherit;
}
input:focus, textarea:focus, .btn:focus-visible, a:focus-visible {
  outline: 3px solid var(--saffron);
  outline-offset: 2px;
}
form .btn { align-self: flex-start; margin-top: 0.5rem; }

/* ---------- ACCOUNT ---------- */
.account { background: var(--mint); }
.account-box {
  display: flex;
  flex-wrap: wrap;
  gap: 2rem;
}
.login-form, .account-links {
  flex: 1 1 300px;
  background: var(--white);
  padding: 1.5rem;
  border-radius: 10px;
}
.account-links { display: flex; flex-direction: column; gap: 0.8rem; align-items: flex-start; }

/* ---------- FOOTER ---------- */
.site-footer { background: var(--green); color: var(--white); padding: 3rem 5% 1.5rem; }
.footer-top {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 2rem;
  padding-bottom: 2rem;
}
.footer-col { flex: 1 1 200px; display: flex; flex-direction: column; gap: 0.5rem; }
.footer-col h3 { margin-bottom: 0.4rem; }
.footer-col a { transition: color 0.3s; }
.footer-col a:hover { color: var(--saffron); }
.social { display: flex; flex-wrap: wrap; gap: 1rem; }
.footer-bottom {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 0.5rem;
  border-top: 1px solid rgba(255, 255, 255, 0.25);
  padding-top: 1rem;
  font-size: 0.9rem;
}

/* ---------- RESPONSIVE ---------- */
@media (max-width: 768px) {
  .site-header { flex-direction: column; }
  .nav-links { justify-content: center; gap: 1rem; }
  .hero, .about { flex-direction: column; }
  .hero-text h1 { font-size: 2.1rem; }
  .footer-bottom { flex-direction: column; text-align: center; }
}

@media (prefers-reduced-motion: reduce) {
  * { transition: none !important; scroll-behavior: auto !important; }
}

/* ---------- UNIQUE FEATURES: cart, dark mode, steep timer ---------- */
.icon-btn {
  display: flex; align-items: center; gap: 0.4rem;
  background: transparent; color: var(--white);
  border: 1px solid rgba(255,255,255,0.5); border-radius: 6px;
  padding: 0.35rem 0.8rem; font: inherit; cursor: pointer;
  transition: background 0.3s;
}
.icon-btn:hover { background: rgba(255,255,255,0.15); }
.badge {
  display: inline-flex; justify-content: center; align-items: center;
  min-width: 1.4rem; height: 1.4rem; border-radius: 999px;
  background: var(--saffron); color: var(--ink); font-size: 0.8rem; font-weight: 700;
}
.badge.bump { animation: bump 0.3s; }
@keyframes bump { 50% { transform: scale(1.4); } }

.toast {
  position: fixed; bottom: 1.5rem; left: 50%;
  transform: translate(-50%, 200%);
  background: var(--ink); color: var(--white);
  padding: 0.7rem 1.2rem; border-radius: 8px;
  transition: transform 0.3s; z-index: 20;
}
.toast.show { transform: translate(-50%, 0); }

.steep { display: flex; flex-wrap: wrap; align-items: center; gap: 3rem; }
.steep-intro { flex: 1 1 280px; }
.steep-intro p { max-width: 45ch; }
.steep-box {
  flex: 1 1 320px; display: flex; flex-direction: column; align-items: center; gap: 1rem;
  background: var(--mint); padding: 2rem; border-radius: 14px;
}
.tea-options { display: flex; flex-wrap: wrap; gap: 0.6rem; justify-content: center; }
.tea-opt {
  padding: 0.5rem 1.2rem; border-radius: 999px; border: 2px solid var(--green);
  background: transparent; color: var(--green); font: inherit; font-weight: 600; cursor: pointer;
  transition: background 0.3s, color 0.3s;
}
.tea-opt.active, .tea-opt:hover { background: var(--green); color: var(--white); }
.timer-display { font-family: "Fraunces", Georgia, serif; font-size: 4rem; font-weight: 700; color: var(--green); }
.progress { width: 100%; height: 10px; background: #fff; border-radius: 999px; overflow: hidden; }
#progress-bar { height: 100%; width: 0; background: var(--saffron); transition: width 1s linear; }
.timer-actions { display: flex; gap: 0.8rem; flex-wrap: wrap; justify-content: center; }
.steep-box.done .timer-display { color: #c0392b; }

/* Dark mode: only the variables change */
body.dark {
  --green: #9fd3b5; --mint: #1c2a24; --ink: #e8efe9; --white: #121915;
}
body.dark .site-header, body.dark .site-footer { background: #0b120e; color: #e8efe9; }
body.dark .nav-links .nav-cta, body.dark .btn { color: #1b1b1b; }
body.dark .btn.outline { color: var(--green); }
body.dark .btn.outline:hover { color: #121915; }
body.dark .card { border-color: #2c3d34; }
body.dark input, body.dark textarea { background: #1c2a24; color: var(--ink); border-color: #2c3d34; }
body.dark .progress { background: #121915; }
body.dark .tea-opt.active, body.dark .tea-opt:hover { color: #121915; }
```

#Javascript.
```
/* ---------- Dark mode ---------- */
const body = document.body;
const themeBtn = document.getElementById("theme-btn");
try { if (localStorage.getItem("theme") === "dark") body.classList.add("dark"); } catch (e) {}
const syncThemeLabel = () => themeBtn.textContent = body.classList.contains("dark") ? "Light" : "Dark";
syncThemeLabel();
themeBtn.addEventListener("click", () => {
  body.classList.toggle("dark");
  try { localStorage.setItem("theme", body.classList.contains("dark") ? "dark" : "light"); } catch (e) {}
  syncThemeLabel();
});

/* ---------- Add to cart ---------- */
const countEl = document.getElementById("cart-count");
const toast = document.getElementById("toast");
let cart = 0, toastTimer;

function showToast(msg) {
  toast.textContent = msg;
  toast.classList.add("show");
  clearTimeout(toastTimer);
  toastTimer = setTimeout(() => toast.classList.remove("show"), 1800);
}

document.querySelectorAll(".add-btn").forEach(btn => {
  btn.addEventListener("click", () => {
    cart++;
    countEl.textContent = cart;
    countEl.classList.remove("bump");
    void countEl.offsetWidth;            // restart animation
    countEl.classList.add("bump");
    const name = btn.closest(".card").querySelector("h3").textContent;
    showToast(name + " added to cart");
  });
});

/* ---------- Steep timer ---------- */
const display = document.getElementById("timer-display");
const info = document.getElementById("timer-info");
const bar = document.getElementById("progress-bar");
const box = document.querySelector(".steep-box");
const startBtn = document.getElementById("timer-start");
let total = 240, left = 240, tea = "Black Tea", temp = 95, interval = null;

const fmt = s => String(Math.floor(s / 60)).padStart(2, "0") + ":" + String(s % 60).padStart(2, "0");
function render() {
  display.textContent = fmt(left);
  bar.style.width = ((total - left) / total * 100) + "%";
}
function stop() { clearInterval(interval); interval = null; startBtn.textContent = "Start brewing"; }
function reset() {
  stop(); left = total; box.classList.remove("done");
  info.innerHTML = tea + ": water at " + temp + "&deg;C"; render();
}

document.querySelectorAll(".tea-opt").forEach(opt => {
  opt.addEventListener("click", () => {
    document.querySelectorAll(".tea-opt").forEach(o => o.classList.remove("active"));
    opt.classList.add("active");
    tea = opt.dataset.name; total = +opt.dataset.sec; temp = +opt.dataset.temp;
    reset();
  });
});

startBtn.addEventListener("click", () => {
  if (interval) { stop(); return; }                // pause
  if (left === 0) reset();
  startBtn.textContent = "Pause";
  interval = setInterval(() => {
    left--; render();
    if (left <= 0) {
      stop(); box.classList.add("done");
      info.textContent = "Your " + tea + " is ready. Enjoy!";
      showToast("Your " + tea + " is ready");
    }
  }, 1000);
});
document.getElementById("timer-reset").addEventListener("click", reset);
render();
```

#Output.
<img width="1867" height="756" alt="Screenshot 2026-11-03 102359" src="https://github.com/user-attachments/assets/40c9600d-0533-4780-8a8c-0186fdd8c878" />
<img width="1817" height="847" alt="Screenshot 2026-11-03 102417" src="https://github.com/user-attachments/assets/2f179eb9-2986-489e-a22d-cd3945e1a084" />
<img width="1818" height="667" alt="Screenshot 2026-11-03 102429" src="https://github.com/user-attachments/assets/d7a9cce7-cb8d-4da6-8c06-36feee453664" />
<img width="1802" height="817" alt="Screenshot 2026-11-03 102438" src="https://github.com/user-attachments/assets/2d07fda0-eacb-4555-ada4-7b5731e005a1" />
<img width="1790" height="287" alt="image" src="https://github.com/user-attachments/assets/6595fe4e-ae2b-4a78-9373-2592339c1e46" />
