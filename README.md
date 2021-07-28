# Quiz App

## Blog Post API Routes

### Get All Blog Post
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/blog'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": [
        {
            "id": 1,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Assumenda repudiandae rerum delectus maiores illum et sed.",
            "description": "Maxime nesciunt cupiditate eveniet sit laudantium magni impedit. Et aliquam eos molestiae voluptatum. Minus iste eaque laboriosam voluptatem cupiditate magni dolorem est. Similique pariatur rerum laborum explicabo. Neque voluptates et animi dignissimos et totam. Sit velit inventore nemo provident. Tempore sapiente in mollitia. Quae sunt quos expedita aut. Saepe maxime corporis sed nemo. Nemo occaecati aperiam voluptatem consequatur inventore quos id. Amet non libero rerum dicta dicta porro nihil. Veniam et non aperiam.",
            "category": "inventore",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 2,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Asperiores qui asperiores molestiae laboriosam expedita.",
            "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo. Quis at omnis voluptas quam ab qui reprehenderit. Quae libero est earum veniam soluta aut minus et. Veritatis quisquam necessitatibus ut.",
            "category": "sunt",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 3,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Accusantium et rem et voluptas.",
            "description": "Consequuntur hic quas provident sunt. Vero placeat et quasi nam natus quo consequuntur. Harum vel voluptatem est. Sed et quod omnis ipsa veritatis veniam vel. Esse odio voluptas nihil temporibus est. Qui enim temporibus saepe illum deleniti natus tempore. Est molestiae minima et consectetur. Aperiam laudantium deserunt aut rerum libero dolorem in. Et dolor explicabo provident explicabo odio voluptatem. Animi qui enim nihil unde ex nihil illum. Sapiente excepturi sapiente adipisci dolores sapiente velit.",
            "category": "provident",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 4,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Et sapiente magni et et non iusto molestiae.",
            "description": "Dicta ducimus veniam et sed. Aliquam et in eaque optio quidem vel corporis. Ea et et voluptate labore sequi est dolorem. Laudantium voluptatum explicabo ad dolores ut qui id. Officiis rerum nihil quo necessitatibus sed illum quasi. Minima repellendus debitis explicabo aut. Sit omnis qui rerum maiores asperiores aliquid. Harum similique cum tempora minus voluptas provident cumque minima. Ducimus maiores at saepe consequatur laudantium.",
            "category": "hic",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 5,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Libero eius veritatis illo ad.",
            "description": "Ex rem soluta est ab. Voluptas consequatur quo cumque cupiditate ea nihil qui. Voluptas aut enim vitae consequatur possimus eum commodi. Modi ullam enim et. Esse eius iusto facilis. Explicabo cumque quidem consequuntur dolor. Soluta consequatur ut quia fugiat. Id animi rerum laboriosam. At ut possimus iusto iure id officia officiis. Autem et hic qui totam minus enim. Voluptas nam quas et cumque qui quod. Consectetur maiores ducimus illo itaque occaecati laboriosam dolorum.",
            "category": "ut",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 6,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Possimus id magni ut accusamus.",
            "description": "Quia et mollitia ab delectus facilis aut. Placeat recusandae modi modi tempore quibusdam. Temporibus qui odio molestiae accusantium adipisci. Magnam tempora et tempore consectetur aspernatur voluptatum. Itaque dolor fugiat qui quos voluptatum at magnam. Quia asperiores voluptates iste at. Exercitationem id numquam facilis.",
            "category": "commodi",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 7,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Placeat officiis voluptate illo fugit error.",
            "description": "Nostrum labore officia reprehenderit sunt inventore blanditiis dignissimos. Dolore saepe aut omnis est omnis. Et in et tenetur consequatur nostrum. A possimus alias voluptatibus id veniam sed. Asperiores autem consequatur dolores dolore quis consequuntur velit. Ut explicabo vitae mollitia quibusdam. Eaque provident et dolore. Nisi voluptas reiciendis explicabo qui blanditiis et reprehenderit.",
            "category": "corrupti",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 8,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Eligendi tempore corporis fugit corporis ab sunt sit exercitationem.",
            "description": "Perspiciatis et aspernatur eum accusantium optio ab labore recusandae. Illo porro rem dolor earum voluptatem consequuntur. Nihil iusto eum perferendis quo enim. Nam eum ullam perferendis dolorem. Quod deleniti reiciendis in accusamus. Doloribus magni itaque similique harum ad quae doloribus. Qui temporibus in facilis perferendis voluptatem natus. Eius quam cum et quo aut natus. Eaque et assumenda voluptatem quisquam minus. Qui accusantium est odit a neque non. Dolores molestiae voluptatum labore exercitationem eum perferendis ut. Qui accusamus voluptatibus et assumenda corporis.",
            "category": "sint",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 9,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Natus officia aliquam incidunt quia vero quis.",
            "description": "Delectus eius laudantium laboriosam voluptas atque. Cupiditate velit dolorum modi minima id quaerat. Laborum eos molestias consequatur laboriosam aut dolorem. Quidem vitae ipsam ea debitis maxime illo. Qui ut accusantium dolores sit rerum. Facilis facere atque aut nostrum quaerat aspernatur. Consequatur at voluptatem et reiciendis magnam. Fuga quia quis deleniti doloremque optio praesentium. Adipisci quasi voluptatibus quaerat aliquam. Saepe totam doloribus cupiditate voluptas dolorum.",
            "category": "ut",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 10,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Mollitia recusandae et repellendus culpa.",
            "description": "Distinctio facere quia nihil id commodi non est. Omnis omnis rerum cum ipsa aliquid neque omnis ea. Quisquam et aut repellendus qui consequuntur. Ad quas reiciendis veniam. Libero tempore est soluta iusto. Hic id error dicta est eos doloremque dicta. Dignissimos beatae dolorem harum et. Dolorum perferendis qui et dolores nam occaecati modi nulla. Veniam ipsa est ut et autem eaque dolorum.",
            "category": "amet",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 11,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Et velit impedit similique aut saepe et.",
            "description": "Inventore nisi repudiandae qui. Nisi at expedita qui sint quo quibusdam. Earum qui eos non hic. Iure nulla illum non laudantium. Sit nisi et qui. Iusto ullam voluptas quidem ipsa vel. Enim reprehenderit distinctio delectus temporibus possimus. Sit animi ea nesciunt est laudantium qui nesciunt. Qui error ut non aut ut.",
            "category": "nemo",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 12,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Sint illo necessitatibus rerum qui.",
            "description": "Id dolores vel autem et atque voluptas. Earum laborum itaque enim in. Sint voluptatum est accusantium quo voluptas. Cum quas sit maiores. Aut ullam ut voluptatem in voluptatem. Dolor expedita eius doloribus commodi. Consequatur quo adipisci veritatis omnis dignissimos quia ea cumque.",
            "category": "qui",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 13,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Asperiores omnis quae blanditiis voluptatem.",
            "description": "Minima perspiciatis ut ipsum vel iste. Ab sint velit reprehenderit velit nisi eum eveniet. Similique blanditiis incidunt voluptate exercitationem exercitationem. Facere blanditiis dolorum omnis vel harum. Nesciunt sed suscipit non molestias velit. Debitis nihil nemo fugiat perspiciatis provident maxime aut. Aut repellat et voluptatum. Voluptas distinctio laboriosam omnis iste reprehenderit quo consequatur. Quia aut vel voluptates quo. Nam modi sit nihil dolor dolorum dolorem. Tempore quae quasi blanditiis. Unde tenetur culpa error quia est.",
            "category": "sint",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 14,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Aspernatur illum optio dicta et sit sed.",
            "description": "Soluta sequi est doloremque animi dignissimos sapiente rerum placeat. Aut culpa quidem porro sit inventore facere. In possimus placeat voluptas quas. Incidunt quia qui ea amet non. Animi ipsum et consequatur qui est. Nihil harum molestias odit et et rerum vel. Quasi placeat assumenda sit pariatur laboriosam et tempore aut. Veniam quo aliquid magni accusantium debitis. Ut corporis fugit animi ut magnam molestias nulla. Amet nostrum velit architecto tenetur. Et fugiat ex natus unde aut vel. Beatae non provident repellat numquam. Non consequatur cum eligendi eos sit. Qui possimus natus et iure.",
            "category": "quas",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 15,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "Similique repellendus et et id.",
            "description": "Qui eum et exercitationem quam ut necessitatibus omnis autem. Eum similique non aut ab velit voluptas est. Reprehenderit fuga eius quis amet numquam. Dolorum dolorem vero perspiciatis at laudantium at. Id omnis perferendis consequatur in expedita. Cupiditate consequuntur doloribus iure et. Rem qui molestiae delectus aut quisquam unde dolorum. Consequatur est saepe dolor sunt. Iste maiores est rerum molestias qui cumque et.",
            "category": "in",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/blog?page=1",
        "last": "https://revisechemistry.org/api/v1/blog?page=14",
        "prev": null,
        "next": "https://revisechemistry.org/api/v1/blog?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 14,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=5",
                "label": "5",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=6",
                "label": "6",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=7",
                "label": "7",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=8",
                "label": "8",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=9",
                "label": "9",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=10",
                "label": "10",
                "active": false
            },
            {
                "url": null,
                "label": "...",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=13",
                "label": "13",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=14",
                "label": "14",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/blog",
        "per_page": 15,
        "to": 15,
        "total": 200
    }
}
```

### Get Single Blog Post
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/blog/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": {
        "id": 1,
        "thumbnail": "https://source.unsplash.com/random",
        "title": "Assumenda repudiandae rerum delectus maiores illum et sed.",
        "description": "Maxime nesciunt cupiditate eveniet sit laudantium magni impedit. Et aliquam eos molestiae voluptatum. Minus iste eaque laboriosam voluptatem cupiditate magni dolorem est. Similique pariatur rerum laborum explicabo. Neque voluptates et animi dignissimos et totam. Sit velit inventore nemo provident. Tempore sapiente in mollitia. Quae sunt quos expedita aut. Saepe maxime corporis sed nemo. Nemo occaecati aperiam voluptatem consequatur inventore quos id. Amet non libero rerum dicta dicta porro nihil. Veniam et non aperiam.",
        "category": "inventore",
        "created_at": "2021-07-15T02:26:02.000000Z",
        "updated_at": "2021-07-15T02:26:02.000000Z"
    }
}
```

### Create/Add New Blog Post
```js
var formdata = new FormData();
formdata.append("thumbnail", fileInput.files[0], "/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg");
formdata.append("token", "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB");
formdata.append("title", "This is random title");
formdata.append("description", "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.");
formdata.append("category", "physics");

var requestOptions = {
  method: 'POST',
  body: formdata,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.MultipartRequest('POST', Uri.parse('https://revisechemistry.org/api/v1/blog'));
request.fields.addAll({
  'token': 'ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB',
  'title': 'This is random title',
  'description': 'Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.',
  'category': 'physics'
});
request.files.add(await http.MultipartFile.fromPath('thumbnail', '/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg'));

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "title": "This is random title",
        "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.",
        "category": "physics",
        "thumbnail": "http://localhost/resources/images/blog/blog_thumbnail-1626413092.jpeg",
        "message": "New blog post added"
    }
}
```

### Edit Existing Blog Post
```js
var formdata = new FormData();
formdata.append("thumbnail", fileInput.files[0], "/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg");
formdata.append("token", "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB");
formdata.append("title", "This is random title2");
formdata.append("description", "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.");
formdata.append("category", "physics");

var requestOptions = {
  method: 'POST',
  body: formdata,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog/8", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.MultipartRequest('POST', Uri.parse('https://revisechemistry.org/api/v1/blog/8'));
request.fields.addAll({
  'token': 'ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB',
  'title': 'This is random title2',
  'description': 'Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.',
  'category': 'physics'
});
request.files.add(await http.MultipartFile.fromPath('thumbnail', '/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg'));

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 8,
        "title": "This is random title2",
        "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.",
        "category": "physics",
        "thumbnail": "http://localhost/resources/images/blog/blog_thumbnail-8-1626413287.jpeg"
    },
    "message": "Blog post updated successfully"
}
```

