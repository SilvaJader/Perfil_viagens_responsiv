[README.md](https://github.com/user-attachments/files/29684292/README.md)
### **Usage**



Brief instructions on how to use the project. Simply open index.html in your browser. The layout is responsive and adapts to mobile and desktop views.

### 

### Responsive Design



This project uses a mobile-first approach with CSS media queries:



* **Mobile:** Default styles for devices under 80em (1280px)
* **Desk**top: Enhanced layout for screens 80em and wider



### 

### Key Implementation Details



**Responsive Images Grid:** Uses CSS Grid with minmax() to maintain consistent aspect ratios across different screen sizes while preventing scrollbar overflow issues.



@media (width >= 80em) {

&#x20; .pictures {

&#x20;   padding: 1.5rem 2rem;

&#x20;   display: grid;

&#x20;   grid-template-columns: repeat(4, minmax(0, 1fr));

&#x20;   gap: 1.5rem;

&#x20;   \& .pic-img {

&#x20;     width: 100%;

&#x20;     aspect-ratio: 1 / 1;

&#x20;     height: auto;

&#x20;     object-fit: cover;

&#x20;   ...





##### **Aspect Ratio Control:** 

Images maintain a 1:1 aspect ratio using aspect-ratio: 1 / 1 and object-fit: cover for consistent visual presentation.



##### **Desktop-Only Elements:** 

Classes like .desktop-only are hidden by default and shown only on larger screens using media queries.



.desktop-only {

&#x20; display: none;

}



@media (width >= 80em) {

&#x20; .desktop-only {

&#x20;   display: initial;

&#x20; }...



##### **Browser Support**



Works on all modern browsers (Chrome, Firefox, Safari, Edge).





