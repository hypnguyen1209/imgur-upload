# imgur-upload
Project cũ, giờ mới đăng :&lt;
```
var feedback = function(res) {
    if (res.success === true) {
        var get_link = res.data.link.replace(/^http:\/\//i, 'https://');
        document.querySelector('.status').classList.add('bg-success');
        document.querySelector('.status').innerHTML =
            ' ' + '<br><input class="image-url" value=\"' + get_link + '\"/>' + '<img class="img" alt="Imgur-Upload" src=\"' + get_link + '\"/>';
    }
};

new Imgur({
    clientid: 'b4a1c4bd0ea5845', //You can change this ClientID
    callback: feedback
});
```
#### Đăng kí app vào sửa ClientID tại file [upload.js](https://github.com/hypnguyen1209/imgur-upload/blob/master/js/upload.js)
#### Đăng kí app: https://api.imgur.com/oauth2/addclient
#### Hướng dẫn Docs: https://apidocs.imgur.com/?version=latest#authorization-and-oauth