### Delete Existing Blog Post
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/blog/1'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "message": "Blog post deleted successfully"
}
```

### Search For Blog Post
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "title": "random title"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog/search/title", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/blog/search/title'));
request.body = json.encode({
  "title": "random title"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": [
        {
            "id": 8,
            "thumbnail": "http://localhost/resources/images/blog/blog_thumbnail-8-1626413287.jpeg",
            "title": "This is random title2",
            "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.",
            "category": "physics",
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-16T05:28:07.000000Z"
        },
        {
            "id": 201,
            "thumbnail": "https://source.unsplash.com/random",
            "title": "This is a random title",
            "description": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.",
            "category": "biology",
            "created_at": "2021-07-16T04:28:08.000000Z",
            "updated_at": "2021-07-16T04:28:08.000000Z"
        },
        {
            "id": 202,
            "thumbnail": "http://localhost/resources/images/blog/blog_thumbnail-1626413092.jpeg",
            "title": "This is random title",
            "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.",
            "category": "physics",
            "created_at": "2021-07-16T05:24:52.000000Z",
            "updated_at": "2021-07-16T05:24:52.000000Z"
        }
    ]
}
```

### Filter For Blog Post
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "category": "physics",
  "order": "ASC"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/blog/filter/post", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/blog/filter/post'));
request.body = json.encode({
  "category": "physics",
  "order": "ASC"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "current_page": 1,
        "data": [
            {
                "id": 8,
                "thumbnail": "http://localhost/resources/images/blog/blog_thumbnail-8-1626413287.jpeg",
                "title": "This is random title2",
                "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.",
                "category": "physics",
                "created_at": "2021-07-15 02:26:02",
                "updated_at": "2021-07-16 05:28:07"
            },
            {
                "id": 202,
                "thumbnail": "http://localhost/resources/images/blog/blog_thumbnail-1626413092.jpeg",
                "title": "This is random title",
                "description": "Autem corporis dolores sint. Nostrum cum ut ipsum ut. Sit saepe sit voluptate fuga maxime quas suscipit. Ab cupiditate neque ut quae. Nihil sed vero et beatae voluptas qui. Ut itaque debitis dolorum impedit facilis ad rerum. Aspernatur soluta quia autem. Quibusdam ipsa nobis nihil aut nihil sint molestias. Sapiente alias quo tenetur sapiente omnis a et quo.",
                "category": "physics",
                "created_at": "2021-07-16 05:24:52",
                "updated_at": "2021-07-16 05:24:52"
            }
        ],
        "first_page_url": "https://revisechemistry.org/api/v1/blog/filter/post?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "https://revisechemistry.org/api/v1/blog/filter/post?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/blog/filter/post?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "https://revisechemistry.org/api/v1/blog/filter/post",
        "per_page": 15,
        "prev_page_url": null,
        "to": 2,
        "total": 2
    }
}
```





## MetaData API Routes

### Get All MetaData
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/meta-data", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/meta-data'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": [
        {
            "id": 1,
            "about": "dolor",
            "data": "+1-847-606-1015",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 2,
            "about": "qui",
            "data": "kuvalis.alexandro@hotmail.com",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 3,
            "about": "at",
            "data": "floyd.hayes@yahoo.com",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 4,
            "about": "hic",
            "data": "chet.heathcote@gmail.com",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 5,
            "about": "possimus",
            "data": "kimberly50@ohara.net",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 6,
            "about": "sunt",
            "data": "neva.tromp@dach.com",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 7,
            "about": "aut",
            "data": "979-407-1930",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 8,
            "about": "error",
            "data": "deja47@turner.org",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 9,
            "about": "odit",
            "data": "gutmann.willow@bogisich.com",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        },
        {
            "id": 10,
            "about": "voluptates",
            "data": "dach.pearlie@hermiston.com",
            "created_at": "2021-07-15T02:26:03.000000Z",
            "updated_at": "2021-07-15T02:26:03.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/meta-data?page=1",
        "last": "https://revisechemistry.org/api/v1/meta-data?page=20",
        "prev": null,
        "next": "https://revisechemistry.org/api/v1/meta-data?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 20,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=5",
                "label": "5",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=6",
                "label": "6",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=7",
                "label": "7",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=8",
                "label": "8",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=9",
                "label": "9",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=10",
                "label": "10",
                "active": false
            },
            {
                "url": null,
                "label": "...",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=19",
                "label": "19",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=20",
                "label": "20",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/meta-data?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/meta-data",
        "per_page": 10,
        "to": 10,
        "total": 200
    }
}
```

### Get Single MetaData
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/meta-data/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/meta-data/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "id": 1,
    "about": "dolor",
    "data": "+1-847-606-1015",
    "created_at": "2021-07-15T02:26:03.000000Z",
    "updated_at": "2021-07-15T02:26:03.000000Z"
}
```

### Create/Add New MetaData
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "about": "email",
  "data": "justmail@gmail.com"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/meta-data", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/meta-data'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "about": "email",
  "data": "justmail@gmail.com"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "about": "email",
        "data": "justmail@gmail.com",
        "message": "New meta data added"
    }
}
```

### Edit Existing MetaData
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "about": "email",
  "data": "justmail@gmail.com"
});

var requestOptions = {
  method: 'PUT',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/meta-data/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('PUT', Uri.parse('https://revisechemistry.org/api/v1/meta-data/1'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "about": "email",
  "data": "justmail@gmail.com"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 1,
        "about": "email",
        "data": "justmail@gmail.com"
    },
    "message": "Meta data updated successfully"
}
```

### Delete Existing MetaData
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/meta-data/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/meta-data/1'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "message": "Meta data successfully deleted"
}
```



## Forum Data API Routes

### Get All Forum Data
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/forum", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/forum'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": [
        {
            "id": 1,
            "user_id": 58,
            "question": "Illo quia voluptatem est.",
            "reply": "Ratione atque beatae et a atque provident. Cupiditate tempore rem recusandae ipsum et impedit ut. Ipsa voluptatem pariatur consequuntur dignissimos.",
            "reply_to": 60,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 2,
            "user_id": 38,
            "question": "Rerum neque porro voluptatem quo repellat.",
            "reply": "Aut harum ut voluptatum omnis quis quis. Est asperiores sed non. Sit earum rerum perspiciatis voluptate odit id. Praesentium accusantium consequatur ut eius totam eaque. Similique temporibus fugiat sit temporibus quia est.",
            "reply_to": 100,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 3,
            "user_id": 81,
            "question": "Consequatur rerum in excepturi voluptatem odit possimus tenetur odit.",
            "reply": "Voluptas perferendis earum aut repudiandae id sapiente vitae. Voluptatem sunt ab esse error facere dolor nam. Qui exercitationem autem vero ea iure aspernatur distinctio.",
            "reply_to": 34,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 4,
            "user_id": 1,
            "question": "Magnam inventore quasi accusamus.",
            "reply": "Quasi consequatur sunt libero aut. Molestiae et quis aut.",
            "reply_to": 33,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 5,
            "user_id": 71,
            "question": "Porro eos magnam qui omnis veritatis eligendi ratione aliquam.",
            "reply": "Tempore debitis et quae molestiae tempore placeat. Voluptatum veritatis qui qui odio illo. Quisquam esse commodi labore minus et.",
            "reply_to": 82,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 6,
            "user_id": 64,
            "question": "Et iure nemo et sed nisi aut.",
            "reply": "Deleniti quam suscipit recusandae voluptatum quis esse non. Ipsum a voluptatem libero et dolor tempore tempore. Molestiae repellat autem ducimus. Animi ullam hic illo neque ea.",
            "reply_to": 65,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 7,
            "user_id": 29,
            "question": "Quam voluptatem et qui harum.",
            "reply": "Laudantium eum voluptatem vitae eos. Ea odio quas amet provident. Rerum est ut porro unde nam rerum animi. Quidem repudiandae non non dolorem.",
            "reply_to": 30,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 8,
            "user_id": 17,
            "question": "Dolor qui ut qui.",
            "reply": "Voluptatem aperiam nesciunt alias aperiam. Consequatur molestias adipisci reprehenderit perferendis.",
            "reply_to": 26,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 9,
            "user_id": 8,
            "question": "Ab tempore minima impedit.",
            "reply": "Sed non quidem consequatur ut quam quas a. Quis ut porro qui quis quas aut. Officia voluptatem voluptate ea.",
            "reply_to": 44,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        },
        {
            "id": 10,
            "user_id": 30,
            "question": "Pariatur odio unde praesentium repellendus.",
            "reply": "Perspiciatis amet quisquam qui et. Aliquam est quos possimus voluptatum eligendi ut. Rerum nam nam reprehenderit.",
            "reply_to": 81,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/forum?page=1",
        "last": "https://revisechemistry.org/api/v1/forum?page=20",
        "prev": null,
        "next": "https://revisechemistry.org/api/v1/forum?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 20,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=5",
                "label": "5",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=6",
                "label": "6",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=7",
                "label": "7",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=8",
                "label": "8",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=9",
                "label": "9",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=10",
                "label": "10",
                "active": false
            },
            {
                "url": null,
                "label": "...",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=19",
                "label": "19",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=20",
                "label": "20",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/forum?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/forum",
        "per_page": 10,
        "to": 10,
        "total": 200
    }
}
```

### Get Single Forum Data
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/forum/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/forum/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": {
        "id": 1,
        "user_id": 58,
        "question": "Illo quia voluptatem est.",
        "reply": "Ratione atque beatae et a atque provident. Cupiditate tempore rem recusandae ipsum et impedit ut. Ipsa voluptatem pariatur consequuntur dignissimos.",
        "reply_to": 60,
        "created_at": "2021-07-15T02:26:02.000000Z",
        "updated_at": "2021-07-15T02:26:02.000000Z"
    }
}
```

### Create/Add New Forum Data 
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8",
  "question": "What is a random question ?",
  "reply": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.",
  "reply_to": 20
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/forum", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/forum'));
request.body = json.encode({
  "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8",
  "question": "What is a random question ?",
  "reply": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.",
  "reply_to": 20
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "user_id": 201,
        "question": "What is a random question ?",
        "reply": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.",
        "reply_to": 20,
        "message": "New Forum data added"
    }
}
```

### Edit Existing Forum Data
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8",
  "question": "What is a random question ?",
  "reply": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.",
  "reply_to": 20
});

var requestOptions = {
  method: 'PUT',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/forum/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('PUT', Uri.parse('https://revisechemistry.org/api/v1/forum/1'));
request.body = json.encode({
  "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8",
  "question": "What is a random question ?",
  "reply": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.",
  "reply_to": 20
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 1,
        "user_id": 58,
        "question": "What is a random question ?",
        "reply": "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged.",
        "reply_to": 60
    },
    "message": "Forum data updated successfully"
}
```

### Delete Existing Forum Data
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/forum/2", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/forum/2'));
request.body = json.encode({
  "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "message": "Forum data deleted successfully"
}
```


### Search Forum Data
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "question": "Quam voluptatem et qui harum"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/forum/search/question", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/forum/search/question'));
request.body = json.encode({
  "question": "Quam voluptatem et qui harum"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": [
        {
            "id": 7,
            "user_id": 29,
            "question": "Quam voluptatem et qui harum.",
            "reply": "Laudantium eum voluptatem vitae eos. Ea odio quas amet provident. Rerum est ut porro unde nam rerum animi. Quidem repudiandae non non dolorem.",
            "reply_to": 30,
            "created_at": "2021-07-15T02:26:02.000000Z",
            "updated_at": "2021-07-15T02:26:02.000000Z"
        }
    ]
}
```



## Student API Routes

### Get All Student
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/student'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": [
        {
            "id": 1,
            "first_name": "Jeff",
            "last_name": "Daugherty",
            "email": "brando.kulas@example.net",
            "contact": "412.527.7842",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 2,
            "first_name": "Anibal",
            "last_name": "Price",
            "email": "alexandrea51@example.org",
            "contact": "+1-949-679-5883",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 3,
            "first_name": "Isabella",
            "last_name": "Waters",
            "email": "dcormier@example.org",
            "contact": "858.261.0769",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 4,
            "first_name": "Dylan",
            "last_name": "Moen",
            "email": "dedrick07@example.com",
            "contact": "(703) 596-5640",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 5,
            "first_name": "Destini",
            "last_name": "Reynolds",
            "email": "davis.jamarcus@example.org",
            "contact": "+1.641.437.9522",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 6,
            "first_name": "Ashly",
            "last_name": "Lakin",
            "email": "sandrine.rau@example.net",
            "contact": "+1-814-448-6869",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 7,
            "first_name": "Mrs.",
            "last_name": "Schuster",
            "email": "arlo.koelpin@example.com",
            "contact": "+1-605-589-8710",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 8,
            "first_name": "Kyra",
            "last_name": "Bosco",
            "email": "sean.orn@example.org",
            "contact": "+1.419.480.2232",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 9,
            "first_name": "Mr.",
            "last_name": "Conroy",
            "email": "herminia.lakin@example.org",
            "contact": "+1.806.542.9034",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        },
        {
            "id": 10,
            "first_name": "Dr.",
            "last_name": "Rose",
            "email": "judge82@example.com",
            "contact": "870-970-9608",
            "avatar": "https://source.unsplash.com/random",
            "created_at": "2021-07-15T02:26:20.000000Z",
            "updated_at": "2021-07-15T02:26:20.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/student?page=1",
        "last": "https://revisechemistry.org/api/v1/student?page=20",
        "prev": null,
        "next": "https://revisechemistry.org/api/v1/student?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 20,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=5",
                "label": "5",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=6",
                "label": "6",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=7",
                "label": "7",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=8",
                "label": "8",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=9",
                "label": "9",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=10",
                "label": "10",
                "active": false
            },
            {
                "url": null,
                "label": "...",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=19",
                "label": "19",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=20",
                "label": "20",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/student",
        "per_page": 10,
        "to": 10,
        "total": 200
    }
}
```

### Get Single Student
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/student/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": {
        "id": 1,
        "first_name": "Jeff",
        "last_name": "Daugherty",
        "email": "brando.kulas@example.net",
        "contact": "412.527.7842",
        "avatar": "https://source.unsplash.com/random",
        "created_at": "2021-07-15T02:26:20.000000Z",
        "updated_at": "2021-07-15T02:26:20.000000Z"
    }
}
```

### Create/Add New Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "first_name": "Rahul",
  "last_name": "Thapa",
  "email": "rahul34@gmail.com",
  "password": "1234",
  "password_confirmation": "1234"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/student'));
request.body = json.encode({
  "first_name": "Rahul",
  "last_name": "Thapa",
  "email": "rahul34@gmail.com",
  "password": "1234",
  "password_confirmation": "1234"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "first_name": "Rahul",
        "last_name": "Thapa",
        "email": "rahul34@gmail.com",
        "contact": null,
        "password": "1234",
        "avatar": null,
        "token": "zUsifOwM4OVtlzoT8S04tukXrepz6LrZKGfzO2FS6fwYtvdNgsyUhcuKPw5QLakyH3wEAf2NnwTPDM36rdOg5slrtGu8KTODRFfPSycl9vuNGYhP0TVUlcuPj7jRwGCdP9piJSjhazMHnRQ9OVTXw37NsOOorJSQvPt0JV03bXDM9GaDKZeGN7p1ZZWgOEtErUgH8nA7n8AlJaObd8RcC0rtttrBubQlQrn0iRPMyENRxHbzlmd8JoFIMvBPgR8",
        "message": "New student added"
    }
}
```

### General Editing Existing Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed",
  "first_name": "Rohit",
  "last_name": "Karki",
  "contact": "2318756187"
});

var requestOptions = {
  method: 'PUT',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('PUT', Uri.parse('https://revisechemistry.org/api/v1/student'));
request.body = json.encode({
  "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed",
  "first_name": "Rohit",
  "last_name": "Karki",
  "contact": "2318756187"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 202,
        "first_name": "Rohit",
        "last_name": "Karki",
        "contact": "2318756187",
        "email": "roshan34@gmail.com",
        "avatar": null
    },
    "message": "Student record updated successfully"
}
```

### Editing Password Of Existing Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed",
  "new_password": "456",
  "new_password_confirmation": "456"
});

