‎<!DOCTYPE html>
‎<html lang="en">
‎<head>
‎<meta charset="UTF-8">
‎<meta name="viewport" content="width=device-width, initial-scale=1">
‎<meta name="description" content="Shop everyday finds at AWS Developer Store. Browse products and add items to your cart.">
‎<title>AWS Developer Store</title>
‎<style>
‎:root{--green:#176b45;--green2:#104b31;--gold:#f1c75b;--ink:#17231d;--muted:#66736b;--paper:#fffdf8;--line:#e5e9e1;--shadow:0 14px 35px rgba(24,48,34,.1)}
‎*{box-sizing:border-box}html{scroll-behavior:smooth;scroll-padding-top:85px}body{margin:0;background:var(--paper);color:var(--ink);font-family:system-ui,-apple-system,"Segoe UI",sans-serif;line-height:1.6}a{color:inherit;text-decoration:none}button,input{font:inherit}button{cursor:pointer}.container{width:min(1120px,calc(100% - 34px));margin:auto}
‎header{position:sticky;top:0;z-index:30;background:rgba(255,253,248,.94);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}.nav{min-height:74px;display:flex;align-items:center;justify-content:space-between;gap:18px}.brand{display:flex;align-items:center;gap:10px;font-weight:850;letter-spacing:-.04em;font-size:1.08rem}.brand-icon{display:grid;place-items:center;background:var(--green);color:white;border-radius:14px;width:42px;height:42px;font-size:1.25rem}.brand small{display:block;color:var(--muted);font-size:.68rem;letter-spacing:.1em;text-transform:uppercase}.nav-links{display:flex;align-items:center;gap:24px;font-weight:650;font-size:.92rem}.nav-links a:hover{color:var(--green)}.btn{border:0;border-radius:999px;padding:12px 19px;background:var(--green);color:white;font-weight:800;display:inline-flex;align-items:center;justify-content:center;gap:8px;transition:.2s}.btn:hover{background:var(--green2);transform:translateY(-2px)}.btn-gold{background:var(--gold);color:#243025}.btn-gold:hover{background:#ffdb75}.menu-toggle{display:none;border:1px solid var(--line);background:white;border-radius:12px;padding:9px 12px}
‎.cart-open{position:relative}.cart-count{display:inline-grid;place-items:center;background:var(--gold);color:#1e2a20;border-radius:50%;min-width:22px;height:22px;padding:0 5px;font-size:.75rem;margin-left:3px}
‎.hero{min-height:555px;display:flex;align-items:center;position:relative;background:#20392d url("https://i.ibb.co/0Vcnn4zy/images.jpg") center/cover no-repeat;color:white}.hero:before{content:"";position:absolute;inset:0;background:linear-gradient(90deg,rgba(8,27,17,.84),rgba(8,27,17,.5) 55%,rgba(8,27,17,.08))}.hero-content{position:relative;padding:78px 0;max-width:690px}.eyebrow{color:#f7d978;text-transform:uppercase;letter-spacing:.15em;font-size:.75rem;font-weight:850}.eyebrow:before{content:"";display:inline-block;width:24px;height:2px;background:currentColor;vertical-align:middle;margin-right:9px}h1{font-size:clamp(2.8rem,7vw,5.4rem);line-height:1.01;letter-spacing:-.06em;margin:19px 0}.hero p{max-width:520px;color:#f0f3ee;font-size:1.08rem;margin:0 0 28px}.hero-actions{display:flex;gap:12px;flex-wrap:wrap}.btn-outline{background:rgba(255,255,255,.1);border:1px solid rgba(255,255,255,.5)}.btn-outline:hover{background:rgba(255,255,255,.2)}
‎.highlights{background:#f3f3eb;border-bottom:1px solid var(--line)}.highlight-row{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;padding:18px 0}.highlight{text-align:center;font-size:.9rem;font-weight:750;color:#405247}.highlight span{color:var(--green);margin-right:7px}
‎section.section{padding:78px 0}.section-head{display:flex;justify-content:space-between;align-items:end;gap:18px;margin-bottom:27px}.kicker{color:var(--green);text-transform:uppercase;letter-spacing:.15em;font-size:.75rem;font-weight:850}h2{font-size:clamp(2rem,4vw,3.1rem);line-height:1.1;letter-spacing:-.05em;margin:8px 0}.muted{color:var(--muted);max-width:550px;margin:10px 0 0}.controls{display:flex;gap:8px}.circle{width:43px;height:43px;border:1px solid var(--line);border-radius:50%;background:white;font-size:1.1rem}.circle:hover{background:var(--green);color:white}
‎.carousel{display:grid;grid-auto-flow:column;grid-auto-columns:minmax(245px,1fr);gap:18px;overflow-x:auto;scroll-snap-type:x mandatory;scroll-behavior:smooth;padding:4px 2px 18px;scrollbar-color:#cbd6ca transparent}.card{background:white;border:1px solid var(--line);border-radius:21px;overflow:hidden;scroll-snap-align:start;box-shadow:0 5px 18px rgba(24,48,34,.035);transition:transform .2s,box-shadow .2s}.card:hover{transform:translateY(-4px);box-shadow:var(--shadow)}.image-wrap{height:220px;background:#f0f1e9;overflow:hidden}.product-image{width:100%;height:100%;object-fit:cover;display:block;transition:transform .3s}.card:hover .product-image{transform:scale(1.04)}.fallback{display:none;height:100%;place-items:center;text-align:center;color:var(--muted);padding:20px}.card-body{padding:18px}.tag{display:inline-block;padding:4px 10px;border-radius:99px;background:#eaf3e9;color:var(--green);font-size:.7rem;font-weight:850;margin-bottom:8px}.card h3{font-size:1.08rem;margin:0 0 5px}.card p{font-size:.88rem;color:var(--muted);margin:0 0 15px;min-height:44px}.card-bottom{display:flex;align-items:center;justify-content:space-between;gap:8px}.price{font-weight:850}.add-btn{border:0;background:var(--green);color:white;border-radius:999px;padding:10px 13px;font-size:.8rem;font-weight:800;white-space:nowrap}.add-btn:hover{background:var(--green2)}.catalog{background:#f4f5ee}.search{width:min(480px,100%);padding:14px 16px;border:1px solid #dfe5db;border-radius:14px;background:white;outline:none;margin:23px 0}.search:focus{border-color:var(--green);box-shadow:0 0 0 3px #176b4518}.grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}.empty{grid-column:1/-1;text-align:center;color:var(--muted);padding:30px}
‎.about-grid,.contact-grid{display:grid;grid-template-columns:1fr 1fr;align-items:center;gap:48px}.about-photo{min-height:330px;border-radius:25px;overflow:hidden;background:#e1e9dc}.about-photo img{display:block;width:100%;height:100%;min-height:330px;object-fit:cover}.about-copy p{color:var(--muted)}.points{display:grid;gap:10px;margin:22px 0}.points div:before{content:"✓";color:var(--green);font-weight:900;margin-right:10px}
‎.contact{background:#153d2b;color:white}.contact .kicker{color:#f1d16d}.contact .muted{color:#d3dfd5}.contact-card{padding:24px;border:1px solid #ffffff2a;border-radius:22px;background:#ffffff0b}.contact-line{display:flex;gap:12px;padding:13px 0;border-bottom:1px solid #ffffff20;overflow-wrap:anywhere}.contact-line:last-child{border:0}.contact-line small{display:block;color:#c2d0c5;font-size:.76rem}.contact-line a,.contact-line span{font-weight:700}.contact-icon{width:38px;height:38px;border-radius:12px;background:#ffffff18;display:grid;place-items:center;flex-shrink:0}
‎footer{background:#0e2c1e;color:#c6d2c8;padding:24px 0;font-size:.88rem}.footer-row{display:flex;justify-content:space-between;gap:14px;flex-wrap:wrap}.footer-row strong{color:white}
‎.whatsapp{position:fixed;right:19px;bottom:19px;z-index:40;display:flex;align-items:center;gap:8px;border-radius:999px;background:#20b966;color:white;padding:14px 18px;font-weight:850;box-shadow:0 10px 28px #12683a4d}.whatsapp:hover{background:#159c53}
‎.cart-panel{position:fixed;inset:0;z-index:80;display:none}.cart-panel.open{display:block}.cart-backdrop{position:absolute;inset:0;background:#101a13a6}.cart-drawer{position:absolute;right:0;top:0;height:100%;width:min(440px,100%);background:var(--paper);padding:22px;overflow:auto;box-shadow:-15px 0 40px #0002}.cart-head{display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--line);padding-bottom:15px}.cart-head h2{font-size:1.7rem;margin:0}.close-cart{border:1px solid var(--line);background:white;border-radius:50%;width:40px;height:40px;font-size:1.2rem}.cart-list{display:grid;gap:14px;margin:20px 0}.cart-item{display:grid;grid-template-columns:66px 1fr auto;gap:12px;align-items:center;border-bottom:1px solid var(--line);padding-bottom:14px}.cart-item img{width:66px;height:66px;object-fit:cover;border-radius:12px;background:#eee}.cart-item strong{display:block;font-size:.92rem}.cart-item small{color:var(--muted)}.qty{display:flex;align-items:center;gap:8px;margin-top:6px}.qty button{width:27px;height:27px;border:1px solid var(--line);border-radius:50%;background:white}.remove{border:0;background:none;color:#a33;font-size:.8rem;padding:5px}.cart-total{border-top:1px solid var(--line);padding-top:17px;display:flex;justify-content:space-between;font-weight:850}.cart-note{font-size:.82rem;color:var(--muted)}.checkout{width:100%;margin-top:13px}.toast{position:fixed;left:50%;bottom:24px;transform:translate(-50%,20px);background:#17231d;color:white;padding:11px 18px;border-radius:999px;z-index:100;opacity:0;pointer-events:none;transition:.25s;font-size:.9rem}.toast.show{opacity:1;transform:translate(-50%,0)}
‎@media(max-width:850px){.nav-links{gap:14px}.nav-cta{display:none}.grid{grid-template-columns:repeat(2,minmax(0,1fr))}.about-grid,.contact-grid{gap:28px}}
‎@media(max-width:640px){.container{width:calc(100% - 28px)}.nav{min-height:68px}.menu-toggle{display:block}.nav-links{display:none;position:absolute;left:14px;right:14px;top:70px;padding:8px;background:white;border:1px solid var(--line);border-radius:15px;box-shadow:var(--shadow);flex-direction:column;align-items:stretch;gap:0}.nav-links.open{display:flex}.nav-links a{padding:12px;border-radius:9px}.hero{min-height:500px;background-position:center}.hero-content{padding:62px 0}.hero-actions .btn{width:100%}.highlight-row{grid-template-columns:1fr;gap:10px}.highlight{text-align:left}.section{padding:58px 0!important}.section-head{align-items:flex-start}.carousel{grid-auto-columns:minmax(78%,1fr);gap:14px}.grid{grid-template-columns:1fr}.image-wrap{height:245px}.about-grid,.contact-grid{grid-template-columns:1fr}.about-photo,.about-photo img{min-height:250px}.whatsapp{width:54px;height:54px;padding:0;justify-content:center;right:14px;bottom:14px}.whatsapp .wa-text{display:none}.footer-row{padding-right:48px}}
‎@media(prefers-reduced-motion:reduce){*,*:before,*:after{scroll-behavior:auto!important;transition-duration:.01ms!important}}
‎
‎.checkout-form{display:grid;gap:12px;margin:18px 0}.checkout-form label{display:grid;gap:5px;font-size:.86rem;font-weight:750;color:var(--ink)}.checkout-form input,.checkout-form textarea,.checkout-form select{width:100%;padding:12px 13px;border:1px solid var(--line);border-radius:12px;background:white;color:var(--ink);outline:none}.checkout-form input:focus,.checkout-form textarea:focus,.checkout-form select:focus{border-color:var(--green);box-shadow:0 0 0 3px #176b4518}.checkout-form textarea{resize:vertical;min-height:78px}.form-row{display:grid;grid-template-columns:1fr 1fr;gap:10px}.required-note{font-size:.78rem;color:var(--muted);margin:0}.order-confirmation{display:none;border:1px solid #b9d9c1;background:#eef8ef;border-radius:16px;padding:16px;margin:16px 0;color:#194a2c}.order-confirmation.show{display:block}.order-confirmation h3{margin:0 0 7px}.order-confirmation .order-id{font-size:1.15rem;font-weight:900;overflow-wrap:anywhere}.order-summary{font-size:.88rem;white-space:pre-line;margin-top:10px}.secondary-btn{border:1px solid var(--line);background:white;color:var(--ink);border-radius:999px;padding:10px 14px;font-weight:750}.admin-note{background:#fff8df;border:1px solid #efdc9a;border-radius:12px;padding:12px;font-size:.82rem;color:#5f4b17;margin:12px 0}
‎@media(max-width:460px){.form-row{grid-template-columns:1fr}}
‎
‎</style>
‎</head>
‎<body>
‎<header>
‎  <div class="container nav">
‎    <a class="brand" href="#home"><span class="brand-icon">✦</span><span>AWS Developer Store<small>Everyday essentials</small></span></a>
‎    <nav class="nav-links" id="navLinks" aria-label="Main navigation">
‎      <a href="#home">Home</a><a href="#products">Products</a><a href="#about">About</a><a href="#contact">Contact</a>
‎    </nav>
‎    <div style="display:flex;gap:9px;align-items:center">
‎      <button class="btn nav-cta cart-open" id="openCartTop">Cart <span class="cart-count" id="cartCountTop">0</span></button>
‎      <button class="menu-toggle" id="menuToggle" aria-label="Toggle menu" aria-expanded="false">☰</button>
‎    </div>
‎  </div>
‎</header>
‎
‎<main>
‎<section class="hero" id="home">
‎  <div class="container hero-content">
‎    <div class="eyebrow">Welcome to AWS Developer Store</div>
‎    <h1>Fresh finds.<br>Everyday essentials.</h1>
‎    <p>Explore our collection of useful everyday products. Find something you like, add it to your cart, and contact us to ask about ordering.</p>
‎    <div class="hero-actions"><a class="btn btn-gold" href="#products">Shop Now <span>→</span></a><a class="btn btn-outline" href="#contact">Contact Us</a></div>
‎  </div>
‎</section>
‎<div class="highlights"><div class="container highlight-row"><div class="highlight"><span>✦</span>Easy product browsing</div><div class="highlight"><span>▣</span>Simple shopping cart</div><div class="highlight"><span>↗</span>Direct WhatsApp enquiries</div></div></div>
‎
‎<section class="section" id="products">
‎  <div class="container">
‎    <div class="section-head"><div><div class="kicker">Browse our collection</div><h2>Featured products</h2><p class="muted">Swipe horizontally or use the arrows to explore the product images.</p></div>
‎    <div class="controls"><button class="circle" id="prev" aria-label="Previous products">←</button><button class="circle" id="next" aria-label="Next products">→</button></div></div>
‎    <div class="carousel" id="carousel" aria-label="Featured product carousel"></div>
‎  </div>
‎</section>
‎
‎<section class="section catalog" id="catalog">
‎  <div class="container"><div class="kicker">Shop the range</div><h2>All products</h2><p class="muted">Search the collection and add items to your cart. Names and prices can be edited in the product data in this file.</p>
‎  <input class="search" id="search" type="search" placeholder="Search products..." aria-label="Search products">
‎  <div class="grid" id="productGrid"></div></div>
‎</section>
‎
‎<section class="section" id="about"><div class="container about-grid">
‎  <div class="about-photo"><img src="https://i.ibb.co/0Vcnn4zy/images.jpg" alt="AWS Developer Store" loading="lazy" onerror="this.style.display='none'"></div>
‎  <div class="about-copy"><div class="kicker">About our store</div><h2>Your local stop for everyday needs.</h2>
‎  <p>Welcome to AWS Developer Store. Browse our collection, add products to your cart, and contact us directly if you have questions about an item.</p>
‎  <p>This website is designed to make exploring products easy on mobile phones, tablets, and computers.</p>
‎  <div class="points"><div>Easy-to-browse product collection</div><div>Cart with quantity controls</div><div>Direct contact for product enquiries</div></div>
‎  <a class="btn" href="#contact">Get in touch →</a></div>
‎</div></section>
‎
‎<section class="section contact" id="contact"><div class="container contact-grid">
‎  <div><div class="kicker">Contact us</div><h2>Need help choosing a product?</h2><p class="muted">Send us an email or message us on WhatsApp to ask about product availability and ordering.</p><a class="btn btn-gold" id="contactWhatsApp" href="#contact">Message on WhatsApp ↗</a></div>
‎  <div class="contact-card">
‎    <div class="contact-line"><span class="contact-icon">✉</span><div><small>Email</small><a href="mailto:awsdeveloper12531@gmail.com">awsdeveloper12531@gmail.com</a></div></div>
‎    <div class="contact-line"><span class="contact-icon">☎</span><div><small>Phone</small><span id="phoneDisplay">Add your phone number in the settings below</span></div></div>
‎    <div class="contact-line"><span class="contact-icon">◉</span><div><small>WhatsApp</small><span id="whatsappDisplay">Add your WhatsApp number in the settings below</span></div></div>
‎    <p style="color:#c2d0c5;font-size:.82rem">Prices shown are editable examples. Confirm final prices and availability with the store.</p>
‎  </div>
‎</div></section>
‎</main>
‎<footer><div class="container footer-row"><div>© <span id="year"></span> <strong>AWS Developer Store</strong>. All rights reserved.</div><div>Fresh finds, everyday essentials.</div></div></footer>
‎<a class="whatsapp" id="floatingWhatsApp" href="#contact" aria-label="WhatsApp contact"><span aria-hidden="true">◉</span><span class="wa-text">WhatsApp us</span></a>
‎
‎<div class="cart-panel" id="cartPanel" aria-hidden="true">
‎  <div class="cart-backdrop" id="cartBackdrop"></div>
‎  <aside class="cart-drawer" role="dialog" aria-modal="true" aria-labelledby="cartTitle">
‎    <div class="cart-head"><h2 id="cartTitle">Your cart</h2><button class="close-cart" id="closeCart" aria-label="Close cart">×</button></div>
‎    <div class="cart-list" id="cartList"></div>
‎    <div class="cart-total"><span>Total</span><span id="cartTotal">Rs 0</span></div>
‎    <form class="checkout-form" id="checkoutForm">
‎      <h3 style="margin:8px 0 0">Delivery & customer details</h3>
‎      <p class="required-note">Fill in your details to create an order and receive an on-screen confirmation.</p>
‎      <div class="form-row">
‎        <label>Full name *<input name="customerName" autocomplete="name" required maxlength="100" placeholder="Your full name"></label>
‎        <label>Phone number *<input name="customerPhone" type="tel" autocomplete="tel" required maxlength="25" placeholder="03xx xxxxxxx"></label>
‎      </div>
‎      <label>Email address *<input name="customerEmail" type="email" autocomplete="email" required maxlength="160" placeholder="you@example.com"></label>
‎      <label>Delivery address *<textarea name="address" autocomplete="street-address" required maxlength="500" placeholder="House, street, area, city"></textarea></label>
‎      <div class="form-row">
‎        <label>City *<input name="city" autocomplete="address-level2" required maxlength="80" placeholder="Your city"></label>
‎        <label>Postal code (optional)<input name="postalCode" autocomplete="postal-code" maxlength="20" placeholder="Postal code"></label>
‎      </div>
‎      <label>Payment method *
‎        <select name="paymentMethod" required>
‎          <option value="Cash on Delivery">Cash on Delivery (COD)</option>
‎          <option value="Bank transfer - confirm with shop">Bank transfer (confirm with shop)</option>
‎        </select>
‎      </label>
‎      <label>Order notes (optional)<textarea name="notes" maxlength="500" placeholder="Delivery instructions or other requests"></textarea></label>
‎      <p class="required-note">Please check your details before placing the order. This demo stores orders in this browser only; it does not send automatic email or save orders to a shared shop database.</p>
‎      <button class="btn checkout" id="checkout" type="submit">Place order</button>
‎    </form>
‎    <div class="order-confirmation" id="orderConfirmation" role="status" aria-live="polite">
‎      <h3>Order created successfully</h3>
‎      <div>Your order ID:</div><div class="order-id" id="confirmedOrderId"></div>
‎      <div class="order-summary" id="confirmedOrderSummary"></div>
‎      <p style="font-size:.82rem;margin-bottom:0">Keep your order ID for reference. For actual email delivery and centralized order management, connect a backend/email service.</p>
‎      <div style="display:flex;gap:8px;flex-wrap:wrap;margin-top:12px"><button type="button" class="secondary-btn" id="copyOrder">Copy order details</button><button type="button" class="btn" id="sendOrderWhatsApp">Send to shop on WhatsApp</button></div>
‎    </div>
‎  </aside>
‎</div>
‎<div class="toast" id="toast" role="status" aria-live="polite"></div>
‎
‎<script>
‎// SHOP SETTINGS: enter your real phone and WhatsApp numbers before publishing.
‎// Use international digits only for WhatsApp (example format: 923001234567).
‎// Orders get an ID and are stored in this browser's localStorage only.
‎// For real customer email confirmations and orders shared across devices, 
