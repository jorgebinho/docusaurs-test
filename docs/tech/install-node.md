---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# 🟢 Como Instalar o Node.js no Ubuntu

A forma mais recomendada é usando o **NVM** (Node Version Manager), que permite instalar e trocar de versão facilmente.

## 1. Instalar o NVM

<Tabs>
  <TabItem value="bash" label="bash / zsh" default>

```bash
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

  </TabItem>
  <TabItem value="fish" label="fish shell">

```bash
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
  source ~/.config/fish/config.fish
```

  </TabItem>
</Tabs>
Depois, recarregue o terminal:

```bash
source ~/.bashrc
```

## 2. Verificar se o NVM foi instalado

```bash
nvm --version
```

## 3. Instalar o Node.js

```bash
nvm install --lts
```

## 4. Verificar a instalação

```bash
node -v
npm -v
```

:::tip Dica
Com o NVM você pode ter várias versões instaladas e trocar entre elas com `nvm use 18`, `nvm use 20`, etc.
:::

:::info Por que NVM?
Instalar pelo `apt` do Ubuntu costuma trazer versões antigas. O NVM garante sempre a versão que você quiser.
:::