var requestOptions = {
  method: 'PUT',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student/new-password", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('PUT', Uri.parse('https://revisechemistry.org/api/v1/student/new-password'));
request.body = json.encode({
  "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed",
  "new_password": "456",
  "new_password_confirmation": "456"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 202,
        "first_name": "Rohit",
        "last_name": "Karki",
        "contact": "2318756187",
        "email": "roshan34@gmail.com",
        "avatar": null,
        "token": "xYAAczA0jq3Up6JvgSz9AysPFsqycdehp2ntgyxR9affdL93yfjGJb3Bi5HSmZItltVzQlUkNJc8nah3PHGUDZwl66ltvCWp3mQzbUXvf85lQ0ZIotCBXlnbYNBRIrNAGgbqhSlvatZWok0yyhGl289rDMxgfdr3RdbNptM2uTb8GHo2TgNC2icPXirRnYqG92OeeuogSY3BtbGJVjOYAYXC7NnpL65wVyIH53wWpnkiNC47UxzinpbEgc6mbDP"
    },
    "message": "Student record updated successfully"
}
```


### Delete Existing Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "xYAAczA0jq3Up6JvgSz9AysPFsqycdehp2ntgyxR9affdL93yfjGJb3Bi5HSmZItltVzQlUkNJc8nah3PHGUDZwl66ltvCWp3mQzbUXvf85lQ0ZIotCBXlnbYNBRIrNAGgbqhSlvatZWok0yyhGl289rDMxgfdr3RdbNptM2uTb8GHo2TgNC2icPXirRnYqG92OeeuogSY3BtbGJVjOYAYXC7NnpL65wVyIH53wWpnkiNC47UxzinpbEgc6mbDP"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/student'));
request.body = json.encode({
  "token": "xYAAczA0jq3Up6JvgSz9AysPFsqycdehp2ntgyxR9affdL93yfjGJb3Bi5HSmZItltVzQlUkNJc8nah3PHGUDZwl66ltvCWp3mQzbUXvf85lQ0ZIotCBXlnbYNBRIrNAGgbqhSlvatZWok0yyhGl289rDMxgfdr3RdbNptM2uTb8GHo2TgNC2icPXirRnYqG92OeeuogSY3BtbGJVjOYAYXC7NnpL65wVyIH53wWpnkiNC47UxzinpbEgc6mbDP"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": "Account deleted successfully"
}
```

### Login Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "email": "roshan34@gmail.com",
  "password": "1234"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student/login", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/student/login'));
request.body = json.encode({
  "email": "roshan34@gmail.com",
  "password": "1234"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "first_name": "Roshan",
        "last_name": "Thapa",
        "email": "roshan34@gmail.com",
        "contact": "135367563",
        "password": "$2y$10$y5Ry7EINS/6QXyH3zQKXWuYbYKwgHe59nDMg0dSvW53naZWXgd3BG",
        "avatar": null,
        "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed"
    }
}
```

### Logout Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student/logout", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/student/logout'));
request.body = json.encode({
  "token": "j6kqLmPMGg6uAKSLKpD7B7guW5DfCJWWRTttbWweHMoCGRKGDr1vop9FIkICdgAAfSfHDcpz5yH6JA2j8zexv3ohkigdmjNWGxAPeVa1xsp3Ri60Jm2FB0y3FQEdyU0BTsSDFuKuKoi60qspplvUOXeGxZ9Uxa9PcgakRk26X5fsRvDdaJIoHDtOiu59ZKe8jj6074CCFDhrifrqxWXdhXqQoTT9sVoJk5XWDjr9IS3nKInXpCKnotGiTzlqoed"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": "Loging out",
    "note": "Clear client token"
}
```

### Forgot Password Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "xYAAczA0jq3Up6JvgSz9AysPFsqycdehp2ntgyxR9affdL93yfjGJb3Bi5HSmZItltVzQlUkNJc8nah3PHGUDZwl66ltvCWp3mQzbUXvf85lQ0ZIotCBXlnbYNBRIrNAGgbqhSlvatZWok0yyhGl289rDMxgfdr3RdbNptM2uTb8GHo2TgNC2icPXirRnYqG92OeeuogSY3BtbGJVjOYAYXC7NnpL65wVyIH53wWpnkiNC47UxzinpbEgc6mbDP",
  "email": "rahul34@gmail.com"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student/forgot-password", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/student/forgot-password'));
request.body = json.encode({
  "token": "xYAAczA0jq3Up6JvgSz9AysPFsqycdehp2ntgyxR9affdL93yfjGJb3Bi5HSmZItltVzQlUkNJc8nah3PHGUDZwl66ltvCWp3mQzbUXvf85lQ0ZIotCBXlnbYNBRIrNAGgbqhSlvatZWok0yyhGl289rDMxgfdr3RdbNptM2uTb8GHo2TgNC2icPXirRnYqG92OeeuogSY3BtbGJVjOYAYXC7NnpL65wVyIH53wWpnkiNC47UxzinpbEgc6mbDP",
  "email": "rahul34@gmail.com"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": "Sending reset link"
}
```


## Admin API Routes

### Edit Existing Admin
```js
var formdata = new FormData();
formdata.append("thumbnail", fileInput.files[0], "/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg");
formdata.append("token", "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB");
formdata.append("first_name", "Quiz");
formdata.append("last_name", "App");
formdata.append("avatar", fileInput.files[0], "/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg");

var requestOptions = {
  method: 'POST',
  body: formdata,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/admin/update", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.MultipartRequest('POST', Uri.parse('https://revisechemistry.org/api/v1/admin/update'));
request.fields.addAll({
  'token': 'ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB',
  'first_name': 'Quiz',
  'last_name': 'App'
});
request.files.add(await http.MultipartFile.fromPath('thumbnail', '/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg'));
request.files.add(await http.MultipartFile.fromPath('avatar', '/C:/Users/Ankit/Desktop/resource/martial-arts-master.jpeg'));

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 1,
        "first_name": "Quiz",
        "last_name": "App",
        "email": "admin@gmail.com",
        "avatar": "https://revisechemistry.org/resources/images/avatar/admin_profile-1-1626417207.jpeg",
        "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
    },
    "message": "Admin record updated successfully"
}
```

### Login Admin
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "email": "admin@gmail.com",
  "password": "quizapp"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/admin/login", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/admin/login'));
request.body = json.encode({
  "email": "admin@gmail.com",
  "password": "quizapp"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "first_name": "admin",
        "last_name": "admin",
        "email": "admin@gmail.com",
        "password": "$2y$10$Wq/Jvqe/xvEB1AiSoVzo1OwMIz6mOKQUQcQ0Rr1VOQCOR9XYPaRLG",
        "avatar": "https://source.unsplash.com/random",
        "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
    }
}
```

### Logout Admin
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/admin/logout", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/admin/logout'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": "Loging out",
    "note": "Clear client token"
}
```

### Forgot Password Admin
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "email": "admin@gmail.com"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/admin/forgot-password", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/admin/forgot-password'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "email": "admin@gmail.com"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": "Sending reset link"
}
```



## Student Report API Routes

