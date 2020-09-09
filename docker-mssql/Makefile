up:
	clear
	@mkdir -p data
	@docker-compose up -d

down:
	clear
	@docker-compose down

restart:
	clear
	@docker-compose restart

ps:
	clear
	@docker-compose ps

logs:
	clear
	@docker-compose logs -f

console:
	clear
	@docker exec -it mssql /opt/mssql-tools/bin/sqlcmd -S localhost -U sa
	