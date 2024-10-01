# SOON-Development-Environment

 Codespaces üzerinden veya VPS üzerinden yapabilirsiniz


      curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y

      rustc --version
      
  ÇIKTI  rustc 1.81.0 (eeb90cda1 2024-09-04) Olmalı

     rustup default 1.79.0 
 
 1.79.0  Dönmemizin sebebi 1.81.0 de hata veriyor
 
     sh -c "$(curl -sSfL https://release.anza.xyz/v2.0.3/install)"
     export PATH="$HOME/.local/share/solana/install/active_release/bin:$PATH"
     sudo apt install gcc


     cargo install --git https://github.com/coral-xyz/anchor avm --force
     avm install latest
     avm use latest
     
     curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/master/install.sh | bash
     
     export NVM_DIR="$HOME/.nvm"
     [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
     [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

     command -v nvm
     nvm install node
     npm install -g yarn
     npm install -g pnpm


     solana config set --url https://rpc.devnet.soo.network/rpc
     solana config get


   Sıfırdan Cüzdan Oluşturmak İçin
      
      solana-keygen new

  Eski Cüzdan için

      solana-keygen recover prompt://?key=0/0

 İşlemlere Devam

      git clone https://github.com/soonlabs/hello-world
      cd hello-world
      cd example-hello-world/src/program-rust
      cargo build-sbf
      solana config set --url https://rpc.devnet.soo.network/rpc
      solana program deploy ./target/deploy/helloworld.so

 https://explorer.devnet.soo.network/ Sitesi Üzerinden Signature koplayaıp tx ine bakabilirsiniz