### Get All Student Report
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student-report", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/student-report'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": [
        {
            "id": 1,
            "user_id": 92,
            "question_answer": "[{\"question_id\":13,\"answer\":\"A\"},{\"question_id\":2,\"answer\":\"B\"},{\"question_id\":77,\"answer\":\"C\"},{\"question_id\":74,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 2,
            "user_id": 93,
            "question_answer": "[{\"question_id\":32,\"answer\":\"A\"},{\"question_id\":77,\"answer\":\"B\"},{\"question_id\":5,\"answer\":\"C\"},{\"question_id\":75,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 3,
            "user_id": 42,
            "question_answer": "[{\"question_id\":91,\"answer\":\"A\"},{\"question_id\":20,\"answer\":\"B\"},{\"question_id\":30,\"answer\":\"C\"},{\"question_id\":50,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 4,
            "user_id": 53,
            "question_answer": "[{\"question_id\":63,\"answer\":\"A\"},{\"question_id\":66,\"answer\":\"B\"},{\"question_id\":91,\"answer\":\"C\"},{\"question_id\":33,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 5,
            "user_id": 11,
            "question_answer": "[{\"question_id\":77,\"answer\":\"A\"},{\"question_id\":37,\"answer\":\"B\"},{\"question_id\":63,\"answer\":\"C\"},{\"question_id\":54,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 6,
            "user_id": 57,
            "question_answer": "[{\"question_id\":52,\"answer\":\"A\"},{\"question_id\":23,\"answer\":\"B\"},{\"question_id\":53,\"answer\":\"C\"},{\"question_id\":46,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 7,
            "user_id": 48,
            "question_answer": "[{\"question_id\":76,\"answer\":\"A\"},{\"question_id\":89,\"answer\":\"B\"},{\"question_id\":29,\"answer\":\"C\"},{\"question_id\":1,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 8,
            "user_id": 36,
            "question_answer": "[{\"question_id\":9,\"answer\":\"A\"},{\"question_id\":73,\"answer\":\"B\"},{\"question_id\":65,\"answer\":\"C\"},{\"question_id\":28,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 9,
            "user_id": 68,
            "question_answer": "[{\"question_id\":65,\"answer\":\"A\"},{\"question_id\":99,\"answer\":\"B\"},{\"question_id\":65,\"answer\":\"C\"},{\"question_id\":15,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 10,
            "user_id": 99,
            "question_answer": "[{\"question_id\":62,\"answer\":\"A\"},{\"question_id\":97,\"answer\":\"B\"},{\"question_id\":24,\"answer\":\"C\"},{\"question_id\":55,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 11,
            "user_id": 69,
            "question_answer": "[{\"question_id\":20,\"answer\":\"A\"},{\"question_id\":21,\"answer\":\"B\"},{\"question_id\":98,\"answer\":\"C\"},{\"question_id\":67,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 12,
            "user_id": 53,
            "question_answer": "[{\"question_id\":97,\"answer\":\"A\"},{\"question_id\":97,\"answer\":\"B\"},{\"question_id\":66,\"answer\":\"C\"},{\"question_id\":22,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 13,
            "user_id": 3,
            "question_answer": "[{\"question_id\":95,\"answer\":\"A\"},{\"question_id\":91,\"answer\":\"B\"},{\"question_id\":86,\"answer\":\"C\"},{\"question_id\":51,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 14,
            "user_id": 40,
            "question_answer": "[{\"question_id\":23,\"answer\":\"A\"},{\"question_id\":42,\"answer\":\"B\"},{\"question_id\":4,\"answer\":\"C\"},{\"question_id\":34,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 15,
            "user_id": 50,
            "question_answer": "[{\"question_id\":78,\"answer\":\"A\"},{\"question_id\":82,\"answer\":\"B\"},{\"question_id\":94,\"answer\":\"C\"},{\"question_id\":3,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 16,
            "user_id": 6,
            "question_answer": "[{\"question_id\":28,\"answer\":\"A\"},{\"question_id\":76,\"answer\":\"B\"},{\"question_id\":7,\"answer\":\"C\"},{\"question_id\":85,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 17,
            "user_id": 94,
            "question_answer": "[{\"question_id\":13,\"answer\":\"A\"},{\"question_id\":14,\"answer\":\"B\"},{\"question_id\":90,\"answer\":\"C\"},{\"question_id\":13,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 18,
            "user_id": 32,
            "question_answer": "[{\"question_id\":26,\"answer\":\"A\"},{\"question_id\":34,\"answer\":\"B\"},{\"question_id\":65,\"answer\":\"C\"},{\"question_id\":62,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 19,
            "user_id": 21,
            "question_answer": "[{\"question_id\":42,\"answer\":\"A\"},{\"question_id\":83,\"answer\":\"B\"},{\"question_id\":86,\"answer\":\"C\"},{\"question_id\":52,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 20,
            "user_id": 3,
            "question_answer": "[{\"question_id\":59,\"answer\":\"A\"},{\"question_id\":78,\"answer\":\"B\"},{\"question_id\":28,\"answer\":\"C\"},{\"question_id\":15,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 21,
            "user_id": 99,
            "question_answer": "[{\"question_id\":21,\"answer\":\"A\"},{\"question_id\":80,\"answer\":\"B\"},{\"question_id\":51,\"answer\":\"C\"},{\"question_id\":9,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 22,
            "user_id": 40,
            "question_answer": "[{\"question_id\":40,\"answer\":\"A\"},{\"question_id\":1,\"answer\":\"B\"},{\"question_id\":66,\"answer\":\"C\"},{\"question_id\":86,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 23,
            "user_id": 12,
            "question_answer": "[{\"question_id\":24,\"answer\":\"A\"},{\"question_id\":69,\"answer\":\"B\"},{\"question_id\":35,\"answer\":\"C\"},{\"question_id\":17,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 24,
            "user_id": 31,
            "question_answer": "[{\"question_id\":45,\"answer\":\"A\"},{\"question_id\":74,\"answer\":\"B\"},{\"question_id\":26,\"answer\":\"C\"},{\"question_id\":73,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 25,
            "user_id": 66,
            "question_answer": "[{\"question_id\":97,\"answer\":\"A\"},{\"question_id\":60,\"answer\":\"B\"},{\"question_id\":57,\"answer\":\"C\"},{\"question_id\":55,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 26,
            "user_id": 90,
            "question_answer": "[{\"question_id\":85,\"answer\":\"A\"},{\"question_id\":5,\"answer\":\"B\"},{\"question_id\":72,\"answer\":\"C\"},{\"question_id\":33,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 27,
            "user_id": 45,
            "question_answer": "[{\"question_id\":43,\"answer\":\"A\"},{\"question_id\":57,\"answer\":\"B\"},{\"question_id\":66,\"answer\":\"C\"},{\"question_id\":96,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 28,
            "user_id": 64,
            "question_answer": "[{\"question_id\":47,\"answer\":\"A\"},{\"question_id\":37,\"answer\":\"B\"},{\"question_id\":15,\"answer\":\"C\"},{\"question_id\":87,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 29,
            "user_id": 90,
            "question_answer": "[{\"question_id\":84,\"answer\":\"A\"},{\"question_id\":72,\"answer\":\"B\"},{\"question_id\":44,\"answer\":\"C\"},{\"question_id\":12,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 30,
            "user_id": 18,
            "question_answer": "[{\"question_id\":55,\"answer\":\"A\"},{\"question_id\":70,\"answer\":\"B\"},{\"question_id\":73,\"answer\":\"C\"},{\"question_id\":93,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 31,
            "user_id": 17,
            "question_answer": "[{\"question_id\":64,\"answer\":\"A\"},{\"question_id\":23,\"answer\":\"B\"},{\"question_id\":97,\"answer\":\"C\"},{\"question_id\":71,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 32,
            "user_id": 27,
            "question_answer": "[{\"question_id\":20,\"answer\":\"A\"},{\"question_id\":50,\"answer\":\"B\"},{\"question_id\":11,\"answer\":\"C\"},{\"question_id\":44,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 33,
            "user_id": 100,
            "question_answer": "[{\"question_id\":7,\"answer\":\"A\"},{\"question_id\":70,\"answer\":\"B\"},{\"question_id\":38,\"answer\":\"C\"},{\"question_id\":100,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 34,
            "user_id": 89,
            "question_answer": "[{\"question_id\":5,\"answer\":\"A\"},{\"question_id\":27,\"answer\":\"B\"},{\"question_id\":39,\"answer\":\"C\"},{\"question_id\":54,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 35,
            "user_id": 53,
            "question_answer": "[{\"question_id\":14,\"answer\":\"A\"},{\"question_id\":49,\"answer\":\"B\"},{\"question_id\":51,\"answer\":\"C\"},{\"question_id\":74,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 36,
            "user_id": 11,
            "question_answer": "[{\"question_id\":38,\"answer\":\"A\"},{\"question_id\":11,\"answer\":\"B\"},{\"question_id\":82,\"answer\":\"C\"},{\"question_id\":19,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 37,
            "user_id": 16,
            "question_answer": "[{\"question_id\":52,\"answer\":\"A\"},{\"question_id\":94,\"answer\":\"B\"},{\"question_id\":6,\"answer\":\"C\"},{\"question_id\":8,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 38,
            "user_id": 14,
            "question_answer": "[{\"question_id\":4,\"answer\":\"A\"},{\"question_id\":58,\"answer\":\"B\"},{\"question_id\":59,\"answer\":\"C\"},{\"question_id\":65,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 39,
            "user_id": 80,
            "question_answer": "[{\"question_id\":4,\"answer\":\"A\"},{\"question_id\":16,\"answer\":\"B\"},{\"question_id\":86,\"answer\":\"C\"},{\"question_id\":13,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 40,
            "user_id": 84,
            "question_answer": "[{\"question_id\":82,\"answer\":\"A\"},{\"question_id\":58,\"answer\":\"B\"},{\"question_id\":65,\"answer\":\"C\"},{\"question_id\":84,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 41,
            "user_id": 16,
            "question_answer": "[{\"question_id\":66,\"answer\":\"A\"},{\"question_id\":12,\"answer\":\"B\"},{\"question_id\":89,\"answer\":\"C\"},{\"question_id\":8,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 42,
            "user_id": 31,
            "question_answer": "[{\"question_id\":68,\"answer\":\"A\"},{\"question_id\":2,\"answer\":\"B\"},{\"question_id\":20,\"answer\":\"C\"},{\"question_id\":20,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 43,
            "user_id": 23,
            "question_answer": "[{\"question_id\":35,\"answer\":\"A\"},{\"question_id\":92,\"answer\":\"B\"},{\"question_id\":42,\"answer\":\"C\"},{\"question_id\":80,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 44,
            "user_id": 21,
            "question_answer": "[{\"question_id\":37,\"answer\":\"A\"},{\"question_id\":3,\"answer\":\"B\"},{\"question_id\":63,\"answer\":\"C\"},{\"question_id\":88,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 45,
            "user_id": 91,
            "question_answer": "[{\"question_id\":89,\"answer\":\"A\"},{\"question_id\":88,\"answer\":\"B\"},{\"question_id\":77,\"answer\":\"C\"},{\"question_id\":17,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 0,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 46,
            "user_id": 45,
            "question_answer": "[{\"question_id\":62,\"answer\":\"A\"},{\"question_id\":90,\"answer\":\"B\"},{\"question_id\":11,\"answer\":\"C\"},{\"question_id\":55,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 47,
            "user_id": 48,
            "question_answer": "[{\"question_id\":61,\"answer\":\"A\"},{\"question_id\":59,\"answer\":\"B\"},{\"question_id\":75,\"answer\":\"C\"},{\"question_id\":99,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 2,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 48,
            "user_id": 40,
            "question_answer": "[{\"question_id\":77,\"answer\":\"A\"},{\"question_id\":81,\"answer\":\"B\"},{\"question_id\":30,\"answer\":\"C\"},{\"question_id\":14,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 49,
            "user_id": 52,
            "question_answer": "[{\"question_id\":76,\"answer\":\"A\"},{\"question_id\":53,\"answer\":\"B\"},{\"question_id\":18,\"answer\":\"C\"},{\"question_id\":14,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 3,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 50,
            "user_id": 86,
            "question_answer": "[{\"question_id\":79,\"answer\":\"A\"},{\"question_id\":80,\"answer\":\"B\"},{\"question_id\":17,\"answer\":\"C\"},{\"question_id\":39,\"answer\":\"D\"}]",
            "question_attempted_count": 4,
            "correct_answer_count": 1,
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/student-report?page=1",
        "last": "https://revisechemistry.org/api/v1/student-report?page=4",
        "prev": null,
        "next": "https://revisechemistry.org/api/v1/student-report?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 4,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student-report?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "https://revisechemistry.org/api/v1/student-report?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student-report?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student-report?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student-report?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/student-report",
        "per_page": 50,
        "to": 50,
        "total": 200
    }
}
```

### Get All Student Report For Specific Student
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "QRHl07Z2PaIs2tum7LhvkDk2I7Qx615kCSsDJjKAKllhVfQlZvt6k1RpPhutuqlAdp4dGGelUtuORbvlbey7idWxu7gP7XiKBNq7yElE2ob5DynD0FsolqAyx9l4l7bLZzJd03pPw8lNz587x73osbwqSiYxibMOenyfaenHn5aOXu1eg2DekfLIlmkNmprcYFU59HHoeUGfHPhWkuvg4RYazPrdex0Vv3lxppKu6tyHiAwVtlb1MgYLYRBB2BJ"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student-report/student", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/student-report/student'));
request.body = json.encode({
  "token": "QRHl07Z2PaIs2tum7LhvkDk2I7Qx615kCSsDJjKAKllhVfQlZvt6k1RpPhutuqlAdp4dGGelUtuORbvlbey7idWxu7gP7XiKBNq7yElE2ob5DynD0FsolqAyx9l4l7bLZzJd03pPw8lNz587x73osbwqSiYxibMOenyfaenHn5aOXu1eg2DekfLIlmkNmprcYFU59HHoeUGfHPhWkuvg4RYazPrdex0Vv3lxppKu6tyHiAwVtlb1MgYLYRBB2BJ"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "current_page": 1,
        "data": [
            {
                "id": 13,
                "user_id": 3,
                "question_answer": "[{\"question_id\":95,\"answer\":\"A\"},{\"question_id\":91,\"answer\":\"B\"},{\"question_id\":86,\"answer\":\"C\"},{\"question_id\":51,\"answer\":\"D\"}]",
                "question_attempted_count": 4,
                "correct_answer_count": 1,
                "created_at": "2021-07-15T02:26:04.000000Z",
                "updated_at": "2021-07-15T02:26:04.000000Z"
            },
            {
                "id": 20,
                "user_id": 3,
                "question_answer": "[{\"question_id\":59,\"answer\":\"A\"},{\"question_id\":78,\"answer\":\"B\"},{\"question_id\":28,\"answer\":\"C\"},{\"question_id\":15,\"answer\":\"D\"}]",
                "question_attempted_count": 4,
                "correct_answer_count": 1,
                "created_at": "2021-07-15T02:26:04.000000Z",
                "updated_at": "2021-07-15T02:26:04.000000Z"
            },
            {
                "id": 150,
                "user_id": 3,
                "question_answer": "[{\"question_id\":55,\"answer\":\"A\"},{\"question_id\":87,\"answer\":\"B\"},{\"question_id\":22,\"answer\":\"C\"},{\"question_id\":37,\"answer\":\"D\"}]",
                "question_attempted_count": 4,
                "correct_answer_count": 3,
                "created_at": "2021-07-15T02:26:04.000000Z",
                "updated_at": "2021-07-15T02:26:04.000000Z"
            }
        ],
        "first_page_url": "https://revisechemistry.org/api/v1/student-report/student?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "https://revisechemistry.org/api/v1/student-report/student?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/student-report/student?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "https://revisechemistry.org/api/v1/student-report/student",
        "per_page": 50,
        "prev_page_url": null,
        "to": 3,
        "total": 3
    }
}
```

