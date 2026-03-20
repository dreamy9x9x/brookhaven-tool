# 🧰 Brookhaven Tool - Roblox Script

Este repositório contém uma ferramenta personalizada para o jogo **Brookhaven 🏡RP**, desenvolvida em **Luau** (linguagem usada no Roblox).  
Ela oferece funcionalidades prontas para facilitar a criação de scripts no Brookhaven.

---

## 📦 Código de Importação

```lua
local brookhavenTool = loadstring(game:HttpGet("https://raw.githubusercontent.com/Laelmano24/brookhaven-tool/refs/heads/main/src/main.luau"))()
```

Esse comando faz o seguinte:

- Baixa o script principal diretamente do GitHub.
- Executa o script e retorna um objeto com funções utilitárias.

---

## 🛠️ Funcionalidades

### 📍 teleport, teleportVehicle e teleportToPlayer

#### 🧭 teleport
```lua
brookhavenTool:teleport(position)
```

- `position` (Vector3): A posição de destino (eixos X, Y, Z).

#### 🧭 teleportVehicle
```lua
brookhavenTool:teleportVehicle(position)
```

- `position` (Vector3): A posição de destino do veículo.

**Exemplo:**
```lua
brookhavenTool:teleportVehicle(Vector3.new(100, 100, 100))
```

#### 🧭 teleportToPlayer
```lua
brookhavenTool:teleportToPlayer(playerName)
```

- `playerName` (string): Nome do jogador para o qual deseja teleportar.

**Exemplo:**
```lua
brookhavenTool:teleportToPlayer("Laelmano24")
```

---

### 🎥 spectatePlayer

```lua
brookhavenTool:spectatePlayer({state, playerName})
```

- `state` (boolean): `true` para começar a espectar, `false` para parar.
- `playerName` (string): Nome do jogador que será espectado.

**Exemplo:**
```lua
brookhavenTool:spectatePlayer({true, "Laelmano24"})
```

---

### 🚫 removeBanHouses e autoRemoveBanHouses

#### 🔹 removeBanHouses
```lua
brookhavenTool:removeBanHouses()
```

#### 🔹 autoRemoveBanHouses
```lua
brookhavenTool:autoRemoveBanHouses(state)
```

- `state` (boolean): `true` para ativar, `false` para desativar.

**Exemplo:**
```lua
brookhavenTool:autoRemoveBanHouses(true) -- Ativa o autoRemoveBanHouses
```

---

### 🚗 checkPlayerSittingCar

```lua
brookhavenTool:checkPlayerSittingCar({targetName, nameVehicle, onlyVehicleSeat})
```

- `targetName` (string): Nome do jogador que você quer verificar.
- `nameVehicle` (string): Nome do jogador dono do veículo.
- `onlyVehicleSeat` (boolean): `true` para verificar apenas o assento do piloto, `false` para verificar todos os assentos.

**Exemplos:**
```lua
brookhavenTool:checkPlayerSittingCar({"SlaPow2025", "Laelmano24", false})
-- Verifica se o jogador "SlaPow2025" está em qualquer assento do veículo do "Laelmano24"

brookhavenTool:checkPlayerSittingCar({"SlaPow2025", "Laelmano24", true})
-- Verifica se o jogador "SlaPow2025" está no assento do piloto do veículo do "Laelmano24"
```

### 👘 getIdAccessoriesPlayer

```lua
brookhavenTool:getIdAccessoriesPlayer(targetName, typeCopy)
```

- `targetName` (string): Nome do jogador que você querer copiar.
- `typeCopy` (string): O tipo de copiar, para copiar a skin do brookhaven ou do perfil da roblox.

**Exemplos:**
```lua
brookhavenTool:getIdAccessoriesPlayer("Laelmano24", "brookhaven")
-- Ele retorna uma lista dos ids do jogador no brookhaven.

brookhavenTool:getIdAccessoriesPlayer("Laelmano24", "roblox")
-- Ele retorna uma lista dos ids do jogador no roblox.
```

### 👘 getIdsBodyPlayer

```lua
brookhavenTool:getIdsBodyPlayer(targetName, typeCopy)
```

- `targetName` (string): Nome do jogador que você querer copiar.
- `typeCopy` (string): O tipo de copiar, para copiar a skin do brookhaven ou do perfil da roblox.

**Exemplos:**
```lua
brookhavenTool:getIdsBodyPlayer("Laelmano24", "brookhaven")
-- Ele retorna uma lista de ids do corpo do jogador na ordem do remote que modifica o corpo do personagem.

brookhavenTool:getIdsBodyPlayer("Laelmano24", "roblox")
-- Ele retorna uma lista de ids do corpo do jogador na ordem do remote que modifica o corpo do personagem, a diferença é que vai pegar do perfil da roblox.
```

### 👘 getIdsClothesPlayer

```lua
brookhavenTool:getIdsClothesPlayer(targetName, typeCopy)
```

- `targetName` (string): Nome do jogador que você querer copiar.
- `typeCopy` (string): O tipo de copiar, para copiar a skin do brookhaven ou do perfil da roblox.

**Exemplos:**
```lua
brookhavenTool:getIdsClothesPlayer("Laelmano24", "brookhaven")
-- Ele retorna uma lista que o primeiro valor vai ser o id da camisa e segundo valor vai ser o id da calça do brookhaven.

brookhavenTool:getIdsClothesPlayer("Laelmano24", "roblox")
-- Ele retorna uma lista que o primeiro valor vai ser o id da camisa e segundo valor vai ser o id da calça do perfil do usuario da roblox.
```

### 👘 getColorPlayer

```lua
brookhavenTool:getColorPlayer(targetName, typeCopy)
```

- `targetName` (string): Nome do jogador que você querer copiar.
- `typeCopy` (string): O tipo de copiar, para copiar a skin do brookhaven ou do perfil da roblox.

**Exemplos:**
```lua
brookhavenTool:getColorPlayer("Laelmano24", "brookhaven")
-- Ele retorna a cor da cabeça do jogador do brookhaven.

brookhavenTool:getColorPlayer("Laelmano24", "roblox")
-- Ele retorna a cor da cabeça do jogador, mas do perfil da roblox dele. 
```
### ✉️ spamInviteAllPlayersToFamily

```lua
brookhavenTool:spamInviteAllPlayersToFamily()
```


**Exemplos:**
```lua

```

---

⚠️ **Aviso**

Este script é feito para fins educacionais e experimentais.  
O uso de scripts de terceiros pode violar os Termos de Serviço da Roblox, podendo resultar em banimento.  
Use por sua conta e risco.

---

## 🛠 Autor

**Laelmano24**  
[GitHub](https://github.com/Laelmano24)

**Nexusdevy**
[GitHub](https://github.com/dreamy9x9x)
