# Nice Pricing Card

![image](https://github.com/WajdWael/nicePricingCard/assets/81550668/b5d19db8-6492-49e2-9f49-96b1b4721e89)
[Demo - Preview Website](https://wajdwael.github.io/nicePricingCard/)

Support us with a star ⭐!

---

# Goal 🧠:

This project for advanced CSS developers.

# Key Points 🗝️:

  1. **Variables: define them by using `:root{}`**

  ---
  
  2. **Adjust font-size for small screens:**
      - ```CSS
        @media (min-width: 968px) {
          :root {
            /* == TIPOGRAPHY == */
            --biggest-sz: 2.125rem;
            --h2-sz: 1.5rem;
            --normal-sz: 1rem;
            --small: 0.875rem;
            --smaller0: 0.813rem;
            --tiny: 0.688rem;
          }
        }
        ```
  --- 

  3. **Shadow in hover effect:**
      - ```CSS
        .card__content:hover {
          box-shadow: 0 16px 24px hsla(var(--hue-clr), 61%, 16%, 0.15);
        }
        ```

  ---
  
  
  4. ## How to create a circle with CSS:
      -  **You should equal the width and the height, with border-radius: 50% to show the circle you should give it a color.**
      - ```CSS
        .card__header-circle {
          width: 40px;
          height: 40px;
          background-color: var(--lihgter-clr);
          border-radius: 50%;
          margin-bottom: 1rem;
          place-items: center;
        }
        ```
--- 
![image](https://github.com/WajdWael/nicePricingCard/assets/81550668/44da65bb-c245-4c4e-bbd3-1b731789cb51)

  5. How to create this
       - ```CSS
         // ::before creates the small triangle 
         .card__pricing::before {
            width: 14px;
            height: 16px;
            background-color: var(--one-clr);
            top: 0;
            left: -14px;
            clip-path: polygon(0 100%, 100% 0, 100% 100%);
          }
         // ::after create the figure at the end 
          .card__pricing::after {
            width: 100%;
            height: 14px;
            background-color: #fff;
            left: 0;
            bottom: -1px;
            clip-path: polygon(0 100%, 50% 0, 100% 100%);
          }
         ```
       - According to MDN ``The clip-path CSS property``: creates a clipping region that sets what part of an element should be shown. Parts that are inside the region are shown, while those outside are hidden. 
       - According to MDN ``polygon()``: **Defines a polygon using an SVG filling rule and a set of vertices.**

---

Thanks,
