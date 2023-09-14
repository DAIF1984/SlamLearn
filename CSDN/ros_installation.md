
```markdown
# 在 Ubuntu 20.04 上安装 ROS Noetic

## 1. 设置软件源

```bash
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros-latest.list'
```

## 2. 添加 ROS GPG key

```bash
sudo apt install curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
```

## 3. 更新软件包列表

```bash
sudo apt update
```

## 4. 安装 ROS Noetic

### 安装完整版

```bash
sudo apt install ros-noetic-desktop-full
```

### 或者安装基础版

```bash
sudo apt install ros-noetic-desktop
```

## 5. 初始化 rosdep

```bash
sudo rosdep init
rosdep update
```

## 6. 设置环境变量

```bash
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

（如果你使用 zsh，请将 `.bashrc` 替换为 `.zshrc`）

## 7. 安装额外工具（可选）

```bash
sudo apt install python3-rosinstall
```

现在你已经成功在 Ubuntu 20.04 上安装了 ROS Noetic，可以开始进行你的 ROS 项目了！如果需要任何额外的帮助，欢迎随时询问！
```

