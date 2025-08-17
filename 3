// Theme helpers
const $ = (q,ctx=document) => ctx.querySelector(q);
const $$ = (q,ctx=document) => [...ctx.querySelectorAll(q)];
const byId = id => document.getElementById(id);

// Data: sample products (replace images, names, prices)
const PRODUCTS = [
  { id:1, name:"PRJKT TK Core Tee — Black", price:1800, tag:"tshirt", badge:"New", img:"https://picsum.photos/seed/tk1/800/800" },
  { id:2, name:"Graffiti Script Tee — White", price:1800, tag:"tshirt", img:"https://picsum.photos/seed/tk2/800/800" },
  { id:3, name:"Nairobi Skyline Hoodie — Jet", price:4200, tag:"hoodie", img:"https://picsum.photos/seed/tk3/800/800" },
  { id:4, name:"PRJKT TK Cap — Midnight", price:1500, tag:"cap", img:"https://picsum.photos/seed/tk4/800/800" },
  { id:5, name:"Logo Stack Tee — Grey", price:1800, tag:"tshirt", img:"https://picsum.photos/seed/tk5/800/800" },
  { id:6, name:"Oversized Hoodie — Stone", price:4500, tag:"hoodie", badge:"Hot", img:"https://picsum.photos/seed/tk6/800/800" }
];

function money(n){
  return new Intl.NumberFormat('en-KE',{style:'currency',currency:'KES',maximumFractionDigits:0}).format(n);
}

function renderProducts(list){
  const wrap = byId('products');
  if(!wrap) return;
  wrap.innerHTML = list.map(p => `
    <article class="card">
      <div class="thumb" style="position:relative">
        ${p.badge ? `<span class="badge">${p.badge}</span>`:''}
        <img src="${p.img}" alt="${p.name}">
      </div>
      <div class="card__body">
        <div class="card__title">${p.name}</div>
        <div class="card__meta">${p.tag.toUpperCase()}</div>
        <div class="price">${money(p.price)}</div>
        <div class="actions">
          <button class="action primary" data-id="${p.id}">Add to Cart</button>
          <button class="action" data-id="${p.id}" data-view>View</button>
        </div>
      </div>
    </article>
  `).join('');
}

function initFilters(){
  const chips = $$('#filters .chip');
  chips.forEach(ch => ch.addEventListener('click', () => {
    chips.forEach(c => c.classList.remove('active'));
    ch.classList.add('active');
    applyFilters();
  }));
  byId('search').addEventListener('input', applyFilters);
}

function applyFilters(){
  const active = $('.chip.active')?.dataset.filter || 'all';
  const q = byId('search').value.trim().toLowerCase();
  const list = PRODUCTS.filter(p => (active==='all' || p.tag===active) && p.name.toLowerCase().includes(q));
  renderProducts(list);
}

function initNav(){
  const btn = byId('hamburger');
  const nav = byId('nav');
  btn?.addEventListener('click', () => {
    const open = nav.classList.toggle('open');
    btn.setAttribute('aria-expanded', open);
  });
  $$('#nav a').forEach(a => a.addEventListener('click', () => nav.classList.remove('open')));
}

function initContact(){
  const form = byId('contactForm');
  const msg = byId('formMsg');
  form?.addEventListener('submit', e => {
    e.preventDefault();
    const data = Object.fromEntries(new FormData(form).entries());
    // Basic validation
    if(!data.name || !data.email || !data.message){
      msg.textContent = 'Please fill out all fields.';
      return;
    }
    // Simulate send — replace with your form endpoint
    msg.textContent = 'Thanks! We\'ll reply via email soon.';
    form.reset();
  });
}

function initYear(){
  const y = byId('year');
  if(y) y.textContent = new Date().getFullYear();
}

// Boot
document.addEventListener('DOMContentLoaded', () => {
  initYear();
  initNav();
  renderProducts(PRODUCTS);
  initFilters();
  initContact();
});
