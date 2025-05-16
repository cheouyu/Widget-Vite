網址：https://widget-vite-two.vercel.app/

# Vite + React 项目

## 组件使用说明

### Toast 通知组件

项目使用 `react-toastify` 来实现通知功能。

1. 在组件中引入：

```jsx
import { toast, ToastContainer } from "react-toastify";
```

2. 在组件中使用 ToastContainer：

```jsx
<ToastContainer
  position="bottom-right"
  autoClose={5000}
  hideProgressBar={false}
  newestOnTop={false}
  closeOnClick={false}
  rtl={false}
  pauseOnFocusLoss
  draggable
  pauseOnHover
  theme="dark"
  style={{ zIndex: 9999999999 }}
/>
```

3. 调用通知：

```jsx
toast("这是一条通知消息");
```

### MetaCRM Widget

项目集成了 MetaCRM Widget 用于客户关系管理。

1. Widget 已在 `index.html` 中自动加载和初始化
2. 配置参数：

   - apiKey: "*********"
   - autoOpenNewNotification: true
   - manualConnect: true
   - MetaCRMWidgetExecutionEnvironment: "dev"

## 开发环境设置

1. 安装依赖：

```bash
npm install
```

2. 启动开发服务器：

```bash
npm run dev
```

3. 构建生产版本：

```bash
npm run build
```
