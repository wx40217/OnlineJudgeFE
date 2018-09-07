<template>
  <panel>
    <div slot="title">{{$t('m.Frequently_Asked_Questions')}}</div>
    <div class="content markdown-body">
      <ul>
        <li>输入输出在哪里？
          <p>你的程序应该从 <code>stdin</code>('标准输入') 获得输入， 把输出写到 <code>stdout</code>('标准输出')中。
            比方说,C语言可以使用 <code>scanf</code>从stdin读取输入,用 <code>printf</code> 写入到cstdin中。 C++可以使用 <code>cin</code>和 <code>cout</code> 。
            你的程序不允许读取或写入文件, 不然你会遇到 <code>Runtime Error</code>。
          </p>
        </li>
        <li>提交执行时间的含义是什么？
        <p>
          oj可能会使用不同的输入文件多次测试代码。 如果代码在每个输入文件的时间限制内给出正确的答案，则显示的执行时间是每个测试用例花费的最大时间。 否则，执行时间就没有意义了。
        </p>
        </li>
        <li>我怎么在C++中使用INT64？
          <p>用 <code>long long</code> 声明，用<code>cin/cout</code> 或者 <code>%lld</code>输入输出， 用<code> __int64</code> 会导致<code>Compile Error</code>。</p>
        </li>
        <li>Java的规范？
          <p>所有的程序都必须以<code>Main</code> 类中的静态main方法打头。 不要使用public类： <code>Main</code>也必须是非public，为了避免编译错误。使用缓冲I / O以避免由于过度刷新而超出时间限制。</p>
        </li>
        <li>讲讲<code>presentation error </code>（格式错误）？
          <p>不存在的。oj 会自动去掉<b>最后一行</b>的空格和换行符 。
           如果这样还不对，返回的就会是<code>Wrong Answer</code>。</p>
        </li>
        <li>如何报告oj的bug？
          <p><s>The onlinejudge is open source, you can open an issue in <a href="https://github.com/QingdaoU/OnlineJudge">Github</a>.
            The details(like env, version..) about a bug is required, which will help us a lot to solve the bug.
            Certainly, we are very pleased to merge your pull requests.</s><br/>
            有问题直接报告QQ185605170.
          </p>
        </li>
      </ul>
    </div>
  </panel>
</template>

<script>
</script>

<style lang="less" scoped>
  .content {
    font-size: 16px;
    margin: 0 50px 40px 50px;
    > ul {
      list-style: disc;
      li {
        font-size: 16px;
        margin-top: 20px;
        &:first-child {
          margin-top: 0;
        }
        p {
          font-size: 14px;
          margin-top: 5px;
        }
      }
    }
  }
</style>
