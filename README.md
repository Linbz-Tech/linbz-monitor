# linbz-monitor

Monitor de disponibilidade da plataforma da Linbz (https://app.linbz.com).

A cada 5 minutos, o GitHub Actions confere a página inicial e o `/mcp/platform/health`. Se cair,
abre uma issue "Plataforma fora do ar" neste repositório (o GitHub avisa por e-mail); quando volta,
comenta e fecha.

Fica num repositório público porque repositório público tem minutos ilimitados de GitHub Actions;
aqui não há código da plataforma nem segredo, só o endereço público que já está na internet.
Documentação completa: `docs/producao.md` do repositório da plataforma.
