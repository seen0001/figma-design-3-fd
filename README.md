# Kort refleksion over projektet:

I implementeringen af Figma-designet valgte jeg at fokusere på en velstruktureret CSS-arkitektur og komponentbaseret udvikling. Min tilgang med CSS nesting har givet mig mulighed for at holde stylingen velorganiseret og vedligeholdelsesvenlig. Det var særligt udfordrende at strukturere de mere komplekse komponenter som HeroSection og Navigation, men ved at bruge nestede selektorer lykkedes det mig at skabe en overskuelig hierarkisk struktur, hvor koden er så clean, som vi nu kan gøre det indtil videre.
Et eksempel på en nyere lært løsning er mit system af custom properties. I global.css etablerede jeg et omfattende sæt variabler for spacing, typografi og farver. Særligt vores nyligt lærte brug af clamp() til responsive størrelser har vist sig meget effektiv. For eksempel definerede jeg fonte sådan her: --font-35-50: clamp(2.1875rem, 1.8614rem + 1.6304vw, 3.125rem);, hvilket gav mig flydende typografi uden behov for mange breakpoints.

## Udfordringer
I udviklingen af komponenter udnyttede jeg Astros logikker. En af de mere komplekse implementeringer var EmployeeCard.astro, hvor jeg håndterede billeder og sociale medier dynamisk gennem props og betingede renderinger. Det var udfordrende at få det hele til at spille sammen, men resultatet blev fleksibelt og genbrugeligt.

Noget anden der har udfordret mig har været klassenavngivningen, da jeg kan have svært ved at huske at gøre disse navne konkrete nok.
Nogle steder endte jeg med at bruge meget beskrivende navne som "newsletter-section", mens andre steder blev mere generiske som "container". Det er helt klart et område, jeg vil forbedre i fremtiden.

Min største tekniske udfordring var dog implementeringen af PieChart-komponenten. Her kombinerede jeg custom properties med JavaScript for at skabe animerede datavisualiseringer.
For responsiviteten valgte jeg primært at arbejde med media queries og fleksible grid-layouts. Dog blev resultatet ikke fuldendt, og dette vil også kunne forbedres.
