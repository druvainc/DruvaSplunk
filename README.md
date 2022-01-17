# DruvaSplunk
Druva apps for Splunkbase


# Druva's app for Splunk base
Run following command to create tar.gz file

COPYFILE_DISABLE=1 tar -cvzf druva-app-for-splunk_101.tar.gz Druva

Run following command to generate the auth token, enter password when prompt 
curl -k -u username \
     --url "https://api.splunk.com/2.0/rest/login/splunk"

Run following command to validate the app with splunk before pushing it to splunkbase

curl -X POST 
-H "Authorization: bearer authtoken" 
-H "Cache-Control: no-cache" 
-F "app_package=@"druva-app-for-splunk_101.tar.gz"" 
-F "included_tags=cloud" 
--url https://appinspect.splunk.com/v1/app/validate
