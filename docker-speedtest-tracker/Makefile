up:
	clear
	@mkdir ./config
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

key:
	clear
	@echo "base64:$$(cat /dev/urandom | head -c32 | base64)"

servers:
	clear
	@docker run -it --rm --entrypoint /bin/bash lscr.io/linuxserver/speedtest-tracker:latest list-servers