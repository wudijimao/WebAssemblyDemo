# Mac电脑环境配置方法
## 1.安装rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
## 2.安装wasm-pack
cargo install wasm-pack

# 编译方法
wasm-pack build --target web

# 验证方法
npx http-server  
这个命令将在当前目录下启动一个本地服务器，并将当前目录作为服务器的根目录。然后，你可以通过 http://localhost:8080/test.html 访问 HTML 文件