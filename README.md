# UI/UX Notes

A place for me to dump all my things I am learning about UI/UX

##UX
### Forms
- **Always use single column forms** are much better for usability and decrease the chance of users misunderstanding the sequential flow of the form.
- **Long forms should be broken into smaller parts** to increase user completion rate
    - A stepper is a great way of breaking your form into smaller easier to complete steps. 
- **Avoid placeholders as description for the input** 
    - using placeholders as description is bad practice due to losing your description when you input anything
- **Avoid placeholder as label**
    - when using placeholder as label you lose the input label
    - this can be okay if you are doing it the Material way that is, while empty use placeholder and float to top when not empty input
- **Put labels above input.** Google’s UX researchers found that aligning labels above fields on the left-hand side increased form completion time. This is because it requires fewer ‘visual fixations’
- **Input should be sized according to the size of the expected input** (i.e. do not use full with for zip code input), having the input larger than the expected input makes users second guess what they are supposed to do.

### Type
- Font size
  - body text 16px you can not go wrong with - usually header should be around 2.5x the size of the body text (40px) in this case - that should be 1rem vs 2.5rem
- Prefer smaller line height on larger text, increase line height on paragraphs to make more legible

## UI
- **Do not use high contrast borders** they draw unecessary attention from your eyes
    - using the law of proximity can aleviate a lot of the problems that borders are trying to solve.
    - using borders can be fine in some cases when they are low contrast
- Religious Debates 
    - People think everyone on the web thinks in the way that they do, if I dont like it nobody will 
    - You can sit and argue design decisions but the only thing that will really help is user testing
    #### Mobile Design
    - For margins we recommend keeping a safe zone of at least 20 pixels vertically free on each side (https://instapage.com/blog/mobile-landing-page-design)