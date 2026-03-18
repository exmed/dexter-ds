# Dexter

Design System by Exmed 😎

[![version](https://img.shields.io/npm/v/@exmed/dexter-ds.svg)](https://www.npmjs.com/package/@exmed/dexter-ds)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

<img align="right" alt="Logo" src="website/static/logo.png" style="margin-bottom: 16px">


## Como utilizar

Instale no seu projeto:

```bash
npm i @exmed/dexter-ds
```

Neste repositório, você encontrará

- [Cores](#cores)
- [Ícones](#ícones)

### Cores

Utilize as cores individuais ou o conjunto completo:

```js
import { primary } from "@exmed/dexter-ds/lib/colors"

primary[20];	// "#B1EFE8"
...					// ...
primary[40];		// "#83E7DB"
```

```js
import * as colors from '@exmed/dexter-ds/lib/colors';

colors; // { primary: {...}, empresas: {...}, ... }

colors.empresas[0]; // "#6161FF"
```

### Ícones

Utilize os ícones de acordo com a sua plataforma

### React web

`index.jsx`

```jsx
import { IcClose } from '@exmed/dexter-ds/lib/icons';

<Container>
	<IcClose />
</Container>;
```

`styles.js`

```js
import styled from 'styled-components';
import { neutral } from '@exmed/dexter-ds/lib/colors';

const Container = styled.div`
	color: ${neutral[90]}; // #141414

	svg {
		${neutral[0]}; // #FFFFFF
	}
`;
// A cor do ícone será sempre herdada do seu pai, caso não seja definida diretamente.
```

### React Native

`styles.js`

```js
import styled from "styled-components";
import { neutral } from "@exmed/dexter-ds/lib/colors"
---
import { IcClose } from "@exmed/dexter-ds/lib/icons/svg";

const Icon = styled(Close)`
	color: ${neutral[90]};		// #141414
`
```

### Imagens

As imagens podem ser acessadas pelo diretório `/lib/images`

```js
import BrFlag from "@exmed/dexter-ds/lib/images/flag_for_brasil.svg";

import NoRequisition from "@exmed/dexter-ds/lib/images/empty-states/report.svg";
```

### Bons códigos 🧑‍💻🖥️⚙️
