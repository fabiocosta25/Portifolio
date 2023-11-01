// Função para mostrar/ocultar o menu
function toggleMenu(toggleId, navId) {
  const toggle = document.getElementById(toggleId);
  const nav = document.getElementById(navId);

  if (toggle && nav) {
    toggle.addEventListener('click', () => {
      nav.classList.toggle('show');
    });
  }
}

toggleMenu('nav-toggle', 'nav-menu');

// Função para lidar com a ação do link do menu
function linkAction() {
  const navMenu = document.getElementById('nav-menu');
  // Quando clicamos em um link, removemos a classe 'show' do menu
  navMenu.classList.remove('show');
}

const navLinks = document.querySelectorAll('.nav__link');
navLinks.forEach((link) => link.addEventListener('click', linkAction));

// Função para destacar a seção ativa com base no scroll
const sections = document.querySelectorAll('section[id]');

function scrollActive() {
  const scrollY = window.pageYOffset;

  sections.forEach((current) => {
    const sectionHeight = current.offsetHeight;
    const sectionTop = current.offsetTop - 50;
    const sectionId = current.getAttribute('id');

    const link = document.querySelector(`.nav__menu a[href*=${sectionId}]`);

    if (scrollY > sectionTop && scrollY <= sectionTop + sectionHeight) {
      link.classList.add('active');
    } else {
      link.classList.remove('active');
    }
  });
}

window.addEventListener('scroll', scrollActive);

// Configurações para animação de revelação de scroll
const sr = ScrollReveal({
  origin: 'top',
  distance: '60px',
  duration: 2000,
  delay: 200,
  // reset: true
});

// Definindo os elementos a serem revelados
sr.reveal('.home__data, .about__img, .skills__subtitle, .skills__text', {});
sr.reveal('.home__img, .about__subtitle, .about__text, .skills__img', {
  delay: 400,
});
sr.reveal('.home__social-icon', { interval: 200 });
sr.reveal('.skills__data, .work__img, .contact__input', { interval: 200 });
