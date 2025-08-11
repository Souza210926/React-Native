# Instalação do React Native 

Como instalar e configurar o React Native das **duas formas**:

- Usando a **CLI oficial** (acesso total a código nativo)
- Usando o **Expo** (mais rápido e simples para começar)

---

## 1. Instalação via React Native CLI

### 📋 Pré-requisitos

Configurar e instalar os seguintes: 

- [Node.js (LTS)](https://nodejs.org)
- [Java JDK 17](https://adoptium.net)
- [Android Studio](https://developer.android.com/studio)

---

### Criando o projeto

```bash
# Para criar projeto com a CLI oficial
npx react-native init MeuProjeto

# Entrar na pasta do projeto
cd MeuProjeto
```

---

### Executando o app

```bash
# Android
npx react-native run-android

# iOS
npx react-native run-ios
```

---

## 2. Instalação via Expo

O **Expo** é uma plataforma que facilita o desenvolvimento React Native, sem precisar configurar SDKs e código nativo inicialmente.

### Criando o projeto

```bash
# Instalar CLI do Expo
npm install -g expo-cli

# Criar novo projeto
expo init MeuAppExpo

# Entrar na pasta
cd MeuAppExpo
```

---

### Executando o app

```bash
# Rodar o projeto
expo start
```

Isso abrirá o **Metro Bundler** no navegador, permitindo rodar o app:

- No emulador Android/iOS
- No dispositivo físico via **Expo Go** (disponível na Play Store e App Store)

---

## Diferenças entre CLI e Expo

| Característica                 | React Native CLI                                       | Expo                                                           |
| ------------------------------ | ------------------------------------------------------ | -------------------------------------------------------------- |
| **Acesso a código nativo**     | Total                                                  | Limitado (precisa de "Eject" para APIs nativas personalizadas) |
| **Facilidade de configuração** | Média (precisa configurar SDKs, Android Studio, Xcode) | Alta (nenhuma configuração de SDK necessária)                  |
| **Tamanho inicial do app**     | Menor                                                  | Maior (bibliotecas Expo incluídas)                             |
| **Atualizações OTA**           | Manual                                                 | Integrado via Expo Updates                                     |
| **Velocidade para prototipar** | Média                                                  | Alta                                                           |
| **Controle sobre build**       | Total (Android Studio / Xcode)                         | Limitado (build na nuvem com `expo build`)                     |

---

## Resumo

- **CLI** → Ideal para quem precisa de acesso completo a APIs nativas e customizações profundas.
- **Expo** → Melhor para começar rápido, prototipar e testar sem configurar todo o ambiente nativo.

---

📚 Mais informações:

- [Documentação React Native](https://reactnative.dev/docs/getting-started)
- [Documentação Expo](https://docs.expo.dev)
