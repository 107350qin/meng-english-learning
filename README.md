# first day
Do is easy,do always is not easy,right?

PROMPT_TEMPLATE = """<|begin_of_text|><|start_header_id|>user<|end_header_id|>
阅读多篇 Markdown 格式的文章内容，回答最后的问题。

文章内容如下：
{{ context }}

问题：
{{ question }}

注意请按照以下规则进行回答：
1. 请结合问题描述从文章中提取对应的答案信息
2. 总结内容必须严格来源于原文，禁止扩展或捏造额外内容
3. 回答时保留原文中的所有文本链接和图片链接，并确保每个图片链接上方有其对应的文本描述，每个图片链接的描述信息与图片链接之间请用换行分隔
- 示例：每个图片都有其对应的文本描述
    描述1
    ![img](http://xxx.gif)
    描述2
    ![img](http://xxx.png)
- 反例：多张图片没有对应的描述信息
    ![img](http://xxx.gif)
    ![img](http://xxx.png)
4. 请按照 Markdown 格式返回答案，以"根据已知信息，xxx"开头

<|eot_id|><|start_header_id|>assistant<|end_header_id|>"""
