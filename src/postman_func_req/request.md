# 新建Request

去新建接口，即对应的**Request**：`New -> Request`

![Postman新建Request](../assets/img/postman_new_request.png)

或，在右边的Tab页面中点击加号**+**：

![Postman在Tab页新建Request](../assets/img/postman_tab_new_request.png)

即可看到新建的Tab页：

![Postman新建了的Tab页的Request](../assets/img/postman_newly_created_tab_request.png)

然后：
* 设置HTTP的Method方法和输入api的地址

![Postman设置Method和输入API地址](../assets/img/postman_set_method_and_api.png)

* 设置相关头信息

![Postman设置Header头的key](../assets/img/postman_set_headers_key.png)

![Postman设置Header头的value](../assets/img/postman_set_headers_value.png)

* 设置相关GET或POST等的参数

![Postman设置POST的Body的JSON](../assets/img/postman_set_post_body_json.png)

都填写好之后，点击Send去发送**请求Request**：

![Postman点击发送请求](../assets/img/postman_send_request.png)

即可看到返回的**响应Response**的信息了：

![Postman返回响应](../assets/img/postman_return_response.png)

然后可以重复上述修改Request的参数，点击Send去发送请求的过程，以便调试到API接口正常工作为止。

待整个接口都调试完毕后，记得点击Save去保存接口信息：

![Postman点击Save保存](../assets/img/postman_click_save.png)

去保存当前API接口，然后需要填写相关的接口信息：
* Request Name: 请求的名字
  * 我一般习惯用保存为 接口的最后的字段名，比如`http://{% raw %}{{% endraw %}{server_address}}/ucows/login/login`中的`/login/login`
* Request Description: 接口的描述
  * `可选` 最好写上该接口的要实现的基本功能和相关注意事项
  * 支持Markdown语法
* Select a collection or folder to save: 选择要保存到哪个分组（或文件夹）
  * 往往保存到某个API接口到所属的该项目名的分组

![Postman保存时填写接口信息](../assets/img/postman_fill_api_info_to_save.png)

填写好内容，选择好分组，再点击保存：

![Postman保存到分组](../assets/img/postman_save_to_collection.png)

此时，Tab的右上角的黄色点（表示没有保存）消失了，表示已保存。

且对应的分组中可以看到对应的接口了：

![Postman已保存的API接口Tab页](../assets/img/postman_saved_api_tab.png)

> #### warning::默认不保存返回的Response数据
> * 直接点击Save去保存，只能保存API本身（的Request请求），不会保存Response的数据
> * 想要保存Response数据，需要用后面要介绍的 [多个Example](http://book.crifan.com/books/api_tool_postman/website/postman_func_resp/save_multi_example.html)
