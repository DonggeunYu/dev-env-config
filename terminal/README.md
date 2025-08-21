# Terminal 환경 세팅 가이드 (Mac)

이 가이드는 Mac에서 **Kitty 터미널, zsh, Powerlevel10k, Hack Nerd Font**를 설치하고 바로 사용할 수 있도록 최소 단계로 정리한 가이드입니다.

---

## 1. Kitty 터미널

#### 1. Hack Nerd Font 다운로드 & 설치
- [Hack Font Releases](https://github.com/source-foundry/Hack/releases)  
- 원하는 `.ttf` 파일 다운로드 → 더블클릭 후 **Font Book**에 설치

#### 2. Kitty 설치
- [Kitty Releases](https://github.com/kovidgoyal/kitty/releases)  

설치 후 설정 파일 복사:
~~~bash
mkdir -p ~/.config/kitty
cp kitty.conf ~/.config/kitty/kitty.conf
~~~

#### 3. 폰트 확인
~~~bash
kitty +list-fonts | grep "Hack"
~~~
설치된 폰트가 목록에 보이면 OK


## 2. Oh My Zsh + Powerlevel10k
#### 1. Oh My Zsh 설치 (설치되어 있지 않은 경우)
~~~bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
~~~

#### 2. Powerlevel10k 다운로드
~~~bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
~~~

#### 3. 설정 파일 복사
~~~bash
cp .p10k.zsh ~/.p10k.zsh
cp .zshrc ~/.zshrc
~~~

#### 4. 적용
~~~bash
source ~/.zshrc
~~~