### Get Single Student Report
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student-report/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/student-report/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": {
        "id": 1,
        "user_id": 92,
        "question_answer": "[{\"question_id\":13,\"answer\":\"A\"},{\"question_id\":2,\"answer\":\"B\"},{\"question_id\":77,\"answer\":\"C\"},{\"question_id\":74,\"answer\":\"D\"}]",
        "question_attempted_count": 4,
        "correct_answer_count": 0,
        "created_at": "2021-07-15T02:26:04.000000Z",
        "updated_at": "2021-07-15T02:26:04.000000Z"
    }
}
```

### Create/Add New Student Report
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "QRHl07Z2PaIs2tum7LhvkDk2I7Qx615kCSsDJjKAKllhVfQlZvt6k1RpPhutuqlAdp4dGGelUtuORbvlbey7idWxu7gP7XiKBNq7yElE2ob5DynD0FsolqAyx9l4l7bLZzJd03pPw8lNz587x73osbwqSiYxibMOenyfaenHn5aOXu1eg2DekfLIlmkNmprcYFU59HHoeUGfHPhWkuvg4RYazPrdex0Vv3lxppKu6tyHiAwVtlb1MgYLYRBB2BJ",
  "question_answer": [
    {
      "question_id": 2,
      "answer": "A"
    },
    {
      "question_id": 3,
      "answer": "B"
    },
    {
      "question_id": 4,
      "answer": "C"
    },
    {
      "question_id": 5,
      "answer": "D"
    }
  ],
  "question_attempted_count": 10,
  "correct_answer_count": 4
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student-report/", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/student-report/'));
request.body = json.encode({
  "token": "QRHl07Z2PaIs2tum7LhvkDk2I7Qx615kCSsDJjKAKllhVfQlZvt6k1RpPhutuqlAdp4dGGelUtuORbvlbey7idWxu7gP7XiKBNq7yElE2ob5DynD0FsolqAyx9l4l7bLZzJd03pPw8lNz587x73osbwqSiYxibMOenyfaenHn5aOXu1eg2DekfLIlmkNmprcYFU59HHoeUGfHPhWkuvg4RYazPrdex0Vv3lxppKu6tyHiAwVtlb1MgYLYRBB2BJ",
  "question_answer": [
    {
      "question_id": 2,
      "answer": "A"
    },
    {
      "question_id": 3,
      "answer": "B"
    },
    {
      "question_id": 4,
      "answer": "C"
    },
    {
      "question_id": 5,
      "answer": "D"
    }
  ],
  "question_attempted_count": 10,
  "correct_answer_count": 4
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "user_id": 3,
        "question_answer": [
            {
                "question_id": 2,
                "answer": "A"
            },
            {
                "question_id": 3,
                "answer": "B"
            },
            {
                "question_id": 4,
                "answer": "C"
            },
            {
                "question_id": 5,
                "answer": "D"
            }
        ],
        "question_attempted_count": 10,
        "correct_answer_count": 4,
        "message": "New Student report added"
    }
}
```

