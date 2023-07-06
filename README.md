# Scheduled backups Netlify function

This is a collection of lambda functions and scheduled functions meant to be used with [this DatoCMS plugin](https://github.com/marcelofinamorvieira/datocms-plugin-automatic-environment-backups) to automatically backup your main environment on a daily and weekly manner.

You can also deploy this project to netlify through [this one-click-deploy](https://app.netlify.com/start/deploy?repository=https://github.com/marcelofinamorvieira/datocms-backups-scheduled-netlify-function)

It consists of two scheduled functions that fork and replace old backups with new ones (if the old backups are not being used), making it so there is always a daily backup environment, and weekly backup environment.
Additionally, it also has a "initialization" lambda function that connects the plugin with the netlify instance.
