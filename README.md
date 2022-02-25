# tanzu-dotnet-app
tanzu-dotnet-app


Create the app
```
# dot net (core) api
tanzu apps workload create tanzu-dotnet-app \
-n dev --git-repo https://github.com/bmullan-pivotal/tanzu-dotnet-app \
--git-branch main --type web  
```

Get the url
```
tanzu apps workload get tanzu-dotnet-app
```

Curl the endpoint

```
curl http://tanzu-dotnet-app-dev.tap.vinalhaven.info/weatherforecast
``


