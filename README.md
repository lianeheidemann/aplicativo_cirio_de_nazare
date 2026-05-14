# Círio Map

Aplicativo mobile desenvolvido em Flutter utilizando Google Maps e geolocalização para exibir informações relacionadas ao Círio de Nazaré.

O projeto apresenta:

- Rota oficial do Círio
- Rota da Trasladação
- Localização atual do usuário
- Rota até o ponto inicial do evento

---

# Demonstração

<p align="center">
  <img src="https://github.com/user-attachments/assets/4f567b2f-74dc-48b8-a548-dc188ac9dac1" width="250"/>

  <img src="https://github.com/user-attachments/assets/132b1e6f-7b2f-4337-9b2d-004b5b75a997" width="250"/>
</p>

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
lib/
│
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

```text

