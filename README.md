# Download
```
mkdir go_calculate
cd go_calculate
git clone https://github.com/heemesss/yandex_go
```
# Start
```
go run main.go
```

# Test
```
curl --location 'localhost:8080/api/v1/calculate' \
--header 'Content-Type: application/json' \
--data '{
    "expression": "2+2*2"
}'
```
## Error 422
```
curl --location 'localhost:8080/api/v1/calculate' \
--header 'Content-Type: application/json' \
--data '{
    "expression": ""
}'
```
