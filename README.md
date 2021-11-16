# UI/UX Notes

A place for me to dump all my things I am learning about UI/UX

## UX
### Forms
- Avoid multi-column forms 
    - If a form has horizontally adjacent fields, then the user must scan in a Z pattern, slowing the speed of comprehension and muddying the path to completion.
    - Single column froms have a straight line down to completion.
- Break long forms into smaller pieces
    - When designing forms general rule of thumb is that the less fields the better. Less effort on the user or percieved less effort results in higher completion rate.
    - Displaying 5-7 inputs at a time is a [common practice](https://xd.adobe.com/ideas/principles/web-design/best-practices-form-design/) 
    - A stepper is a great way of breaking your form into smaller easier to complete steps. 
- Avoid placeholders as description for the input
    - Using placeholders as description is bad practice due to losing your description when you input anything.
- Avoid placeholder as label
    - When using placeholder as label you lose the input label.
    - This can be okay if you are using floating placeholders (placeholder moves to label when there is input).
- Put labels above input.
    -  Google’s UX researchers found that aligning labels above fields on the left-hand side increased form completion time. This is because it requires fewer ‘visual fixations’.
- Input should be sized according to the size of the expected input** (i.e. do not use full with for zip code input), 
    - having the input larger than the expected input makes users second guess what they are supposed to do.
- Action Buttons
    - Avoid generic words on the button for example "Submit", instead use descriptive words for example "Create Account", "Place Order", etc.
    - 99% of the time it is the wrong choice to include reset buttons.
- Validation
    - Validation is all over the place with implementation but the Reward early, punish late paradigm I tend to agree with the most
    - Reward early, punish late ["Inline Validation in Forms: Designing the Experience"](https://medium.com/wdstack/inline-validation-in-forms-designing-the-experience-123fb34088ce)
        - If field is empty or valid only show validations on leaving the input.
        - If field input was left at an invalid state and returned to, validate during input.
        - Implementation described in the article above looks like
            - The validation library must keep track of the dirty fields.
            - If the field was in a valid state, perform the validation on the blur event
            - If the field was in an invalid state, perform the validation when the field value is changed (using the combination of onchange, onblur and onkeypress events)
            - When the field goes from the invalid to valid state, treat it like a valid field

### Type
- Font size
  - Body text 16px you can not go wrong with 
    - usually header should be around 2.5x the size of the body text (40px) in this case 
    - that should be 1rem vs 2.5rem
- Prefer smaller line height on larger text, increase line height on paragraphs to make more legible

## UI
- **Do not use high contrast borders** they draw unecessary attention from your eyes
    - using the law of proximity can aleviate a lot of the problems that borders are trying to solve.
    - using borders can be fine in some cases when they are low contrast
- Religious Debates 
    - People think everyone on the web thinks in the way that they do, if I dont like it nobody will 
    - You can sit and argue design decisions but the only thing that will really help is user testing
- The landing page should generally consist of a Hero Section which are made up of:
    - Headline
    - Sub-headline (optional)
    - Call to action
    - Usually some art or and illustration
### Mobile Design
- For margins we recommend keeping a safe zone of at least 20 pixels vertically free on each side (https://instapage.com/blog/mobile-landing-page-design)
