# Obywatel BIELIK Infra

Repozytorium zawierające konfigurację infrastruktury i pliki wdrożeniowe dla projektu Obywatel BIELIK.

## Opis projektu

Obywatel BIELIK to aplikacja służąca do gromadzenia opisów zdjęć (anotacji) przez społeczność, w tym seniorów i lokalnych aktywistów. To repozytorium zawiera definicje infrastruktury jako kodu, konfiguracje środowisk i skrypty wdrożeniowe.

## Struktura projektu

```
obywatel-bielik-infra/
├── terraform/                   # Infrastruktura jako kod (Terraform)
│   ├── modules/                 # Moduły Terraform
│   │   ├── database/            # Konfiguracja bazy danych
│   │   ├── kubernetes/          # Klaster Kubernetes
│   │   ├── storage/             # Przechowywanie plików
│   │   └── networking/          # Konfiguracja sieci
│   ├── environments/            # Konfiguracje środowisk
│   │   ├── development/         # Środowisko deweloperskie
│   │   ├── staging/             # Środowisko testowe
│   │   └── production/          # Środowisko produkcyjne
│   └── variables.tf             # Wspólne zmienne
├── kubernetes/                  # Konfiguracja Kubernetes
│   ├── manifests/               # Pliki manifestów
│   │   ├── api/                 # Manifesty dla backendu
│   │   ├── web/                 # Manifesty dla frontendu webowego
│   │   └── database/            # Manifesty dla bazy danych
│   ├── helm-charts/             # Wy
