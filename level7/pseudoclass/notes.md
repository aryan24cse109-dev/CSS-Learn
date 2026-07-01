<!----------Notes--------------------->
Used to define special states of HTML Elements.
Syntax : selector:pseudo-class{styles}
common examples: :hover, :active,:first-child.
target elements based on their position or user action on the page. Pseudo-classes are used to add special effects to some selectors.

All pseudo-classes can be divided into three categories:
1) User Action: :hover, :active, :focus, :focus-within, :focus-visible
2) Links: :link, :visited, :hover, :active
3) Forms: :checked, :disabled, :enabled, :required, :optional, :valid, :invalid, :read-only, :placeholder-shown
4) Position: :first-child, :last-child, :nth-child, :only-child, :first-of-type, :last-of-type
5) Others: :not(), :is(), :where(), :has(), :empty, :root, :target


💡 Pseudo Class vs Pseudo Element:
a:hover     → Pseudo Class   (state target karo)  :
p::before   → Pseudo Element (content add karo)   ::
