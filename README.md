# goit-js-hw-08
<!-- another way wuth variable: -->
<!-- // Отримуємо посилання на ul.gallery
const galleryList = document.querySelector('.gallery');

// Створюємо розмітку
const galleryMarkup = images.map(({ preview, original, description }) => {
  return `
    <li class="gallery-item">
      <a class="gallery-link" href="${original}">
        <img
          class="gallery-image"
          src="${preview}"
          data-source="${original}"
          alt="${description}"
        />
      </a>
    </li>
  `;
}).join('');

// Додаємо всю розмітку до контейнера
galleryList.innerHTML = galleryMarkup;

// Забороняємо стандартну поведінку при кліку
galleryList.addEventListener('click', event => {
  event.preventDefault();
}); -->




 <!-- Conclusion:
Adding = [] is like saying:

If no toppings are specified, just assume it's a plain cheese pizza. -->

<!-- function createGalleryMarkup(data = []) {
That's called a default parameter. It means:

If no argument is passed to this function, use an empty array by default.
 So do you really need it?
No, it's not strictly necessary if you're always calling the function with a valid array (like createGalleryMarkup(images)).

But it is helpful as a safety fallback in case:

You forget to pass any data.
The function gets called with undefined or null due to a bug.
You want to make the function more reusable and robust.

data = [] is not strictly required — but it's a smart safety net.
It prevents your code from breaking if the function is ever called without data.
It's a great habit when working with arrays or objects as parameters. -->