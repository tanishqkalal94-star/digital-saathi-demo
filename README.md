# digital-saathi-demo
Official Digital Saathi demo app for a secure document wallet concept prototype
const menuToggle = document.querySelector('.menu-toggle');
const navigation = document.querySelector('.primary-nav');
const dialog = document.querySelector('#demo-dialog');
const closeDialog = document.querySelector('.dialog-close');
const previewButton = document.querySelector('#preview-share');
const result = document.querySelector('#demo-result');
const toast = document.querySelector('#toast');
let toastTimer;

menuToggle?.addEventListener('click', () => {
  const isOpen = menuToggle.getAttribute('aria-expanded') === 'true';
  menuToggle.setAttribute('aria-expanded', String(!isOpen));
  menuToggle.setAttribute('aria-label', isOpen ? 'Open navigation' : 'Close navigation');
  navigation?.classList.toggle('is-open', !isOpen);
});

navigation?.querySelectorAll('a').forEach((link) => {
  link.addEventListener('click', () => {
    navigation.classList.remove('is-open');
    menuToggle?.setAttribute('aria-expanded', 'false');
    menuToggle?.setAttribute('aria-label', 'Open navigation');
  });
});

function openDemo() {
  if (typeof dialog?.showModal === 'function') {
    dialog.showModal();
  } else {
    showToast('This browser does not support the interactive preview.');
  }
}

document.querySelectorAll('[data-open-demo]').forEach((button) => {
  button.addEventListener('click', openDemo);
});

closeDialog?.addEventListener('click', () => dialog.close());

dialog?.addEventListener('click', (event) => {
  if (event.target === dialog) dialog.close();
});

previewButton?.addEventListener('click', () => {
  const documentName = document.querySelector('#sample-document')?.value;
  const purpose = document.querySelector('#sample-purpose')?.value;
  result.innerHTML = `<strong>Sample permission preview</strong>${escapeHTML(documentName)} would be shared for: ${escapeHTML(purpose)}.<br>This is only a visual preview—no data has been sent.`;
  result.hidden = false;
});

function escapeHTML(value) {
  return String(value).replace(/[&<>\"']/g, (character) => ({
    '&': '&amp;', '<': '&lt;', '>': '&gt;', '"': '&quot;', "'": '&#39;'
  })[character]);
}

function showToast(message) {
  if (!toast) return;
  toast.textContent = message;
  toast.classList.add('is-visible');
  window.clearTimeout(toastTimer);
  toastTimer = window.setTimeout(() => toast.classList.remove('is-visible'), 2800);
}

document.querySelector('#year').textContent = new Date().getFullYear();
