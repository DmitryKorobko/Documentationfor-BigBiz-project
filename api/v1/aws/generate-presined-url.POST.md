Метод формирования ссылки для закгрузки картинки на AWS S3
==========================================

`POST /api/v1/image/sign-s3-image-policy`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| folder             | string               | Название папки                     | +              |
| fileType           | ENUM (png, jpeg, jpg)| Тип файла                          | +              |

Пример ответа `POST /api/v1/image/sign-s3-image-policy`
------------------------------------------------------

```json
{
  "url": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozgcYQNdN97d2PelAf9.png",
  "signedUrl": "https://s3.eu-central-1.amazonaws.com/assets-dev.ourcnc.com/comment_images/9oyf_ahbHeH7VozgcYQNdN97d2PelAf9.png?X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIYUF773SEDJRRZRA%2F20170309%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20170309T130945Z&X-Amz-SignedHeaders=host&X-Amz-Expires=172800&X-Amz-Signature=6afad1067b8adbb0f7b340833998596592355a225c90aaad0312f7a3419aaded"
}
```