# 🎓 Zespół Szkół Elektrycznych i Licealnych w Opolu

<div align="center">

[![License](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-Powered-326CE5?logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![GitOps](https://img.shields.io/badge/GitOps-ArgoCD-EF7B4D?logo=argo&logoColor=white)](https://argo-cd.readthedocs.io/)
[![Infrastructure as Code](https://img.shields.io/badge/IaC-Terraform-7B42BC?logo=terraform&logoColor=white)](https://www.terraform.io/)

**Nowoczesna infrastruktura edukacyjna oparta na Open Source**

[🌐 Website](https://zsel.opole.pl) • [📧 Contact](mailto:kontakt@zsel.opole.pl) • [🤝 Contribute](#contributing)

</div>

---

## 📖 O nas

Zespół Szkół Elektrycznych i Licealnych w Opolu to nowoczesna placówka edukacyjna, która łączy tradycyjne wykształcenie zawodowe z najnowszymi technologiami informatycznymi. Nasza misja to przygotowanie uczniów do wyzwań cyfrowej przyszłości poprzez praktyczne doświadczenie z technologiami używanymi w przemyśle.

### 🎯 Nasza wizja

- **Edukacja przez praktykę** – uczniowie uczą się na rzeczywistej infrastrukturze
- **Open Source first** – promujemy wolne oprogramowanie i otwarte standardy
- **Cloud Native** – przygotowujemy do pracy z nowoczesnymi architekturami
- **DevOps culture** – automatyzacja, CI/CD, Infrastructure as Code
- **Security by design** – bezpieczeństwo wbudowane w każdy proces

---

## 🛠️ Stack technologiczny

Nasza infrastruktura wykorzystuje sprawdzone technologie open source:

### 🐳 Orchestration & Automation
- **Kubernetes (K3s)** – orkiestracja kontenerów
- **ArgoCD** – GitOps continuous delivery
- **Terraform** – Infrastructure as Code dla infrastruktury
- **Ansible** – automatyzacja konfiguracji

### 📊 Observability
- **Prometheus & Grafana** – monitoring i wizualizacja metryk
- **Loki** – centralne logowanie
- **AlertManager** – zarządzanie alertami
- **Zabbix** – monitoring infrastruktury sieciowej

### 🔒 Security
- **Sealed Secrets** – bezpieczne zarządzanie sekretami w GitOps
- **Trivy & Falco** – skanowanie bezpieczeństwa kontenerów
- **OPA (Open Policy Agent)** – policy enforcement
- **WireGuard VPN** – bezpieczny dostęp zdalny
- **Zero Trust Network** – NetworkPolicies dla każdej aplikacji

### 🎓 Educational Services
- **Moodle** – platforma e-learningowa
- **NextCloud** – chmura plików i współpraca
- **JupyterHub** – interaktywne środowisko programistyczne
- **GitLab** – hosting kodu, CI/CD dla projektów uczniowskich

### 🌐 Network & Infrastructure
- **MikroTik RouterOS** – infrastruktura sieciowa
- **Terraform MikroTik Provider** – automatyzacja konfiguracji sieci
- **FreeIPA** – centralne zarządzanie tożsamościami
- **Bind9** – własne serwery DNS

---

## 📁 Repozytoria

Nasze repozytoria są zorganizowane według funkcji:

| Repository | Opis |
|------------|------|
| **`zsel-eip-infra`** | Podstawowa infrastruktura Kubernetes (Terraform) |
| **`zsel-eip-gitops`** | Aplikacje wdrażane przez ArgoCD |
| **`zsel-eip-network`** | Konfiguracja infrastruktury sieciowej (MikroTik) |
| **`zsel-eip-ansible`** | Automatyzacja konfiguracji (Ansible playbooks) |
| **`zsel-eip-dokumentacja`** | Dokumentacja architektury i procesów |
| **`zsel-opole-ad`** | Active Directory integration |

---

## 🤝 Contributing

Zapraszamy do współpracy! Każdy pull request jest mile widziany.

### 📋 Zasady kontrybuowania

1. **Fork & Clone** – stwórz fork repozytorium i sklonuj go lokalnie
2. **Branch** – twórz branch dla swojej feature/fix (`feature/amazing-feature`)
3. **Code** – pisz kod zgodnie z naszymi standardami
4. **Test** – upewnij się, że wszystkie testy przechodzą
5. **Commit** – używaj [Conventional Commits](https://www.conventionalcommits.org/)
6. **Push** – wypchnij zmiany do swojego forka
7. **Pull Request** – stwórz PR z opisem zmian

### ✅ Standards

- **Infrastructure as Code:** Wszystkie zmiany przez Terraform/Ansible
- **GitOps:** Aplikacje wdrażane tylko przez ArgoCD
- **Security:** Scanowanie przed merge (Trivy, kubesec, OPA)
- **Documentation:** Każda zmiana wymaga update dokumentacji
- **Testing:** Minimum 80% code coverage
- **Code Review:** 2 approvals required (DevOps + Security)

### 📝 Conventional Commits

```
feat: Add new Moodle plugin integration
fix: Resolve FreeIPA authentication issue
docs: Update GitOps deployment guide
chore: Upgrade Prometheus to v2.50
security: Patch CVE-2024-1234 in NextCloud
```

---

## 🔐 Security

Bezpieczeństwo jest naszym priorytetem. Jeśli znajdziesz lukę bezpieczeństwa:

1. **NIE twórz** publicznego issue
2. Wyślij email na: **security@zsel.opole.pl**
3. Zawrzyj szczegółowy opis problemu
4. Damy Ci znać w ciągu 48 godzin

### 🛡️ Security Features

- **Network Segmentation:** Pełna segmentacja VLAN, firewall rules
- **Zero Trust:** NetworkPolicies dla każdej aplikacji (deny-all default)
- **RBAC:** Role-Based Access Control w Kubernetes
- **Sealed Secrets:** Encrypted secrets w GitOps workflow
- **Image Scanning:** Automatyczne skanowanie CVE (Trivy, Falco)
- **Compliance:** RODO/GDPR compliance checks w CI/CD
- **Audit Logging:** Pełny audit trail wszystkich operacji

---

## 📚 Dokumentacja

Główna dokumentacja znajduje się w repozytorium **`zsel-eip-dokumentacja`**:

- 📘 **Architektura** – diagramy, topology, network design
- 📙 **Deployment** – procedury wdrożeniowe, runbook
- 📗 **Security** – polityki bezpieczeństwa, hardening guides
- 📕 **Operations** – monitoring, troubleshooting, incident response

---

## 🌟 Dla uczniów

### 🎓 Praktyki i projekty

Jesteś uczniem ZSEL i chcesz się zaangażować? Sprawdź:

- **Projekty uczniowskie** w GitLab ([gitlab.zsel.opole.pl](https://gitlab.zsel.opole.pl))
- **JupyterHub** – programowanie w Python, Data Science
- **Moodle** – kursy online z Kubernetes, Docker, Linux
- **Praktyki DevOps** – współpraca przy prawdziwej infrastrukturze

### 🚀 Co możesz się nauczyć?

- **Kubernetes & Docker** – orkiestracja kontenerów
- **GitOps & CI/CD** – automatyzacja wdrożeń
- **Infrastructure as Code** – Terraform, Ansible
- **Monitoring & Logging** – Prometheus, Grafana, Loki
- **Network Engineering** – MikroTik, VLANs, routing, firewalle
- **Security** – CVE scanning, secrets management, Zero Trust

---

## 📞 Kontakt

**Zespół Szkół Elektrycznych i Licealnych w Opolu**

- 🌐 Website: [zsel.opole.pl](https://zsel.opole.pl)
- 📧 Email: [kontakt@zsel.opole.pl](mailto:kontakt@zsel.opole.pl)
- 🔧 IT Team: [it@zsel.opole.pl](mailto:it@zsel.opole.pl)
- 🛡️ Security: [security@zsel.opole.pl](mailto:security@zsel.opole.pl)

### 👥 Zespół DevOps

| Rola | Kontakt |
|------|---------|
| **DevOps Lead** | devops@zsel.opole.pl |
| **Security Officer** | security@zsel.opole.pl |
| **Network Admin** | network@zsel.opole.pl |

---

## 📜 Licencja

Większość naszych projektów jest dostępna na licencji **GPL-3.0**, chyba że zaznaczono inaczej w konkretnym repozytorium.

```
Copyright (C) 2024-2025 Zespół Szkół Elektrycznych i Licealnych w Opolu

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License.
```

---

## 🙏 Acknowledgments

Dziękujemy społeczności Open Source za narzędzia, które umożliwiają nasze projekty:

- [Kubernetes](https://kubernetes.io/) & [K3s](https://k3s.io/)
- [ArgoCD](https://argo-cd.readthedocs.io/)
- [Terraform](https://www.terraform.io/)
- [Ansible](https://www.ansible.com/)
- [MikroTik](https://mikrotik.com/)
- [Prometheus](https://prometheus.io/) & [Grafana](https://grafana.com/)
- Oraz wszystkim kontrybutorów open source! ❤️

---

<div align="center">

**Zbudowane z ❤️ przez zespół DevOps ZSEL Opole**

[⬆ Powrót na górę](#-zespół-szkół-elektrycznych-i-licealnych-w-opolu)

</div>
