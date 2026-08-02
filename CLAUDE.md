# self-host-starter - AI Agent Guidelines

## Agent Context
This is an infrastructure-as-code repository. If the user asks you to add a new service to this stack:
1. Ensure the new service is lightweight and absolutely necessary.
2. Add it to `docker-compose.yml`.
3. Add any required environment variables to `.env.example`.
4. Ensure it has a `restart: unless-stopped` policy.
5. Use standard official images wherever possible.