### Delete Existing Student Report
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/student-report/2", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/student-report/2'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "message": "Student report deleted successfully"
}
```


## Quiz Data API Routes

### Get All Quiz Data
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/quiz'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": [
        {
            "id": 1,
            "question": "Dolorem est fugit ut occaecati.",
            "options": "{\"A\":\"suscipit\",\"B\":\"sint\",\"C\":\"quia\",\"D\":\"nobis\"}",
            "answer": "D",
            "description": "Fuga sequi sit doloremque optio aut. Veniam ut ipsum natus doloremque ducimus eum.",
            "category": "animi",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 2,
            "question": "Et minus voluptatibus perspiciatis consequatur qui.",
            "options": "{\"A\":\"dignissimos\",\"B\":\"quae\",\"C\":\"odit\",\"D\":\"harum\"}",
            "answer": "C",
            "description": "Rerum ullam autem numquam nostrum blanditiis est. Repellat dolores aut dignissimos expedita nihil voluptas. Quo occaecati cumque qui quasi dignissimos. Nam aut ipsam voluptas aut distinctio error quia.",
            "category": "pariatur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 3,
            "question": "Veniam veniam sint similique optio distinctio.",
            "options": "{\"A\":\"necessitatibus\",\"B\":\"sit\",\"C\":\"autem\",\"D\":\"accusamus\"}",
            "answer": "D",
            "description": "Alias eos veritatis ratione quia voluptas. Consequatur porro facere non et amet autem laborum. Consequuntur quod aliquid ipsa. Ut consequatur ullam incidunt repudiandae odio.",
            "category": "sunt",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 4,
            "question": "Laudantium ut expedita expedita at non nisi et animi.",
            "options": "{\"A\":\"aspernatur\",\"B\":\"et\",\"C\":\"cum\",\"D\":\"aut\"}",
            "answer": "D",
            "description": "In at aut est placeat voluptatem. Odio ad autem eum vitae facilis quia. Et consectetur labore quisquam harum et cupiditate veritatis.",
            "category": "illum",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 5,
            "question": "Sunt ipsum quisquam temporibus dolorem repellendus culpa nihil.",
            "options": "{\"A\":\"aut\",\"B\":\"est\",\"C\":\"voluptatem\",\"D\":\"enim\"}",
            "answer": "C",
            "description": "Dolorum dolores non consequuntur recusandae magni. Omnis dolorem id in. Aut et veniam tempora ipsum autem voluptate.",
            "category": "dolorem",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 6,
            "question": "Et omnis vero ea quo deserunt in fugit aut.",
            "options": "{\"A\":\"est\",\"B\":\"dolorum\",\"C\":\"explicabo\",\"D\":\"cupiditate\"}",
            "answer": "D",
            "description": "Cumque porro minima repudiandae voluptatem pariatur omnis. Quidem ut saepe ut natus animi quibusdam repudiandae. Voluptate assumenda reiciendis voluptatum quia incidunt. Vitae animi est labore incidunt sunt est.",
            "category": "inventore",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 7,
            "question": "Omnis natus quidem voluptatum.",
            "options": "{\"A\":\"libero\",\"B\":\"modi\",\"C\":\"illo\",\"D\":\"placeat\"}",
            "answer": "B",
            "description": "Voluptates qui enim harum nobis excepturi similique velit nihil. Quia sed repudiandae debitis. Autem nulla esse animi eos quo ut dolor nihil. Error ea aperiam facilis assumenda qui.",
            "category": "error",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 8,
            "question": "Quo maxime veritatis dolor possimus voluptatem eum.",
            "options": "{\"A\":\"repellendus\",\"B\":\"quae\",\"C\":\"et\",\"D\":\"provident\"}",
            "answer": "A",
            "description": "Et cumque quaerat doloremque dicta rerum explicabo. Velit voluptas numquam quam placeat. Quas et sapiente ipsa voluptates nulla voluptas. Perspiciatis doloribus est qui quaerat commodi eius voluptates non. Ea rerum est qui in qui.",
            "category": "iusto",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 9,
            "question": "Incidunt commodi numquam qui voluptatem et.",
            "options": "{\"A\":\"quisquam\",\"B\":\"est\",\"C\":\"ratione\",\"D\":\"ea\"}",
            "answer": "C",
            "description": "Odio reiciendis doloribus non cupiditate. Aut nesciunt ad voluptatem id tempore. Nihil voluptatibus provident iste praesentium repellat sed voluptatum. Eos at iste quia harum ut ipsum.",
            "category": "fugiat",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 10,
            "question": "Mollitia incidunt eius est voluptas.",
            "options": "{\"A\":\"voluptas\",\"B\":\"dolorum\",\"C\":\"commodi\",\"D\":\"ducimus\"}",
            "answer": "D",
            "description": "Tempore minima eum dolorem voluptatem a esse veniam. Quae qui autem tempora dolores doloremque modi eum.",
            "category": "laboriosam",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 11,
            "question": "Et quia quibusdam deleniti dolores voluptatem.",
            "options": "{\"A\":\"ut\",\"B\":\"corporis\",\"C\":\"velit\",\"D\":\"sed\"}",
            "answer": "D",
            "description": "Ea iure aspernatur sit. Ut omnis illo aut minus. Qui neque quas ut id sint.",
            "category": "et",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 12,
            "question": "Placeat sit illum aliquam dolorem.",
            "options": "{\"A\":\"voluptas\",\"B\":\"atque\",\"C\":\"ut\",\"D\":\"ipsam\"}",
            "answer": "A",
            "description": "Quod voluptatem laborum voluptatem sit possimus perferendis odit ipsum. Nulla cumque libero modi corrupti modi odit voluptas. Ut atque adipisci optio cumque in ratione.",
            "category": "maxime",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 13,
            "question": "Explicabo rerum et consequatur illum nihil vitae at.",
            "options": "{\"A\":\"perspiciatis\",\"B\":\"eos\",\"C\":\"minus\",\"D\":\"sint\"}",
            "answer": "D",
            "description": "Modi consequatur mollitia consequatur enim nihil rerum. Facilis ut in incidunt veritatis et laborum sapiente. Repudiandae et distinctio voluptatum.",
            "category": "consectetur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 14,
            "question": "Saepe accusamus placeat architecto atque reprehenderit voluptatum vero esse.",
            "options": "{\"A\":\"nam\",\"B\":\"eius\",\"C\":\"praesentium\",\"D\":\"nam\"}",
            "answer": "A",
            "description": "Eos aliquid dolorum provident dicta blanditiis et quae. Iste distinctio fuga sed dolorem eveniet deserunt. Laboriosam ut ut laborum laboriosam voluptas rerum. Culpa inventore distinctio autem fuga corporis. Repudiandae molestias modi et et.",
            "category": "enim",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 15,
            "question": "Voluptas beatae quidem sed quisquam velit.",
            "options": "{\"A\":\"aut\",\"B\":\"impedit\",\"C\":\"optio\",\"D\":\"incidunt\"}",
            "answer": "A",
            "description": "Adipisci voluptates expedita corporis. Aliquam at iste non libero. Voluptatibus vero id quia rem assumenda aut. Vel delectus consequatur sunt ea.",
            "category": "ipsa",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 16,
            "question": "Aliquam dolor debitis eum.",
            "options": "{\"A\":\"suscipit\",\"B\":\"exercitationem\",\"C\":\"incidunt\",\"D\":\"alias\"}",
            "answer": "B",
            "description": "Porro magnam vero ipsa iusto. Omnis repudiandae nobis excepturi quis libero assumenda. Impedit quia consequatur ex impedit quasi in.",
            "category": "aperiam",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 17,
            "question": "Nostrum iure sint vel sit inventore cum commodi.",
            "options": "{\"A\":\"placeat\",\"B\":\"vero\",\"C\":\"velit\",\"D\":\"dolorem\"}",
            "answer": "A",
            "description": "Voluptatem qui non ut fuga sunt fuga omnis. Et consequatur fuga numquam amet itaque eveniet. Consequuntur quae officiis autem eaque dolorum ratione. Minus et et sed.",
            "category": "natus",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 18,
            "question": "Magni officia repudiandae ut enim voluptatibus maxime.",
            "options": "{\"A\":\"sed\",\"B\":\"quo\",\"C\":\"ea\",\"D\":\"soluta\"}",
            "answer": "D",
            "description": "Sit voluptatem non molestias ea velit. Et laboriosam eaque sunt aut nihil quia laboriosam illo. Est dolores aliquam et magni numquam accusantium enim.",
            "category": "expedita",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 19,
            "question": "Qui nam consequatur ullam eveniet.",
            "options": "{\"A\":\"in\",\"B\":\"aspernatur\",\"C\":\"eligendi\",\"D\":\"aperiam\"}",
            "answer": "D",
            "description": "Cumque sequi corporis tenetur. Voluptas sunt dolores sit quam necessitatibus veniam quia. Aut et sunt et voluptatem et tempore.",
            "category": "aspernatur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 20,
            "question": "Eum quos eum modi fugiat.",
            "options": "{\"A\":\"quam\",\"B\":\"laboriosam\",\"C\":\"temporibus\",\"D\":\"odit\"}",
            "answer": "C",
            "description": "Animi deserunt voluptatem nobis repudiandae. Vel laudantium accusamus atque.",
            "category": "minus",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 21,
            "question": "Et neque corporis quis.",
            "options": "{\"A\":\"autem\",\"B\":\"odit\",\"C\":\"eveniet\",\"D\":\"quisquam\"}",
            "answer": "D",
            "description": "Ut quia voluptates doloremque sint. Voluptatibus amet doloribus a laudantium. Est praesentium sit est cupiditate cupiditate quia consequuntur. Officiis molestiae officiis voluptas eaque ex reiciendis voluptatem.",
            "category": "mollitia",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 22,
            "question": "Et ut quia ipsum et inventore sed non.",
            "options": "{\"A\":\"eum\",\"B\":\"nostrum\",\"C\":\"facilis\",\"D\":\"inventore\"}",
            "answer": "D",
            "description": "Atque aut culpa nulla porro accusantium. Ut labore quibusdam dolorem hic non ab molestias. Dicta ipsum et officiis voluptates aut nostrum veritatis.",
            "category": "eveniet",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 23,
            "question": "Blanditiis ducimus sint in earum eum atque animi.",
            "options": "{\"A\":\"quaerat\",\"B\":\"dolorem\",\"C\":\"qui\",\"D\":\"nihil\"}",
            "answer": "C",
            "description": "Et est neque beatae facilis velit ullam. Vitae tempore eos ut saepe ea. Rerum natus et quo assumenda repudiandae perspiciatis culpa. Alias est sunt ad distinctio atque possimus quasi consectetur.",
            "category": "dolorem",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 24,
            "question": "Eius molestiae voluptatem sunt a.",
            "options": "{\"A\":\"quia\",\"B\":\"eveniet\",\"C\":\"illo\",\"D\":\"velit\"}",
            "answer": "A",
            "description": "Consequatur et ducimus dolor perspiciatis cum est quis. Ut quibusdam quam omnis minima. Doloremque inventore molestias eligendi corporis.",
            "category": "ut",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 25,
            "question": "Quod ut facere laborum ipsum sint.",
            "options": "{\"A\":\"qui\",\"B\":\"possimus\",\"C\":\"dolores\",\"D\":\"facere\"}",
            "answer": "C",
            "description": "Illum accusantium quidem deserunt dolorem tenetur ullam perferendis. Ipsa omnis temporibus aut hic nihil et quia corrupti.",
            "category": "sequi",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 26,
            "question": "Enim quia placeat enim quia et ut temporibus autem.",
            "options": "{\"A\":\"velit\",\"B\":\"excepturi\",\"C\":\"nemo\",\"D\":\"ad\"}",
            "answer": "C",
            "description": "Nam vero amet ab ratione consequatur dolor ex. Nam quae ut voluptas accusamus eaque iusto. Id esse dolorem non dicta necessitatibus omnis nihil. Et et eaque velit.",
            "category": "aliquid",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 27,
            "question": "Consequuntur ipsam quo ad aut nostrum provident aut.",
            "options": "{\"A\":\"quae\",\"B\":\"sed\",\"C\":\"odio\",\"D\":\"voluptatem\"}",
            "answer": "D",
            "description": "Enim impedit mollitia quo nostrum. Qui ut ea illum tempore et deserunt. Possimus recusandae consequatur ut sit et inventore.",
            "category": "consequuntur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 28,
            "question": "Delectus suscipit sed ipsam sequi.",
            "options": "{\"A\":\"ipsum\",\"B\":\"vel\",\"C\":\"provident\",\"D\":\"quia\"}",
            "answer": "D",
            "description": "Deserunt et ea consequuntur quidem aut laboriosam consectetur. Ratione quam incidunt minima eos fugit.",
            "category": "distinctio",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 29,
            "question": "Accusantium architecto non iusto fugit.",
            "options": "{\"A\":\"blanditiis\",\"B\":\"molestiae\",\"C\":\"beatae\",\"D\":\"vitae\"}",
            "answer": "D",
            "description": "Ipsam quos commodi dolorem temporibus dolore ut voluptatem quaerat. Aut expedita soluta est aut distinctio architecto in quam. Adipisci sed impedit rerum perferendis.",
            "category": "dolorem",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 30,
            "question": "Temporibus sed assumenda veritatis porro voluptatem corporis dolor.",
            "options": "{\"A\":\"maxime\",\"B\":\"et\",\"C\":\"tenetur\",\"D\":\"neque\"}",
            "answer": "B",
            "description": "Esse velit quis velit aut voluptas omnis. Non corrupti consequuntur aut iste qui aut nesciunt.",
            "category": "et",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 31,
            "question": "Et maiores ipsum ut sit sunt.",
            "options": "{\"A\":\"tempora\",\"B\":\"eius\",\"C\":\"ut\",\"D\":\"praesentium\"}",
            "answer": "B",
            "description": "Id aut quibusdam rem et ipsam. Dignissimos sunt repellendus unde dolores rerum reprehenderit enim. Consequatur iure itaque harum beatae aut velit officia.",
            "category": "consequatur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 32,
            "question": "Dolores iusto est optio voluptatum perferendis perferendis praesentium.",
            "options": "{\"A\":\"magni\",\"B\":\"quibusdam\",\"C\":\"natus\",\"D\":\"reiciendis\"}",
            "answer": "A",
            "description": "Provident sit qui sed omnis consequuntur cumque distinctio incidunt. Esse temporibus soluta consequuntur ut dolor expedita nam. Perspiciatis repellendus neque et qui. Explicabo reprehenderit expedita saepe suscipit cupiditate ut.",
            "category": "vel",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 33,
            "question": "Nemo commodi quis neque incidunt est vel.",
            "options": "{\"A\":\"nostrum\",\"B\":\"earum\",\"C\":\"mollitia\",\"D\":\"inventore\"}",
            "answer": "B",
            "description": "Labore consequuntur deleniti exercitationem assumenda consectetur. Nemo dicta ducimus optio architecto sint. Et reprehenderit facilis accusamus et.",
            "category": "rem",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 34,
            "question": "Placeat doloremque dicta rerum eveniet mollitia vero laboriosam.",
            "options": "{\"A\":\"omnis\",\"B\":\"repellat\",\"C\":\"ipsa\",\"D\":\"repellendus\"}",
            "answer": "C",
            "description": "Neque vel est et. Inventore ea quo voluptas reprehenderit rem qui voluptatem. Omnis consectetur id laudantium accusamus id et sed saepe. Similique minus autem consequatur eos commodi incidunt sint.",
            "category": "quam",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 35,
            "question": "Itaque dolore est qui qui placeat reiciendis.",
            "options": "{\"A\":\"voluptas\",\"B\":\"error\",\"C\":\"est\",\"D\":\"sapiente\"}",
            "answer": "B",
            "description": "Quo omnis officia est. Deleniti maxime et iste quibusdam veritatis omnis. Et veniam natus ut ducimus quae soluta.",
            "category": "suscipit",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 36,
            "question": "Error ut beatae mollitia ratione nostrum ullam.",
            "options": "{\"A\":\"nisi\",\"B\":\"laudantium\",\"C\":\"alias\",\"D\":\"sunt\"}",
            "answer": "A",
            "description": "Nostrum animi provident sed asperiores impedit quia. Esse cum corrupti expedita. Sit facere sunt omnis sit quos voluptatem non ex. Ut quae sint consequatur modi amet voluptatem.",
            "category": "magni",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 37,
            "question": "Voluptas eum qui aut labore sed accusantium.",
            "options": "{\"A\":\"necessitatibus\",\"B\":\"molestias\",\"C\":\"magni\",\"D\":\"ea\"}",
            "answer": "B",
            "description": "A nulla occaecati in et sed qui. Culpa perferendis impedit quae aut omnis voluptatibus. Ut occaecati quos necessitatibus molestiae ducimus.",
            "category": "impedit",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 38,
            "question": "Magnam at aut ut et sunt.",
            "options": "{\"A\":\"fuga\",\"B\":\"accusantium\",\"C\":\"rerum\",\"D\":\"eius\"}",
            "answer": "D",
            "description": "Placeat sint adipisci sit eius animi fuga. Itaque distinctio autem vel eum dolor commodi. Est id molestias quia sapiente. Ipsa consequuntur debitis iure in vero et.",
            "category": "est",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 39,
            "question": "Voluptate nesciunt odio magni dolor ratione nostrum impedit.",
            "options": "{\"A\":\"earum\",\"B\":\"incidunt\",\"C\":\"tempore\",\"D\":\"quos\"}",
            "answer": "C",
            "description": "Enim est praesentium quam architecto. Consequuntur ea voluptates ratione aut dignissimos accusantium vel. Numquam maxime neque inventore molestiae. Quasi voluptatem quis deleniti laborum qui.",
            "category": "quis",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 40,
            "question": "Et non omnis eos atque non hic.",
            "options": "{\"A\":\"minima\",\"B\":\"rerum\",\"C\":\"laboriosam\",\"D\":\"dolore\"}",
            "answer": "A",
            "description": "Saepe omnis quia sunt quia. Ad rerum saepe voluptatem alias qui ut. Vel porro repudiandae aut est aspernatur suscipit odio nam.",
            "category": "voluptatem",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 41,
            "question": "Aut quia officia magni iusto.",
            "options": "{\"A\":\"nihil\",\"B\":\"placeat\",\"C\":\"architecto\",\"D\":\"quasi\"}",
            "answer": "D",
            "description": "Non id quis iste. Iste praesentium facere magnam est veritatis vitae illo. Et dolores quaerat laudantium aut.",
            "category": "minima",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 42,
            "question": "Deleniti et rem consequatur non voluptatem impedit.",
            "options": "{\"A\":\"molestiae\",\"B\":\"qui\",\"C\":\"atque\",\"D\":\"animi\"}",
            "answer": "D",
            "description": "Voluptatum non autem distinctio nobis. Doloribus corrupti rerum eaque placeat fugit. Aut modi totam et nostrum non.",
            "category": "aspernatur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 43,
            "question": "Error numquam minima quidem voluptas sapiente voluptatibus.",
            "options": "{\"A\":\"quaerat\",\"B\":\"accusamus\",\"C\":\"molestiae\",\"D\":\"quia\"}",
            "answer": "C",
            "description": "Minima praesentium sequi sed ratione voluptatibus. Et adipisci est ea minus. Modi ullam eum doloribus non est nisi non itaque.",
            "category": "assumenda",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 44,
            "question": "Hic vel placeat praesentium perspiciatis in illo eligendi.",
            "options": "{\"A\":\"dolor\",\"B\":\"praesentium\",\"C\":\"nulla\",\"D\":\"ut\"}",
            "answer": "B",
            "description": "Quis unde est autem culpa reprehenderit. Eos saepe modi ea ipsam molestias. Repellendus quas quod dolor nesciunt rem facilis. Animi et in tempore dolor autem.",
            "category": "ut",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 45,
            "question": "Corrupti et nihil facere quam.",
            "options": "{\"A\":\"fuga\",\"B\":\"et\",\"C\":\"quidem\",\"D\":\"nihil\"}",
            "answer": "C",
            "description": "Qui molestias repellendus velit et. Laborum voluptatem ut labore sit consectetur aspernatur. Velit nobis eos tenetur ipsum quos.",
            "category": "consectetur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 46,
            "question": "Necessitatibus sunt voluptates dolorem ut odit sequi.",
            "options": "{\"A\":\"provident\",\"B\":\"totam\",\"C\":\"omnis\",\"D\":\"ut\"}",
            "answer": "A",
            "description": "Dolorum cupiditate voluptatum exercitationem quidem eum. Quo commodi aperiam voluptatibus quia sit. Vel facere eligendi ut placeat quae vero.",
            "category": "dignissimos",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 47,
            "question": "Quo ut dolorum possimus similique ducimus cupiditate.",
            "options": "{\"A\":\"illum\",\"B\":\"in\",\"C\":\"dolore\",\"D\":\"dolore\"}",
            "answer": "B",
            "description": "Nulla magni dolores aut quis amet optio. Sed sunt voluptates aut qui sapiente eos. Asperiores non dicta hic. Animi velit dolorem provident modi quasi deleniti perspiciatis. Animi et molestiae vel esse ullam.",
            "category": "velit",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 48,
            "question": "Nesciunt ut consequatur dolores quibusdam voluptatem id deleniti tempora.",
            "options": "{\"A\":\"amet\",\"B\":\"eveniet\",\"C\":\"ratione\",\"D\":\"distinctio\"}",
            "answer": "C",
            "description": "Ut dolorem eligendi vel dolor minima. Eveniet quo sed rem. Est ut facere vero voluptas possimus est modi.",
            "category": "perspiciatis",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 49,
            "question": "Quasi distinctio qui rerum neque et enim.",
            "options": "{\"A\":\"sapiente\",\"B\":\"minima\",\"C\":\"asperiores\",\"D\":\"deleniti\"}",
            "answer": "A",
            "description": "Officia qui tenetur molestias inventore iure possimus. Esse maiores sunt atque placeat quos. Saepe placeat voluptatem ullam et optio.",
            "category": "pariatur",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        },
        {
            "id": 50,
            "question": "Culpa quia possimus itaque minus dignissimos quam rerum quisquam.",
            "options": "{\"A\":\"laudantium\",\"B\":\"consequatur\",\"C\":\"ut\",\"D\":\"voluptatibus\"}",
            "answer": "D",
            "description": "Perspiciatis aliquam animi voluptates qui aut ut odio nobis. Assumenda qui id sint vero similique. Delectus eius omnis odit.",
            "category": "molestias",
            "created_at": "2021-07-15T02:26:04.000000Z",
            "updated_at": "2021-07-15T02:26:04.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/quiz?page=1",
        "last": "https://revisechemistry.org/api/v1/quiz?page=4",
        "prev": null,
        "next": "https://revisechemistry.org/api/v1/quiz?page=2"
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 4,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz?page=2",
                "label": "2",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz?page=3",
                "label": "3",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz?page=4",
                "label": "4",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz?page=2",
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/quiz",
        "per_page": 50,
        "to": 50,
        "total": 200
    }
}
```
### Get All Quiz Data For Specific Quiz Chapter
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "chapter": "et"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz/category/chapter", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/quiz/category/chapter'));
request.body = json.encode({
  "chapter": "et"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "current_page": 1,
        "data": [
            {
                "id": 1,
                "question": "Explicabo velit ut quam.",
                "options": "{\"A\":\"reiciendis\",\"B\":\"quia\",\"C\":\"rem\",\"D\":\"neque\"}",
                "answer": "C",
                "description": "Architecto magnam sed id excepturi. Labore voluptatum est quibusdam vel. Cum voluptatem magni dolores culpa quod numquam ut. Molestiae doloribus laborum neque.",
                "chapter": "et",
                "category": "ut",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 19,
                "question": "Quia voluptas temporibus ut.",
                "options": "{\"A\":\"totam\",\"B\":\"ipsum\",\"C\":\"tempora\",\"D\":\"aut\"}",
                "answer": "D",
                "description": "Autem magnam ut sed. Distinctio quaerat odit et architecto velit aliquid laborum. Ut eum tenetur libero animi numquam.",
                "chapter": "et",
                "category": "rerum",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 24,
                "question": "Inventore sed molestias voluptas et.",
                "options": "{\"A\":\"qui\",\"B\":\"quasi\",\"C\":\"dolore\",\"D\":\"ipsam\"}",
                "answer": "A",
                "description": "Nulla qui impedit autem in. Repellat accusantium nihil nam qui consectetur. Eos hic iste architecto omnis est vitae.",
                "chapter": "et",
                "category": "qui",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 32,
                "question": "Placeat eius praesentium eveniet provident beatae odio iste.",
                "options": "{\"A\":\"rerum\",\"B\":\"perferendis\",\"C\":\"eligendi\",\"D\":\"deserunt\"}",
                "answer": "C",
                "description": "Ad laboriosam explicabo et qui perspiciatis inventore dolorum. Error ut et omnis minus rerum. Deleniti molestiae sed ipsam quasi labore voluptatum.",
                "chapter": "tenetur",
                "category": "tempore",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 46,
                "question": "Explicabo sunt minus aliquid accusamus.",
                "options": "{\"A\":\"corporis\",\"B\":\"maxime\",\"C\":\"quia\",\"D\":\"voluptatem\"}",
                "answer": "C",
                "description": "Aut soluta accusamus quo voluptatem non. Fuga voluptatem accusantium corrupti. Totam numquam atque tenetur modi. Nisi ea eius consequatur aut occaecati voluptatibus pariatur quia. Et doloribus non vitae provident velit quo ipsum aliquam.",
                "chapter": "et",
                "category": "nobis",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 67,
                "question": "Earum natus unde nisi magnam.",
                "options": "{\"A\":\"voluptas\",\"B\":\"beatae\",\"C\":\"numquam\",\"D\":\"aliquam\"}",
                "answer": "D",
                "description": "Eveniet sint pariatur deserunt distinctio sapiente quia debitis. Cumque similique dolores accusantium voluptatum. Est aut sunt autem illo.",
                "chapter": "et",
                "category": "dolorum",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 70,
                "question": "Et dolor omnis totam adipisci et illum quia.",
                "options": "{\"A\":\"illo\",\"B\":\"quia\",\"C\":\"veritatis\",\"D\":\"et\"}",
                "answer": "A",
                "description": "Et distinctio sint illum quae repudiandae. Quod aut aspernatur nobis odit aut tempore. Mollitia possimus voluptates eum odio nesciunt minima culpa nisi. Natus eveniet soluta quam debitis.",
                "chapter": "et",
                "category": "voluptas",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 87,
                "question": "Aut nihil vel distinctio voluptatibus illum eligendi omnis.",
                "options": "{\"A\":\"quo\",\"B\":\"voluptatem\",\"C\":\"earum\",\"D\":\"rem\"}",
                "answer": "B",
                "description": "Tempore cumque molestias itaque rerum sed. Et cumque est laborum incidunt aut. Praesentium nihil vero temporibus et blanditiis libero et.",
                "chapter": "et",
                "category": "eos",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 100,
                "question": "A doloremque est nostrum ab id ad.",
                "options": "{\"A\":\"aut\",\"B\":\"deserunt\",\"C\":\"nihil\",\"D\":\"ut\"}",
                "answer": "A",
                "description": "Cum ea saepe blanditiis voluptatem. Dolores quis qui at. Eligendi iusto fuga consequatur quod. Aut eum aliquam sunt autem perferendis ipsam deserunt eos.",
                "chapter": "consectetur",
                "category": "enim",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 111,
                "question": "Totam vel quia voluptatum ipsum.",
                "options": "{\"A\":\"ratione\",\"B\":\"fugit\",\"C\":\"voluptates\",\"D\":\"ducimus\"}",
                "answer": "C",
                "description": "Et quia hic accusamus repellendus. Sit quod consequatur numquam voluptatem ipsam in eius. Qui voluptates nisi reprehenderit et.",
                "chapter": "consectetur",
                "category": "impedit",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 115,
                "question": "Impedit temporibus voluptatem laboriosam doloribus officiis a temporibus.",
                "options": "{\"A\":\"odio\",\"B\":\"perferendis\",\"C\":\"ab\",\"D\":\"in\"}",
                "answer": "D",
                "description": "Provident nemo voluptate doloremque sit. Maiores nihil qui debitis beatae quo quia ipsam. Voluptatum id officiis iusto in repellat. Aliquid voluptatem voluptatem odio quam autem.",
                "chapter": "amet",
                "category": "voluptatem",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 116,
                "question": "Nihil inventore assumenda atque similique.",
                "options": "{\"A\":\"officiis\",\"B\":\"nemo\",\"C\":\"fugiat\",\"D\":\"sit\"}",
                "answer": "C",
                "description": "Id aspernatur et soluta inventore qui accusantium. Aut aliquam occaecati occaecati amet voluptatibus vel accusantium. Exercitationem tempore eveniet reprehenderit quae. Quasi et non amet consequatur cum sunt.",
                "chapter": "et",
                "category": "sit",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 158,
                "question": "Tempora facilis sit alias fuga.",
                "options": "{\"A\":\"cumque\",\"B\":\"et\",\"C\":\"libero\",\"D\":\"illum\"}",
                "answer": "C",
                "description": "Placeat quis iusto voluptatem eos voluptatem. Officiis iusto velit rerum ea occaecati voluptates. Alias voluptas voluptatem et.",
                "chapter": "et",
                "category": "consequatur",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 165,
                "question": "Corrupti facere aut id quis saepe.",
                "options": "{\"A\":\"id\",\"B\":\"et\",\"C\":\"et\",\"D\":\"eaque\"}",
                "answer": "C",
                "description": "Quo eos illo vero dolorum aut aut. Ullam autem vitae quibusdam pariatur. Ut voluptatem voluptates quasi nemo magnam. Eaque cum velit eum et aliquid et quia voluptatum.",
                "chapter": "amet",
                "category": "sunt",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 182,
                "question": "Rerum modi pariatur expedita dicta.",
                "options": "{\"A\":\"aut\",\"B\":\"consequatur\",\"C\":\"quo\",\"D\":\"omnis\"}",
                "answer": "D",
                "description": "Dolores odio qui cumque nesciunt. Veritatis et sed sit et id quos. Eos et quia atque quo dolor maiores quod. Corporis voluptatem inventore vitae voluptatem.",
                "chapter": "eveniet",
                "category": "odio",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            },
            {
                "id": 185,
                "question": "Et quasi iste nihil fugit esse earum aut.",
                "options": "{\"A\":\"voluptas\",\"B\":\"ab\",\"C\":\"nihil\",\"D\":\"et\"}",
                "answer": "D",
                "description": "Architecto vitae cupiditate dicta. Voluptate ut sint rem suscipit omnis. Corporis similique voluptatem repudiandae sequi nesciunt est qui.",
                "chapter": "consectetur",
                "category": "est",
                "created_at": "2021-07-27T03:17:43.000000Z",
                "updated_at": "2021-07-27T03:17:43.000000Z"
            }
        ],
        "first_page_url": "https://revisechemistry.org/api/v1/quiz/category/chapter?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "https://revisechemistry.org/api/v1/quiz/category/chapter?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz/category/chapter?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "https://revisechemistry.org/api/v1/quiz/category/chapter",
        "per_page": 100,
        "prev_page_url": null,
        "to": 16,
        "total": 16
    }
}
```


### Get All Quiz Data For Specific Quiz Category
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "category": "animi"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz/category", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/quiz/category'));
request.body = json.encode({
  "category": "animi"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "current_page": 1,
        "data": [
            {
                "id": 1,
                "question": "Dolorem est fugit ut occaecati.",
                "options": "{\"A\":\"suscipit\",\"B\":\"sint\",\"C\":\"quia\",\"D\":\"nobis\"}",
                "answer": "D",
                "description": "Fuga sequi sit doloremque optio aut. Veniam ut ipsum natus doloremque ducimus eum.",
                "category": "animi",
                "created_at": "2021-07-15T02:26:04.000000Z",
                "updated_at": "2021-07-15T02:26:04.000000Z"
            },
            {
                "id": 118,
                "question": "Fugiat nisi velit eaque.",
                "options": "{\"A\":\"eligendi\",\"B\":\"et\",\"C\":\"voluptatem\",\"D\":\"est\"}",
                "answer": "D",
                "description": "Repellat id voluptatem est. Debitis quibusdam ea reiciendis pariatur omnis atque voluptas. Molestiae similique veritatis voluptatibus ad. Vel itaque nam aut commodi magnam laboriosam.",
                "category": "animi",
                "created_at": "2021-07-15T02:26:04.000000Z",
                "updated_at": "2021-07-15T02:26:04.000000Z"
            }
        ],
        "first_page_url": "https://revisechemistry.org/api/v1/quiz/category?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "https://revisechemistry.org/api/v1/quiz/category?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/quiz/category?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "https://revisechemistry.org/api/v1/quiz/category",
        "per_page": 100,
        "prev_page_url": null,
        "to": 2,
        "total": 2
    }
}
```

