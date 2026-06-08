# 🕯️ CírioApp

> Aplicativo mobile desenvolvido em **Flutter** para exibir informações geoespaciais do **Círio de Nazaré** — a maior procissão católica do mundo, realizada em Belém do Pará, Brasil.

---

## 📱 Demonstração

<p align="center">
  <img width="300" alt="CírioApp Demo" src="https://github.com/user-attachments/assets/f301c447-8c5e-4f63-9ba6-17d50719a5f9" />
</p>

---

## 📋 Sobre o Projeto

O **CírioApp** é um aplicativo de mapa interativo que permite aos fiéis e participantes acompanhar as rotas oficiais do Círio de Nazaré em tempo real. Com geolocalização integrada e visualização via Google Maps, o app orienta o usuário desde a sua posição atual até os pontos centrais do evento.

Este projeto foi desenvolvido como trabalho acadêmico para a disciplina de **Desenvolvimento Mobile**.

---

## ✨ Funcionalidades

| Funcionalidade | Descrição |
|---|---|
| 🗺️ Mapa Interativo | Visualização do mapa com controles de zoom e pan |
| 📍 Ponto Inicial | Marcador fixo da Basílica de Nazaré (ponto de chegada) |
| 🚶 Rota do Círio | Exibição da rota oficial: Catedral → Basílica |
| 🌙 Rota da Trasladação | Exibição da rota da Trasladação: Basílica → Catedral |
| 📡 Geolocalização | Localização em tempo real do dispositivo do usuário |
| 🧭 Rota até o Evento | Traçado de rota entre o usuário e o ponto inicial |
| 🎯 Centralizar Mapa | Botão para recentrar o mapa na posição do usuário |

---

## 🛠️ Tecnologias Utilizadas

- **[Flutter](https://flutter.dev/)** — SDK de desenvolvimento mobile multiplataforma
- **[Dart](https://dart.dev/)** — Linguagem de programação
- **[google_maps_flutter ^2.6.0](https://pub.dev/packages/google_maps_flutter)** — Integração com Google Maps
- **[geolocator ^11.0.0](https://pub.dev/packages/geolocator)** — Acesso à localização GPS do dispositivo

---

## 🗂️ Estrutura do Projeto

```
lib/
├── core/
│   └── constants/
│       └── map_constants.dart      # Coordenadas e rotas (Basílica, Catedral, Círio, Trasladação)
│
├── features/
│   └── map/
│       ├── models/
│       │   └── evento_cirio.dart   # Modelo de dados do evento
│       │
│       ├── presentation/
│       │   ├── pages/
│       │   │   └── map_page.dart   # Tela principal do mapa
│       │   │
│       │   └── widgets/
│       │       ├── center_map_button.dart    # Botão de centralização
│       │       └── map_toggle_button.dart    # Toggle entre rotas
│       │
│       └── services/
│           └── location_service.dart         # Serviço de geolocalização
│
└── main.dart                       # Ponto de entrada da aplicação

android/
└── app/
    └── src/
        └── main/
            └── AndroidManifest.xml # Configurações e permissões Android
```

---

## 🗺️ Pontos de Referência

| Local | Latitude | Longitude |
|---|---|---|
| Basílica de Nazaré | -1.452624 | -48.476270 |
| Catedral da Sé | -1.456108 | -48.504719 |

**Rota do Círio (dia):** Catedral → Basílica  
**Rota da Trasladação (noite):** Basílica → Catedral

---

## 🚀 Como Executar

### Pré-requisitos

- [Flutter SDK](https://docs.flutter.dev/get-started/install) `^3.11.1` ou superior
- Android Studio ou VS Code com extensões Flutter/Dart
- Chave de API do [Google Maps Platform](https://developers.google.com/maps) configurada no `AndroidManifest.xml`
- Dispositivo físico ou emulador Android/iOS

### Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/lianeheidemann/Aplicativo_CirioDeNazare.git
cd Aplicativo_CirioDeNazare

# 2. Instale as dependências
flutter pub get

# 3. Execute o aplicativo
flutter run
```

> ⚠️ **Atenção:** É necessário adicionar sua chave da Google Maps API no arquivo `android/app/src/main/AndroidManifest.xml` para que o mapa seja exibido corretamente.

---

## 🔐 Permissões Necessárias

O aplicativo solicita as seguintes permissões ao usuário:

- **Localização em uso** (`ACCESS_FINE_LOCATION`) — para exibir a posição atual no mapa
- **Serviços de GPS** — verificados em tempo de execução via `Geolocator`

---

## 📦 Dependências (`pubspec.yaml`)

```yaml
dependencies:
  flutter:
    sdk: flutter
  google_maps_flutter: ^2.6.0
  geolocator: ^11.0.0
  cupertino_icons: ^1.0.8

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^6.0.0
```

---

## 🎯 Sobre o Círio de Nazaré

O **Círio de Nazaré** é a maior procissão religiosa do mundo, realizada anualmente em outubro na cidade de Belém, Pará. Milhões de fiéis acompanham a trasladação da imagem de Nossa Senhora de Nazaré pelas ruas da cidade. O evento foi reconhecido pela **UNESCO** como Patrimônio Cultural Imaterial da Humanidade.

---

## 👩‍💻 Autora

**Liane Heidemann**

Projeto acadêmico desenvolvido para a disciplina de **Desenvolvimento Mobile**.

---

## 📄 Licença

Este projeto é de uso acadêmico. Para mais informações, entre em contato com a autora.

---

<p align="center">
  Feito com ❤️ e devoção para o Círio de Nazaré 🕯️
</p>
