# test-postgres-init
``` helm -n $NS install regclient mosip/regclient \
  --set regclient.upgradeServerUrl=https://$INTERNAL_HOST \
  --set regclient.healthCheckUrl=$HEALTH_URL \
  --set regclient.hostName=$INTERNAL_HOST \
  --set istio.host=$REGCLIENT_HOST \
  --wait \
  -f values.yaml \
  --version $CHART_VERSION ```