### Get Single Quiz Data
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/quiz/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": {
        "id": 1,
        "question": "Dolorem est fugit ut occaecati.",
        "options": "{\"A\":\"suscipit\",\"B\":\"sint\",\"C\":\"quia\",\"D\":\"nobis\"}",
        "answer": "D",
        "description": "Fuga sequi sit doloremque optio aut. Veniam ut ipsum natus doloremque ducimus eum.",
        "category": "animi",
        "created_at": "2021-07-15T02:26:04.000000Z",
        "updated_at": "2021-07-15T02:26:04.000000Z"
    }
}
```

### Create/Add New Quiz Data
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "question": "You can change other options as well",
  "options": {
    "A": "First",
    "B": "Second",
    "C": "Third",
    "D": "Fourth"
  },
  "answer": "C",
  "description": "New description",
  "category": "Physics"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/quiz'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "question": "You can change other options as well",
  "options": {
    "A": "First",
    "B": "Second",
    "C": "Third",
    "D": "Fourth"
  },
  "answer": "C",
  "description": "New description",
  "category": "Physics"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "question": "You can change other options as well",
        "options": {
            "A": "First",
            "B": "Second",
            "C": "Third",
            "D": "Fourth"
        },
        "answer": "C",
        "description": "New description",
        "category": "Physics",
        "message": "New Quiz questions added"
    }
}
```

