Примеры:
 curl --location 'localhost/api/v1/calculate' \
--header 'Content-Type: application/json' \
--data '{
  "expression": "2+2*2"
  "resposense": "6"
}'

curl --location 'localhost/api/v1/calculate' \
--header 'Content-Type: application/json' \
--data '{
  "expression": "два+2*2"
  "resposense": "error 422"
  если сервер принял значение но не смог обработать
}'

curl --location 'localhost/api' \
--header 'Content-Type: application/json' \
--data '{
  "expression": "2"
  "resposense": "error 500"
}'

curl --location 'localhost/api/v1/calculate' \
--header 'Content-Type: application/json' \
--data '{
  "expression": ""
  "resposense": "error 404"
это значит что сервер не нашел такую Url ссылку
}'


Код запускать с помощью этой команды
 go run "c:\lessons.go\calc"
 
 
