# gitlab-untag

<pre>
USAGE: ./gitlab-untag.sh [repository] tagname


DESCRIPTION:
由于早期版本gitlab无法支持中文tag，若不小心上传了含有中文的tag，则页面会出现500错误，因此需要通过该脚本才能完全删除该tag.
【注意】：该操作不可恢复，因此若要保留该tag，则请先checkout该tag，并重新打tag

repository: 远程仓库名，未填写则默认origin
tagname: 标签名

EXAMPLES:

./gitlab-untag.sh 测试1
or
./gitlab-untag.sh origin 测试1

</pre>



远端执行:

<pre>
curl -s https://raw.githubusercontent.com/smallmuou/gitlab-untag/master/gitlab-untag.sh|/bin/bash -s 仓库名 标签名
</pre>

PS: 缺省仓库名为origin