### Edit Existing Quiz Data
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "question": "You can change other options as well",
  "options": {
    "A": "First",
    "B": "Second",
    "C": "Third",
    "D": "Fourth"
  },
  "answer": "C",
  "description": "New description",
  "category": "Physics"
});

var requestOptions = {
  method: 'PUT',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('PUT', Uri.parse('https://revisechemistry.org/api/v1/quiz/1'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB",
  "question": "You can change other options as well",
  "options": {
    "A": "First",
    "B": "Second",
    "C": "Third",
    "D": "Fourth"
  },
  "answer": "C",
  "description": "New description",
  "category": "Physics"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 1,
        "question": "You can change other options as well",
        "options": {
            "A": "First",
            "B": "Second",
            "C": "Third",
            "D": "Fourth"
        },
        "answer": "C",
        "description": "New description",
        "category": "Physics"
    },
    "message": "Quiz question updated successfully"
}
```

### Delete Existing Quiz Data
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/quiz/3", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/quiz/3'));
request.body = json.encode({
  "token": "ZDaiO8yP0QxcWyjxUuNgREqtijGlqcpTEA1FP4pF8zoYZlgCMQ7siygFFb5BMWRMziDXdhnzYB6rgDJ1QKVYnxFlU1UUKQixwXXUURRedVzMeQ522vBmJZn1wJhPA5xpfcuyilK0y2Yud6CzyxwmjTSllwLSJcQ4vtLh2pDLbTQ3Y1TyWqGCL99iHsKSTf0gy6ry4uGWuBz6cY9GbIUHTLfiS37A6uMtFIYyxuE3ioSkTwrVlGMHlLtFl2ybYcB"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "message": "Quiz questions deleted successfully"
}
```


## Notes API Routes

### Get All Notes
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/note'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

``json
{
    "data": [
        {
            "id": 1,
            "chapter": "qui",
            "category": "consequuntur",
            "notes": "Fugit id ratione voluptate deserunt aut reiciendis. Architecto beatae ut dolores ut nisi dignissimos. Facilis ea mollitia ut nihil et repudiandae reprehenderit. Velit maxime modi aut facere deleniti accusamus. Ut dolor ut quia in aliquid qui. Quibusdam iusto eius perferendis culpa quis qui dolorem consequatur. Dignissimos dolorem itaque omnis cupiditate consequuntur consequuntur eos. Voluptatem reiciendis soluta quisquam qui. Est quia eligendi voluptatem. Pariatur voluptatibus nostrum cumque et molestiae ea. Consequatur enim ratione aspernatur et enim. Unde nulla aut ratione aut suscipit. Qui aut fuga voluptatem est quia quidem enim. Ut ducimus nostrum quo eaque.",
            "created_at": "2021-07-27T03:17:55.000000Z",
            "updated_at": "2021-07-27T03:17:55.000000Z"
        }
    ],
    "links": {
        "first": "https://revisechemistry.org/api/v1/note?page=1",
        "last": "https://revisechemistry.org/api/v1/note?page=1",
        "prev": null,
        "next": null
    },
    "meta": {
        "current_page": 1,
        "from": 1,
        "last_page": 1,
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/note?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "path": "https://revisechemistry.org/api/v1/note",
        "per_page": 50,
        "to": 1,
        "total": 1
    }
}
```

### Get A Single Note
```js
var requestOptions = {
  method: 'GET',
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var request = http.Request('GET', Uri.parse('https://revisechemistry.org/api/v1/note/1'));


http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "data": {
        "id": 1,
        "chapter": "qui",
        "category": "consequuntur",
        "notes": "Fugit id ratione voluptate deserunt aut reiciendis. Architecto beatae ut dolores ut nisi dignissimos. Facilis ea mollitia ut nihil et repudiandae reprehenderit. Velit maxime modi aut facere deleniti accusamus. Ut dolor ut quia in aliquid qui. Quibusdam iusto eius perferendis culpa quis qui dolorem consequatur. Dignissimos dolorem itaque omnis cupiditate consequuntur consequuntur eos. Voluptatem reiciendis soluta quisquam qui. Est quia eligendi voluptatem. Pariatur voluptatibus nostrum cumque et molestiae ea. Consequatur enim ratione aspernatur et enim. Unde nulla aut ratione aut suscipit. Qui aut fuga voluptatem est quia quidem enim. Ut ducimus nostrum quo eaque.",
        "created_at": "2021-07-27T03:17:55.000000Z",
        "updated_at": "2021-07-27T03:17:55.000000Z"
    }
}
```

### Create New Note
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "uNTaIBJEqPTyVthi0sUelUUISdz74V4px3It7KCnWjSPwZZaVD4CbcGcevLKzdUvi12JeMgV7MXRlbZGgF2laGsB7iXAFLTDbUTolYyIAgWlNPzLgc9UdDNw6RPQJrZmvp0hrK5adhPZ2CoDvhh3KfXrmGyhnCWes4njuHTi4bsXGiYYOoioC28bljSQzEhK4gO9lgFOPZHLXwoyZxiaW72WyLL9VFrV2FFhZHdIoyYApgC8ri29nu0DsqdYfnZ",
  "chapter": "force",
  "category": "physic",
  "notes": "lorem ipsum and more dummy text"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/note'));
request.body = json.encode({
  "token": "uNTaIBJEqPTyVthi0sUelUUISdz74V4px3It7KCnWjSPwZZaVD4CbcGcevLKzdUvi12JeMgV7MXRlbZGgF2laGsB7iXAFLTDbUTolYyIAgWlNPzLgc9UdDNw6RPQJrZmvp0hrK5adhPZ2CoDvhh3KfXrmGyhnCWes4njuHTi4bsXGiYYOoioC28bljSQzEhK4gO9lgFOPZHLXwoyZxiaW72WyLL9VFrV2FFhZHdIoyYApgC8ri29nu0DsqdYfnZ",
  "chapter": "force",
  "category": "physic",
  "notes": "lorem ipsum and more dummy text"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "chapter": "force",
        "category": "physic",
        "notes": "lorem ipsum and more dummy text",
        "message": "New Notes added"
    }
}
```

### Update Existing Note
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "uNTaIBJEqPTyVthi0sUelUUISdz74V4px3It7KCnWjSPwZZaVD4CbcGcevLKzdUvi12JeMgV7MXRlbZGgF2laGsB7iXAFLTDbUTolYyIAgWlNPzLgc9UdDNw6RPQJrZmvp0hrK5adhPZ2CoDvhh3KfXrmGyhnCWes4njuHTi4bsXGiYYOoioC28bljSQzEhK4gO9lgFOPZHLXwoyZxiaW72WyLL9VFrV2FFhZHdIoyYApgC8ri29nu0DsqdYfnZ",
  "chapter": "force",
  "category": "physic",
  "notes": "lorem ipsum and more dummy text"
});

var requestOptions = {
  method: 'PUT',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('PUT', Uri.parse('https://revisechemistry.org/api/v1/note/1'));
request.body = json.encode({
  "token": "uNTaIBJEqPTyVthi0sUelUUISdz74V4px3It7KCnWjSPwZZaVD4CbcGcevLKzdUvi12JeMgV7MXRlbZGgF2laGsB7iXAFLTDbUTolYyIAgWlNPzLgc9UdDNw6RPQJrZmvp0hrK5adhPZ2CoDvhh3KfXrmGyhnCWes4njuHTi4bsXGiYYOoioC28bljSQzEhK4gO9lgFOPZHLXwoyZxiaW72WyLL9VFrV2FFhZHdIoyYApgC8ri29nu0DsqdYfnZ",
  "chapter": "force",
  "category": "physic",
  "notes": "lorem ipsum and more dummy text"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "id": 1,
        "chapter": "force",
        "category": "physic",
        "notes": "lorem ipsum and more dummy text"
    },
    "message": "Note updated successfully"
}
```

### Delete Existing Note
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "token": "uNTaIBJEqPTyVthi0sUelUUISdz74V4px3It7KCnWjSPwZZaVD4CbcGcevLKzdUvi12JeMgV7MXRlbZGgF2laGsB7iXAFLTDbUTolYyIAgWlNPzLgc9UdDNw6RPQJrZmvp0hrK5adhPZ2CoDvhh3KfXrmGyhnCWes4njuHTi4bsXGiYYOoioC28bljSQzEhK4gO9lgFOPZHLXwoyZxiaW72WyLL9VFrV2FFhZHdIoyYApgC8ri29nu0DsqdYfnZ"
});

var requestOptions = {
  method: 'DELETE',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note/1", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('DELETE', Uri.parse('https://revisechemistry.org/api/v1/note/1'));
request.body = json.encode({
  "token": "uNTaIBJEqPTyVthi0sUelUUISdz74V4px3It7KCnWjSPwZZaVD4CbcGcevLKzdUvi12JeMgV7MXRlbZGgF2laGsB7iXAFLTDbUTolYyIAgWlNPzLgc9UdDNw6RPQJrZmvp0hrK5adhPZ2CoDvhh3KfXrmGyhnCWes4njuHTi4bsXGiYYOoioC28bljSQzEhK4gO9lgFOPZHLXwoyZxiaW72WyLL9VFrV2FFhZHdIoyYApgC8ri29nu0DsqdYfnZ"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "message": "Notes deleted successfully"
}
```

### Get All Note Data For Specific Note Category
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "category": "physic"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note/category", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/note/category'));
request.body = json.encode({
  "category": "physic"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "current_page": 1,
        "data": [
            {
                "id": 2,
                "chapter": "force",
                "category": "physic",
                "notes": "lorem ipsum and more dummy text",
                "created_at": "2021-07-27T03:24:27.000000Z",
                "updated_at": "2021-07-27T03:24:27.000000Z"
            }
        ],
        "first_page_url": "https://revisechemistry.org/api/v1/note/category?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "https://revisechemistry.org/api/v1/note/category?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/note/category?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "https://revisechemistry.org/api/v1/note/category",
        "per_page": 100,
        "prev_page_url": null,
        "to": 1,
        "total": 1
    }
}
```

### Get All Note Data For Specific Note Chapter
```js
var myHeaders = new Headers();
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "chapter": "force"
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://revisechemistry.org/api/v1/note/category/chapter", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));
```

```dart
var headers = {
  'Content-Type': 'application/json'
};
var request = http.Request('POST', Uri.parse('https://revisechemistry.org/api/v1/note/category/chapter'));
request.body = json.encode({
  "chapter": "force"
});
request.headers.addAll(headers);

http.StreamedResponse response = await request.send();

if (response.statusCode == 200) {
  print(await response.stream.bytesToString());
}
else {
  print(response.reasonPhrase);
}
```

```json
{
    "response": {
        "current_page": 1,
        "data": [
            {
                "id": 2,
                "chapter": "force",
                "category": "physic",
                "notes": "lorem ipsum and more dummy text",
                "created_at": "2021-07-27T03:24:27.000000Z",
                "updated_at": "2021-07-27T03:24:27.000000Z"
            }
        ],
        "first_page_url": "https://revisechemistry.org/api/v1/note/category/chapter?page=1",
        "from": 1,
        "last_page": 1,
        "last_page_url": "https://revisechemistry.org/api/v1/note/category/chapter?page=1",
        "links": [
            {
                "url": null,
                "label": "&laquo; Previous",
                "active": false
            },
            {
                "url": "https://revisechemistry.org/api/v1/note/category/chapter?page=1",
                "label": "1",
                "active": true
            },
            {
                "url": null,
                "label": "Next &raquo;",
                "active": false
            }
        ],
        "next_page_url": null,
        "path": "https://revisechemistry.org/api/v1/note/category/chapter",
        "per_page": 100,
        "prev_page_url": null,
        "to": 1,
        "total": 1
    }
}
```
