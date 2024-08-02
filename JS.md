#js

```script.js
//sidebar
// document.getElementById('toggle-btn').addEventListener('click', show())
function show(){
    document.getElementById('sidebar').classList.toggle('active');
    }


//sliding img

    const slides = document.querySelectorAll(".slides img");
    let slideIndex = 0;
    let intervalId = null;
    
    // initializeSlider();
    document.addEventListener("DOMContentLoaded", initializeSlider)
    
    function initializeSlider() {

        if (slides.length>0) {
        slides[slideIndex].classList.add('displaySlide');
        intervalId = setInterval(nextSlide, 3000);
        // console.log(intervalId);
        }
        
    }
    
    
    function showSlide(index) {
    if (index >= slides.length) {
            slideIndex = 0;

    }
    else if(index < 0){
        slideIndex = slides.length - 1;
    }

    slides.forEach(slide => {
    slide.classList.remove("displaySlide");
    });

    slides[slideIndex].classList.add("displaySlide");

    }
    
    function nextSlide() {
        slideIndex++;
        showSlide(slideIndex);
    }
    
    function prevSlide() {
        clearInterval(intervalId);
        slideIndex--;
        showSlide(slideIndex);
    }
```
