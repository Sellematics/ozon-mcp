# Ozon MCP — аналитика Ozon в AI-ассистенте | Sellmonitor

**Ozon MCP от Sellmonitor** подключает аналитику маркетплейса Ozon к ChatGPT (Codex), Cursor, VS Code, Claude Code и другим AI-ассистентам. Исследуйте рынок и конкурентов или анализируйте продажи, расходы и прибыль собственного магазина прямо в чате.

[Русский](#русский) · [English](#english)

**Remote MCP** · **Streamable HTTP** · **OAuth** · **Внешняя и внутренняя аналитика Ozon**

[Получить 3 дня бесплатно](https://sellmonitor.com/?promoCode=MCP) · [Инструкция по внешней аналитике](https://sellmonitor.com/mcp/analytics/instructions) · [Инструкция по внутренней аналитике](https://sellmonitor.com/mcp/inner-analytics/instructions)

---

## Русский

### Sellmonitor MCP для Ozon: рынок и ваш магазин

MCP (Model Context Protocol) позволяет AI-ассистенту запрашивать актуальные данные Sellmonitor и использовать их в ответах. Для аналитики Ozon доступны два независимых сервера.

#### `sellmonitor_analytics` — внешняя аналитика Ozon

Исследует рынок Ozon: конкурентов, категории, ниши, бренды, продавцов, товары, поисковые запросы, цены и тренды.

`https://sellmonitor.com/mcp/sellmonitor`

#### `sellmonitor_inner_analytics` — внутренняя аналитика магазина

Работает с вашими данными на Ozon: продажами, заказами, возвратами, расходами, остатками, прибылью и финансовыми отчётами.

`https://sellmonitor.com/mcp/inner-analytics`

> [!TIP]
> Подключите оба MCP: внешний объяснит, что происходит на рынке Ozon, а внутренний — что происходит именно в вашем магазине и почему меняется его прибыль.

> [!IMPORTANT]
> Оба сервера работают через OAuth. Пароль, идентификатор пользователя и токены Sellmonitor вручную указывать не нужно.

> [!NOTE]
> **Доступ к подписке Sellmonitor бесплатно на 3 дня.** Используйте промокод **`MCP`** — карта не требуется. [Получить доступ](https://sellmonitor.com/?promoCode=MCP).

**Навигация:** [внешняя аналитика](#внешняя-аналитика-ozon) · [внутренняя аналитика](#внутренняя-аналитика-ozon) · [подключение](#быстрое-подключение) · [решение проблем](#если-mcp-не-подключается)

### Внешняя аналитика Ozon

Внешний MCP даёт AI-ассистенту доступ к данным рынка, а не к кабинету конкретного продавца. С его помощью можно:

- исследовать категории и перспективные ниши;
- находить и сравнивать товары, бренды и продавцов;
- анализировать продажи, выручку, цены, рейтинг, отзывы и остатки;
- оценивать динамику рынка за выбранный период;
- изучать ценовые сегменты и конкурентность ниши;
- анализировать поисковые запросы покупателей;
- смотреть позиции товара в поисковых запросах и источники его обнаружения;
- получать описание и отзывы товара для SEO-анализа карточки.

Примеры запросов:

- «Используй Sellmonitor MCP и найди топ товаров на Ozon в категории роботов-пылесосов за последний месяц».
- «Найди перспективные товары для продажи на Ozon в новогодний период 2026 года».
- «Сравни бренды в категории и покажи, у кого быстрее всего растёт выручка».
- «Проанализируй ценовые сегменты категории и найди сегмент с растущим спросом и умеренной конкуренцией».
- «Найди продавцов Ozon, которые быстрее рынка растут в этой категории».
- «Какие поисковые запросы в этой нише имеют высокий спрос, но относительно небольшое число товаров?»

### Внутренняя аналитика Ozon

Внутренний MCP работает с данными ваших магазинов, подключённых к Sellmonitor. AI-ассистент видит только кабинеты, доступные вашему аккаунту.

Он помогает анализировать:

- продажи и заказы;
- комиссии, логистику, хранение и другие расходы;
- возвраты и обратную логистику;
- себестоимость, прибыль и маржинальность;
- текущие остатки;
- полноту загрузки данных;
- расходы, которые были загружены позже самой продажи.

Примеры запросов:

- «Почему по товару с артикулом 12345 прибыль за август отрицательная? Разложи расходы по статьям».
- «Покажи товары Ozon без продаж за последние 30 дней, у которых сейчас есть остатки».
- «Проверь, полностью ли загрузились данные Ozon за вчера».
- «Найди товары, у которых выручка растёт, а прибыль или маржинальность падает. Объясни причину по каждому».
- «Найди аномальные дни, когда комиссия, логистика или хранение резко выросли. Покажи товары и заказы, которые дали скачок».
- «Какие товары приносят больше всего потерь на возвратах и обратной логистике?»
- «Почему прибыль по товару изменилась после обновления данных? Покажи, какие расходы пришли позже продажи».
- «Если нужно улучшить прибыль в следующем месяце, какие три проблемы стоит исправить в первую очередь? Подтверди выводы цифрами».

### Быстрое подключение

Перед подключением войдите в [Sellmonitor](https://sellmonitor.com/) в браузере по умолчанию. У аккаунта должен быть активный доступ к Ozon.

#### ChatGPT (Codex)

Основной способ подключения — через интерфейс приложения ChatGPT:

1. Переключитесь в режим **Codex**. В обычном режиме ChatGPT подключённые MCP использоваться не будут.
2. Откройте **Настройки → Плагины → MCP**.
3. Нажмите **Добавить → Добавить сервер MCP**.
4. Выберите транспорт **Streamable HTTP**.
5. Добавьте нужный сервер или оба сервера:

   ```text
   Name: sellmonitor_analytics
   URL: https://sellmonitor.com/mcp/sellmonitor
   Bearer token: оставить пустым
   Headers: оставить пустым
   ```

   ```text
   Name: sellmonitor_inner_analytics
   URL: https://sellmonitor.com/mcp/inner-analytics
   Bearer token: оставить пустым
   Headers: оставить пустым
   ```

6. Сохраните настройки и нажмите **Перезапустить**.
7. В списке MCP-серверов нажмите **Авторизовать** и подтвердите подключение к аккаунту Sellmonitor в браузере.
8. Вернитесь в чат в режиме Codex. Проверить подключение можно командой `/mcp`.

Если кнопка **Авторизовать** не срабатывает, временно отключите VPN перед нажатием. Завершите авторизацию в браузере, после чего VPN можно включить снова.

Альтернатива для Codex CLI:

```bash
codex mcp add sellmonitor_analytics --url https://sellmonitor.com/mcp/sellmonitor
codex mcp login sellmonitor_analytics

codex mcp add sellmonitor_inner_analytics --url https://sellmonitor.com/mcp/inner-analytics
codex mcp login sellmonitor_inner_analytics
```

#### Cursor

Откройте настройки MCP или **Tools & Integrations** и добавьте конфигурацию:

```json
{
  "mcpServers": {
    "sellmonitor_analytics": {
      "url": "https://sellmonitor.com/mcp/sellmonitor"
    },
    "sellmonitor_inner_analytics": {
      "url": "https://sellmonitor.com/mcp/inner-analytics"
    }
  }
}
```

Сохраните конфигурацию и нажмите **Connect** или **Login**. Cursor откроет OAuth-страницу Sellmonitor.

#### VS Code

1. Откройте Command Palette и выберите `MCP: Add Server`.
2. Выберите HTTP / Server-Sent Events.
3. Добавьте URL внешнего или внутреннего MCP.
4. Укажите техническое имя сервера.
5. Через `MCP: List Servers` запустите сервер и завершите OAuth-авторизацию.

#### Claude Code

```bash
claude mcp add --transport http --scope user sellmonitor_analytics https://sellmonitor.com/mcp/sellmonitor
claude mcp add --transport http --scope user sellmonitor_inner_analytics https://sellmonitor.com/mcp/inner-analytics
```

OAuth-вход должен открыться автоматически. Если этого не произошло, выполните `/mcp` внутри Claude Code и выберите авторизацию нужного сервера.

### Если MCP не подключается

- Проверьте URL и обновите список MCP-серверов или перезапустите клиент.
- Убедитесь, что вы вошли в правильный аккаунт Sellmonitor в браузере по умолчанию.
- Проверьте активную подписку и доступ к Ozon.
- Не вставляйте пароль, токен или ID пользователя в настройки MCP.
- Если ассистент отвечает без данных, напишите явно: «Используй Sellmonitor MCP» или «Используй Sellmonitor MCP внутренней аналитики».

Подробные инструкции: [внешняя аналитика](https://sellmonitor.com/mcp/analytics/instructions) · [внутренняя аналитика](https://sellmonitor.com/mcp/inner-analytics/instructions)

---

## English

### Ozon MCP for market and seller analytics

Sellmonitor MCP connects current Ozon analytics to ChatGPT (Codex), Cursor, VS Code, Claude Code, and other AI assistants. Model Context Protocol lets the assistant query Sellmonitor data and use it directly in its answers. Two independent servers are available.

#### `sellmonitor_analytics` — Ozon market analytics

Research the Ozon market: competitors, categories, niches, brands, sellers, products, shopper queries, prices, and trends.

`https://sellmonitor.com/mcp/sellmonitor`

#### `sellmonitor_inner_analytics` — Ozon seller analytics

Analyze your own Ozon business: sales, orders, returns, expenses, inventory, profit, margin, and financial reports.

`https://sellmonitor.com/mcp/inner-analytics`

> [!TIP]
> Connect both servers: market analytics explains what is happening across Ozon, while seller analytics explains what is happening in your own store and why its profit changes.

> [!IMPORTANT]
> Both servers use OAuth. You do not need to paste your Sellmonitor password, user ID, or access token into an MCP client.

> [!NOTE]
> **Get three days of Sellmonitor access for free.** Use promo code **`MCP`** — no payment card is required. [Get access](https://sellmonitor.com/?promoCode=MCP).

**Navigate:** [market analytics](#ozon-market-analytics) · [seller analytics](#ozon-seller-analytics) · [setup](#quick-setup) · [troubleshooting](#troubleshooting)

### Ozon market analytics

The market analytics MCP provides market-wide data rather than private seller-cabinet data. It can help you:

- research categories and promising niches;
- find and compare products, brands, and sellers;
- analyze sales, revenue, prices, ratings, reviews, and inventory;
- evaluate market trends over a selected period;
- compare price segments and niche competition;
- analyze shopper search queries;
- inspect product positions in search queries and discovery sources;
- use product descriptions and reviews for listing SEO analysis.

Example prompts:

- “Use Sellmonitor MCP to find the top robot vacuum products on Ozon over the last month.”
- “Find promising products to sell on Ozon during the 2026 holiday season.”
- “Compare brands in this category and show which ones have the fastest revenue growth.”
- “Analyze the category's price segments and find one with growing demand and moderate competition.”
- “Find Ozon sellers that are growing faster than the rest of this category.”
- “Which shopper queries in this niche have high demand but a relatively low number of competing products?”

### Ozon seller analytics

The seller analytics MCP works with your stores connected to Sellmonitor. The AI assistant can access only the seller accounts available to your Sellmonitor user.

It can analyze:

- sales and orders;
- commissions, logistics, storage, and other expenses;
- returns and reverse logistics;
- cost of goods, profit, and margin;
- current inventory;
- data import completeness;
- expenses reported after the original sale.

Example prompts:

- “Why was profit negative for SKU 12345 in August? Break down all expenses.”
- “Show Ozon products with no sales during the last 30 days that still have inventory.”
- “Check whether yesterday's Ozon data was imported completely.”
- “Find products whose revenue is growing while profit or margin is falling. Explain the reason for each product.”
- “Find anomalous days when commission, logistics, or storage costs increased sharply. Show the products and orders behind each spike.”
- “Which products generate the largest losses from returns and reverse logistics?”
- “Why did a product's profit change after a data refresh? Show which expenses arrived after the sale.”
- “What are the top three issues we should fix next month to improve profit? Support the recommendations with numbers.”

### Quick setup

Before connecting, sign in to [Sellmonitor](https://sellmonitor.com/) in your default browser. Your account must have active Ozon access.

#### ChatGPT (Codex)

The recommended setup uses the ChatGPT app interface:

1. Switch ChatGPT to **Codex** mode. Connected MCP servers are not used in regular ChatGPT mode.
2. Open **Settings → Plugins → MCP**.
3. Select **Add → Add MCP server**.
4. Choose **Streamable HTTP**.
5. Add one or both servers:

   ```text
   Name: sellmonitor_analytics
   URL: https://sellmonitor.com/mcp/sellmonitor
   Bearer token: leave empty
   Headers: leave empty
   ```

   ```text
   Name: sellmonitor_inner_analytics
   URL: https://sellmonitor.com/mcp/inner-analytics
   Bearer token: leave empty
   Headers: leave empty
   ```

6. Save the server and select **Restart**.
7. Select **Authorize** in the MCP server list and approve access to your Sellmonitor account in the browser.
8. Return to a chat in Codex mode. Use `/mcp` to check the connection.

If the **Authorize** button does not respond, temporarily disable your VPN before selecting it. Complete authorization in the browser, then enable the VPN again.

Codex CLI alternative:

```bash
codex mcp add sellmonitor_analytics --url https://sellmonitor.com/mcp/sellmonitor
codex mcp login sellmonitor_analytics

codex mcp add sellmonitor_inner_analytics --url https://sellmonitor.com/mcp/inner-analytics
codex mcp login sellmonitor_inner_analytics
```

#### Cursor

Open MCP settings or **Tools & Integrations** and add:

```json
{
  "mcpServers": {
    "sellmonitor_analytics": {
      "url": "https://sellmonitor.com/mcp/sellmonitor"
    },
    "sellmonitor_inner_analytics": {
      "url": "https://sellmonitor.com/mcp/inner-analytics"
    }
  }
}
```

Save the configuration and select **Connect** or **Login**. Cursor will open the Sellmonitor OAuth page.

#### VS Code

1. Open the Command Palette and select `MCP: Add Server`.
2. Choose HTTP / Server-Sent Events.
3. Add the market or seller analytics MCP URL.
4. Enter the corresponding technical server name.
5. Open `MCP: List Servers`, start the server, and complete OAuth authorization.

#### Claude Code

```bash
claude mcp add --transport http --scope user sellmonitor_analytics https://sellmonitor.com/mcp/sellmonitor
claude mcp add --transport http --scope user sellmonitor_inner_analytics https://sellmonitor.com/mcp/inner-analytics
```

OAuth should open automatically. If it does not, run `/mcp` in Claude Code and authorize the required server.

### Troubleshooting

- Check the URL, refresh the MCP server list, or restart the client.
- Make sure you are signed in to the correct Sellmonitor account in your default browser.
- Check that your subscription and Ozon access are active.
- Never paste your password, access token, or user ID into MCP settings.
- If the assistant answers without data, explicitly say: “Use Sellmonitor MCP” or “Use Sellmonitor seller analytics MCP.”

Detailed guides: [market analytics](https://sellmonitor.com/mcp/analytics/instructions) · [seller analytics](https://sellmonitor.com/mcp/inner-analytics/instructions)
