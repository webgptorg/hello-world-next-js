#!/usr/bin/env ptbk

# ✨ Example: Write Hello for a user

-   URL `https://promptbook.studio/examples/hello.book`
-   INPUT PARAMETER `{yourName}` Name of the user
-   OUTPUT PARAMETER `{greeting}` Greeting for the user

## Sample of the name

- SAMPLE

> Paul

`-> {yourName}`

## Sample of the name

- SAMPLE

> George

`-> {yourName}`

## Writing Greeting

-   PERSONA Jane, HR professional with prior experience in writing emails
-   EXPECT MIN 1 Word
-   EXPECT MAX 1 Line

```markdown
You are writing a greeting for {yourName}.

## Rules

-   Write just the greeting, nothing else
```

`-> {greeting}`
