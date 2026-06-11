# CírioApp
<!-- MOBILE -->
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Google Maps](https://img.shields.io/badge/Google_Maps-4285F4?style=for-the-badge&logo=googlemaps&logoColor=white)

> Aplicativo mobile desenvolvido em **Flutter** para exibir informações geoespaciais do **Círio de Nazaré** — a maior procissão católica do mundo, realizada em Belém do Pará, Brasil.

---

## Demonstração

<p align="left">
  <img width="300" alt="CírioApp Demo" src="https://github.com/lianeheidemann/Aplicativo_CirioDeNazare/blob/main/AppCirio_GIF.gif"  width="80%"/>
</p>

---

## Sobre o App

O **CírioApp** é um aplicativo de mapa interativo que permite aos fiéis e participantes acompanhar as rotas oficiais do Círio de Nazaré em tempo real. Com geolocalização integrada e visualização via Google Maps, o app orienta o usuário desde a sua posição atual até os pontos centrais do evento.


---

## Funcionalidades

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

## Tecnologias Utilizadas

- Flutter
- Dart](https://dart.dev/)**
- google_maps_flutter 

---

## Estrutura do Projeto

```
lib/
├── core/
│   └── constants/
│       └── map_constants.dart      
│
├── features/
│   └── map/
│       ├── models/
│       │   └── evento_cirio.dart   
│       │
│       ├── presentation/
│       │   ├── pages/
│       │   │   └── map_page.dart  
│       │   │
│       │   └── widgets/
│       │       ├── center_map_button.dart   
│       │       └── map_toggle_button.dart
│       │
│       └── services/
│           └── location_service.dart
│
└── main.dart                       

android/
└── app/
    └── src/
        └── main/
            └── AndroidManifest.xml 
```

---

## Pontos de Referência

| Local | Latitude | Longitude |
|---|---|---|
| Basílica de Nazaré | -1.452624 | -48.476270 |
| Catedral da Sé | -1.456108 | -48.504719 |

**Rota do Círio (dia):** Catedral → Basílica  
**Rota da Trasladação (noite):** Basílica → Catedral

---

## Como Executar

### Pré-requisitos
- Flutter SDK `^3.11.1` ou superior
- Chave de API do [Google Maps Platform](https://developers.google.com/maps) configurada no `AndroidManifest.xml`

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

> **Atenção:** É necessário adicionar sua chave da Google Maps API no arquivo `android/app/src/main/AndroidManifest.xml` para que o mapa seja exibido corretamente.

---

## Permissões Necessárias

O aplicativo solicita as seguintes permissões ao usuário:

- **Localização em uso** (`ACCESS_FINE_LOCATION`) — para exibir a posição atual no mapa
- **Serviços de GPS** — verificados em tempo de execução via `Geolocator`

---

## Dependências (`pubspec.yaml`)

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

