# Joje's Blog

Jekyll과 GitHub Pages로 운영하는 개인 블로그 저장소입니다.

**블로그 바로가기:** [https://joje3029.github.io/](https://joje3029.github.io/)

## 이 저장소에 포함된 것

- **Jekyll** 설정과 포스트·페이지 소스 (`_config.yml`, `_posts/`, `_pages/` 등)
- **GitHub Pages** 배포용 구성 (`Gemfile`의 `github-pages` 등)
- 테마는 저장소에 복사하지 않고 **remote theme**으로 불러옵니다: [`mmistakes/minimal-mistakes`](https://github.com/mmistakes/minimal-mistakes) (`_config.yml`의 `remote_theme`)

원래 Minimal Mistakes 저장소의 “starter” 템플릿을 기반으로 시작했을 수 있지만, 지금은 위 파일들이 **이 블로그를 빌드·배포하는 데 필요한 본 저장소**입니다. 샘플 포스트를 지우고 글만 바꿔도 되고, 사이드바·플러그인은 `_config.yml`에서 조정하면 됩니다.

## 로컬에서 미리보기

1. [Ruby](https://www.ruby-lang.org/)와 [Bundler](https://bundler.io/)를 설치합니다.
2. 저장소를 클론한 뒤 프로젝트 루트로 이동합니다.
3. 의존성을 설치합니다.

   ```bash
   bundle install
   ```

4. 로컬 서버를 띄웁니다.

   ```bash
   bundle exec jekyll serve
   ```

5. 브라우저에서 **http://localhost:4000** 으로 접속합니다.

`github-pages` 젬을 쓰고 있으므로, 로컬에서도 GitHub Pages와 비슷한 환경으로 빌드되는 편입니다. `_config.yml`을 수정한 뒤에는 서버를 한 번 재시작해야 반영되는 항목이 있습니다.

### Windows에서만 참고

macOS·Linux와 달리 **Windows에는 Ruby가 기본 설치되어 있지 않습니다.** 위 1번을 진행하려면 [Ruby+Devkit (RubyInstaller)](https://rubyinstaller.org/downloads/)를 쓰거나, **[WSL2](https://learn.microsoft.com/ko-kr/windows/wsl/install)** 안의 Linux에서 같은 절차를 따르는 방법이 일반적입니다. 네이티브 Windows에서 Ruby 환경을 맞추는 과정이 번거롭다면, **푸시 후 GitHub Pages 빌드 결과로 확인**해도 됩니다. 이 저장소 `Gemfile`에는 Windows에서 파일 변경 감지를 돕는 `wdm` 젬이 포함되어 있습니다.

## 참고

- 테마 옵션·레이아웃: [Minimal Mistakes 문서](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)
- Jekyll 일반: [Jekyll 공식 문서](https://jekyllrb.com/docs/)
