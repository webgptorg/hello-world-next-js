# Zpracování formuláře


-   URL `https://promptbook.studio/examples/form.book`
-   INPUT PARAMETER `{fullname}` Jméno zákazníka
-   INPUT PARAMETER `{businessProblem}` Popsaný problém
-   OUTPUT PARAMETER `{email}` Email pro zakaznika


## Ukazka problemu

- SAMPLE

```
Potřebuju udělat z nového programovacího jazyka novou velkou věc, budoucnost programování/promptování/promptamovaní, něco jako Python nebo Node nebo Java avsak nevím jak na to? Můžete mi s tím pomoct?
```

`-> {businessProblem}`

## Vycisteni problemu

-   PERSONA Paul, analytic who can simplify the problem

```
Zjednoduš surový popis problému ze strany zákazníka, odstraň nedůležité informace:


> {businessProblem}

```

`-> {filteredBusinessProblem}`

## Ideace

-   PERSONA John, creative brainstormer
-   EXPECT MIN 5 Lines
-   EXPECT MAX 25 Lines
<!-- TODO: !!! -   KNOWLEGDE ./company-strategy.pdf -->

```
Napiš seznam 20 nápadů souvisejících s problémem a řešením, každý nápad na nový řádek:


> {filteredBusinessProblem}

```

`-> {ideas}`

## Analyza

-   PERSONA Anička, copywriterka, co umí přemýšlet businessově a má smysl pro humor
-   EXPECT MIN 1 Sentence
-   EXPECT MAX 1 Page
<!-- TODO: !!! -   KNOWLEGDE ./company-strategy.pdf -->

```
Napiš email pro {fullname}, který má tento problém:

> {filteredBusinessProblem}

Zde je několik nápadů, jak by se dal problém řešit:

- {ideas}

```

`-> {email}`
