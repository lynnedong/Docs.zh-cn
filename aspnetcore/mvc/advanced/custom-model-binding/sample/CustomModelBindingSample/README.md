# <a name="custom-model-binding-demo"></a><span data-ttu-id="6bda3-101">自定义模型绑定演示</span><span class="sxs-lookup"><span data-stu-id="6bda3-101">Custom Model Binding Demo</span></span>

<span data-ttu-id="6bda3-102">你可以测试`ByteArrayModelBinder`通过运行应用程序并发布 ImageController 终结点的 base64 编码字符串 (/ api/图像 /)。</span><span class="sxs-lookup"><span data-stu-id="6bda3-102">You can test the `ByteArrayModelBinder` by running the application and POSTing a base64-encoded string to the ImageController endpoint (/api/image/).</span></span> <span data-ttu-id="6bda3-103">你应在请求正文作为窗体数据中指定文件和文件名 proparties （使用 Postman 或类似的工具）。</span><span class="sxs-lookup"><span data-stu-id="6bda3-103">You should specify the file and filename proparties in the request Body as form-data (using Postman or a similar tool).</span></span> <span data-ttu-id="6bda3-104">你可以使用[此示例字符串](Base64String.txt)。</span><span class="sxs-lookup"><span data-stu-id="6bda3-104">You can use [this sample string](Base64String.txt).</span></span> <span data-ttu-id="6bda3-105">结果将保存在具有所指定的文件名的 wwwroot/图像/上载文件夹中。</span><span class="sxs-lookup"><span data-stu-id="6bda3-105">The result will be saved in the wwwroot/images/upload folder with the filename you specified.</span></span>

<span data-ttu-id="6bda3-106">若要测试自定义绑定示例，请尝试以下终结点： /api/authors/1 /api/authors/2 （未找到） /api/boundauthors/1 /api/boundauthors/2 （未找到） 此操作不会检查 /api/boundauthors/get/1 /api/boundauthors/get/2 （无内容） 的null，并且返回未找到</span><span class="sxs-lookup"><span data-stu-id="6bda3-106">To test the custom binding example, try the following endpoints: /api/authors/1 /api/authors/2 (NOT FOUND) /api/boundauthors/1 /api/boundauthors/2 (NOT FOUND) /api/boundauthors/get/1 /api/boundauthors/get/2 (NO CONTENT) - this action doesn't check for null and return a Not Found</span></span>