up:
	clear
	@mkdir -p ./data
	@chown 1000 ./data
	@docker compose up -d

down:
	clear
	@docker compose down

restart:
	clear
	@docker compose restart

ps:
	clear
	@docker compose ps

logs:
	clear
	@docker compose logs -f

key:
	clear
	@python -c "import os;import base64;random_bytes = os.urandom(32);app_key = f\"base64:{base64.b64encode(random_bytes).decode('utf-8')}\";print(app_key)"
