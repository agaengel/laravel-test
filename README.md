## Demo Laravel App for Deploy Now

# Setup steps
Setup the project with a Static M [![Deploy to IONOS](https://images.ionos.space/deploy-now-icons/deploy-to-ionos-btn.svg)](https://ionos.space/setup?repo=https://github.com/agaengel/laravel-test)

###  manual changes

change [workflow](.github/workflow/ionos-space.yml) from uses: ionos-deploy-now/deploy-to-ionos-action@v1 to uses: agaengel/deploy-to-ionos-action@master to get the remote command execution from [remote.commands](./remote.commands)

provide these secrets in to send the email in the repos secrects: https://github.com/$user$/$repository$/settings/secrets/actions

|secret|explanation|example|
|------|-----------|-------|
|MAIL_HOST|smtp| smtp.ionos.de |
|MAIL_PORT|smtp port|587|
|MAIL_USERNAME|smtp user||
|MAIL_PASSWORD|smtp password||
|MAIL_FROM_ADDRESS|sending email address||
