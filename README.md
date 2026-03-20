# secure-dns-waf-ansible

온프레미스 환경에서 DNS, WAF, 보안 서버 구성을 자동화하기 위해
Ansible을 활용하여 구축한 인프라 코드입니다.

## 📌 주요 기능

- WAF(ModSecurity) 설치 및 설정 자동화
- Nginx/Apache 웹 서버 구성 자동화
- DNS 서버 설정 자동화
- 보안 정책 적용 및 서비스 복구 자동화

## 🧑‍💻 담당 역할

- 보안 / 네트워크 담당
- WAF 구성 및 룰 적용 자동화
- 방화벽 정책 및 트래픽 흐름 제어
- Ansible Playbook 및 Role 설계

## 🛠 기술 스택

- Ansible
- Linux (Rocky Linux)
- WAF (ModSecurity, OWASP CRS)
- Web Server (Apache / Nginx)

## 📂 디렉토리 구조

- `inventory/` : 대상 서버 정의
- `group_vars/` : 변수 설정
- `roles/` : 서비스 구성 (WAF, DNS 등)
- `playbooks/` : 실행 스크립트

## 🚀 실행 방법

```bash
ansible-playbook -i inventory/hosts playbooks/site.yml
