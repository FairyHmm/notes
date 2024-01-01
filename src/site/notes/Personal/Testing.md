---
{"dg-publish":true,"permalink":"/Personal/Testing/"}
---

---
---
<style>
    table th, table td { padding: 6px; }
</style>

> a
> > a
> > > a
> > > > a
> > > > > a

* * *

<details>aa</details>
<details><summary>aa</summary>bb</details>

||aa||

|aa|

<!-- aa -->

! aaaa
<p>>! aaa</p>


- ||
|-|
|a|


A
: a
: a

-
: |-|
|a|
|a|

a
\
&emsp;a
\
&emsp;&emsp;a

<ul>
a

-
|-|
|a|
</ul>

| Just                               | a   | normal       | table |
| ---------------------------------- | --- | ------------ | ----- |
| Use `<` to merge cells to the left | <   | Merged cell! | <     |
| Use `^` to merge cells up          | <   | ^            | ^     |

| I        | -   | have | horizontal | headers |
| -------- | --- | ---- | ---------- | ------- |
| also     | -   | foo  | bar        | <       |
| have     | -   | 1    | 2          | 3       |
| vertical | -   | A    | B          | C       |
| headers! | -   | X    | Y          | Z       |


```mermaid
graph LR;
	A--> B & C & D;
	B--> A & E;
	C--> A & E;
	D--> A & E;
	E--> B & C & D;
``` 

```mermaid
erDiagram
	CUSTOMER }|..|{ DELIVERY-ADDRESS : has
	CUSTOMER ||--o{ ORDER : places
	CUSTOMER ||--o{ INVOICE : "liable for"
	DELIVERY-ADDRESS ||--o{ ORDER : receives
	INVOICE ||--|{ ORDER : covers
	ORDER ||--|{ ORDER-ITEM : includes
	PRODUCT-CATEGORY ||--|{ PRODUCT : contains
	PRODUCT ||--o{ ORDER-ITEM : "ordered in"
```


<style>
	testin:before { content: '['; }
	testin:after {  content: ']'; }
</style>

<testin>a</testin>

a <t:1689698880:f>

|  | < | < |
| ---- | ---- | ---- |
|  |  |  |
| ^ |  | < |
