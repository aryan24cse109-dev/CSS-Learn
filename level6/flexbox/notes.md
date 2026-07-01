----------------Flex Box Notes--------------------

FLEXBOX:

. Flexbox Kya Hai?
Flexbox (Flexible Box Layout) ek CSS layout model hai jo elements ko ek row ya column mein easily align aur distribute karne deta hai — bina float ya position ke.

2. Flexbox Model :

Flexbox mein 2 axes hote hain:

a) MainAxis : Items jis direction mein flow karte hain (default: left → right).
b) Cross Axis : Main axis ke perpendicular (default: top → bottom)

Main Properties:
css.container {
  display: flex;
  flex-direction: row;         /* items ka direction */
  justify-content: center;     /* main axis pe alignment */
  align-items: center;         /* cross axis pe alignment */
  flex-wrap: wrap;             /* items wrap hon ya nahi */
  gap: 10px;                   /* items ke beech space */
}

3. Flex Direction Notes (Short)

flex-direction — ye decide karta hai items kis direction mein flow karenge.
flex-direction: row;            /* → left se right (default) */
flex-direction: row-reverse;    /* ← right se left */
flex-direction: column;         /* ↓ upar se neeche */
flex-direction: column-reverse; /* ↑ neeche se upar */
Visual samajhne ke liye:
row:             [1] [2] [3]  →
row-reverse:     [3] [2] [1]  ←

column:          [1]
                 [2]   ↓
                 [3]

column-reverse:  [3]
                 [2]   ↑
                 [1]


Quick Recap Table : 

a) display: flexFlexbox on karo
b) flex-direction : Items ka flow direction 
c) justify-content : Main axis alignment 
d) align-items : Cross axis alignment 
e) flex-wrap : Items ek se zyada line mein jaayein
f) gap : Items ke beech spacing

 Yaad rakhein: flex-direction change karne se main axis bhi change ho jaata hai, aur uske saath justify-content aur align-items ka kaam bhi swap ho jaata hai!




 Properties: Flexbox Container 
 1) Justify Content:   
a)Alignment: Aligns flex items alomg the main axis
B)flex start : Items align to the start of the flex container 
c) flex end: Items align the end of flex container 
d) space between/space around/space evenly :
distributes space betwen items evenly

code :
justify-content: xxxxxx ;

2)Flex Wrap:

a)nowrap(default):
Sabhi items ek hi line mein rahenge
Agar space nahi hai toh items chhote ho jaayenge (shrink)
Items container se bahar nahi jaayenge (overflow ho sakta hai)
Container: [  1  ][  2  ][  3  ][  4  ][  5  ]  → overflow →

b)wrap:

Jab space kam ho toh items neeche wali line mein chale jaate hain
Items apni natural size maintain karte hain
Sabse zyada use hone wali value hai
Container: [  1  ][  2  ][  3  ]
           [  4  ][  5  ]

c) wrap reverse:

wrap ki tarah hi kaam karta hai lekin ulta
Naye items upar wrap hote hain, neeche nahi
Cross axis reverse ho jaata hai

Container: [  4  ][  5  ]
           [  1  ][  2  ][  3  ]




3) Align Items :
This property is used to align the flex container items along the cross axis which is perpendicular to the main axis .

1. align-items: stretch (Default)
css.container {
  display: flex;
  align-items: stretch;
}

Items puri height tak stretch ho jaate hain
Container ki full height fill karte hain
Tabhi kaam karta hai jab item ki fixed height na ho

Container:
┌─────────────────────────┐
│ [  1  ] [  2  ] [  3  ] │  ← sab same height
└─────────────────────────┘

2. align-items: flex-start
css.container {
  display: flex;
  align-items: flex-start;
}

Sabhi items top se align hote hain (cross axis ka start)
Items apni natural height rakhte hain

Container:
┌─────────────────────────┐
│ [ 1 ] [ 2 ] [ 3 ]       │  ← upar se aligned
│                         │
│                         │
└─────────────────────────┘

3. align-items: flex-end
css.container {
  display: flex;
  align-items: flex-end;
}

Sabhi items bottom se align hote hain (cross axis ka end)
Items apni natural height rakhte hain

Container:
┌─────────────────────────┐
│                         │
│                         │
│ [ 1 ] [ 2 ] [ 3 ]       │  ← neeche se aligned
└─────────────────────────┘

4. align-items: center
css.container {
  display: flex;
  align-items: center;
}

Sabhi items bilkul beech mein align hote hain
Sabse zyada use hone wali value
Perfect vertical centering ke liye

Container:
┌─────────────────────────┐
│                         │
│ [ 1 ] [ 2 ] [ 3 ]       │  ← beech mein
│                         │
└─────────────────────────┘

5. align-items: baseline
css.container {
  display: flex;
  align-items: baseline;
}

Items ke text ki baseline se align hota hai
Jab different font sizes ho tab useful hai
Text ek straight line mein dikhta hai

Container:
┌──────────────────────────────┐
│ big    [ normal ] [ small ]  │
│ text   text       text       │
│  ↑________↑__________↑       │
│         baseline             │
└──────────────────────────────┘



5) Flex Shrink :
The flex shrink property in css determinew how much a flex item will shrnik relative to other items in the flex conatiner if there is insuffient space.

6) Flex Grow: 
It specifies how much a flex item will grow relative to other items in the flex container when additional space is available .
 

 7) Flex-Order:

 It allows you to define the sequence in which flex items appear within the flex container , overriding their orginal order in the html.