[evgenii-landing-with-photo.html](https://github.com/user-attachments/files/26547164/evgenii-landing-with-photo.html)
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <title>Евгений Шелковый — лендинг-визитка</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg1: #020817;
      --bg2: #071425;
      --card: rgba(8, 18, 38, 0.72);
      --card-border: rgba(120, 190, 255, 0.16);
      --text-main: #f8fbff;
      --text-muted: rgba(223, 235, 255, 0.72);
      --button-bg: #0a0f18;
      --button-hover: #10192a;
      --button-border: rgba(111, 197, 255, 0.18);
      --transition-fast: 0.18s ease-out;
    }
    * { box-sizing: border-box; margin: 0; padding: 0; }
    html, body { height: 100%; }
    body {
      font-family: "Inter", system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      color: var(--text-main);
      -webkit-font-smoothing: antialiased;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 18px;
      background:
        radial-gradient(circle at top, rgba(61, 155, 255, 0.24), transparent 34%),
        radial-gradient(circle at center, rgba(102, 217, 255, 0.09), transparent 28%),
        linear-gradient(180deg, var(--bg1) 0%, var(--bg2) 100%);
      overflow: hidden;
    }
    body::before {
      content: "";
      position: fixed;
      inset: 0;
      background:
        radial-gradient(circle at 20% 20%, rgba(102, 217, 255, 0.13), transparent 16%),
        radial-gradient(circle at 80% 18%, rgba(76, 132, 255, 0.12), transparent 18%),
        radial-gradient(circle at 70% 78%, rgba(102, 217, 255, 0.08), transparent 22%);
      pointer-events: none;
    }
    .page {
      width: 100%;
      max-width: 480px;
      background: linear-gradient(180deg, rgba(12, 24, 45, 0.82), rgba(7, 16, 32, 0.86));
      border: 1px solid var(--card-border);
      border-radius: 28px;
      box-shadow: 0 22px 60px rgba(0, 0, 0, 0.38);
      padding: 42px 24px 28px;
      text-align: center;
      backdrop-filter: blur(12px);
      opacity: 0;
      transform: translateY(12px);
      animation: fadeInUp 0.75s var(--transition-fast) forwards;
    }
    .logo {
      width: 128px;
      height: 128px;
      border-radius: 50%;
      margin: 0 auto 22px;
      overflow: hidden;
      border: 1px solid rgba(102, 217, 255, 0.18);
      box-shadow: 0 10px 24px rgba(0,0,0,0.22);
      opacity: 0;
      transform: translateY(10px);
      animation: fadeInUp 0.75s var(--transition-fast) forwards;
      animation-delay: 0.08s;
    }
    .logo img { width: 100%; height: 100%; object-fit: cover; display: block; }
    .name {
      font-size: 22px;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      margin-bottom: 14px;
      opacity: 0;
      transform: translateY(8px);
      animation: fadeInUp 0.75s var(--transition-fast) forwards;
      animation-delay: 0.14s;
    }
    .subtitle {
      font-size: 15px;
      line-height: 1.58;
      color: var(--text-muted);
      white-space: pre-line;
      margin-bottom: 28px;
      opacity: 0;
      transform: translateY(8px);
      animation: fadeInUp 0.75s var(--transition-fast) forwards;
      animation-delay: 0.2s;
    }
    .buttons {
      display: flex;
      flex-direction: column;
      gap: 12px;
      opacity: 0;
      transform: translateY(8px);
      animation: fadeInUp 0.75s var(--transition-fast) forwards;
      animation-delay: 0.26s;
    }
    .btn {
      display: block;
      width: 100%;
      padding: 14px 18px;
      border-radius: 12px;
      border: 1px solid var(--button-border);
      background: linear-gradient(180deg, var(--button-bg), #050912);
      color: var(--text-main);
      text-decoration: none;
      font-size: 15px;
      font-weight: 500;
      letter-spacing: 0.04em;
      cursor: pointer;
      transition: transform var(--transition-fast), box-shadow var(--transition-fast), background-color var(--transition-fast), border-color var(--transition-fast);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.22);
    }
    .btn:hover, .btn:focus-visible {
      background: linear-gradient(180deg, var(--button-hover), #0d1422);
      transform: translateY(-2px);
      box-shadow: 0 16px 30px rgba(0, 0, 0, 0.32);
      outline: none;
      border-color: rgba(102, 217, 255, 0.28);
    }
    .btn:active { transform: translateY(0px); }
    @keyframes fadeInUp { from { opacity: 0; transform: translateY(16px); } to { opacity: 1; transform: translateY(0); } }
    @media (min-width: 768px) {
      body { padding: 32px; }
      .page { padding: 46px 42px 34px; }
      .name { font-size: 24px; }
      .subtitle { font-size: 16px; }
    }
  </style>
</head>
<body>
  <main class="page">
    <div class="logo">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSCMcroMNhKOw9lnXuls7SGkyNWmAuIbxhElw&s" alt="Фото" />
    </div>
    <h1 class="name">ЕВГЕНИЙ ШЕЛКОВЫЙ</h1>
    <p class="subtitle">Серийный предприниматель
30+ проектов
Эксперт по созданию экстра-команд
IT овнер GetProfi.me</p>
    <div class="buttons">
      <a class="btn" href="https://t.me/Evgenii_Shelkoviy" target="_blank" rel="noopener noreferrer">Telegram</a>
      <a class="btn" href="https://getprofi.lovable.app/" target="_blank" rel="noopener noreferrer">GetProFi.me</a>
    </div>
  </main>
</body>
</html>
