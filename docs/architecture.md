## Architecture Decisions

### Why Telegram Commands?
- Prevents unwanted scheduled spam
- Allows editorial control
- Supports multi-command routing

### Why Google Sheets for Deduplication?
- Simple persistent state
- Human-readable audit log
- Easy recovery and debugging

### Why Limit to 1 Item?
- Avoids Telegram rate limits
- Preserves content quality
- Prevents flooding subscribers

### Why Separate Caption and Image Generation?
- Independent retries
- Better prompt control
- Easier future platform expansion
