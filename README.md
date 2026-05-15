# CírioApp

Aplicativo mobile desenvolvido em Flutter utilizando Google Maps e geolocalização para exibir informações relacionadas ao Círio de Nazaré.

O projeto apresenta:

- Rota oficial do Círio
- Rota da Trasladação
- Localização atual do usuário
- Rota até o ponto inicial do evento

---

# Demonstração

<img width="540" height="1110" alt="cirioApp_50porcento_GIF" src="https://github.com/user-attachments/assets/36c3b695-74cb-4d5d-a7d8-9e9486aa2a1b" />



---

# Tecnologias Utilizadas

- Flutter
- Dart
- Google Maps Flutter
- Geolocator

---

# Funcionalidades

- Exibição do mapa interativo
- Marcador do ponto inicial do Círio
- Exibição da rota do Círio
- Exibição da rota da Trasladação
- Geolocalização do usuário
- Rota entre usuário e evento
- Centralização automática do mapa

---

# Estrutura do Projeto

```text
android/
└── app/
    └── src/
        └── main/
            └── AndroidManifest.xml

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

pubspec.yaml
```

---

# Como Executar

```bash
flutter pub get
flutter run
```

---

# Autor

Liane Heidemann

Projeto acadêmico desenvolvido para a disciplina de Desenvolvimento Mobile com Flutter.
