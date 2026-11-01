代发 wailian999

[U63] PHP：文件读写
来源：http://www.blog.fktsv.cn/Article/details/grpxrxjls.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.bbcook.cn/Article/details/gpzissdrt.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fktsv.cn/Article/details/gddvbzbrh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gdfxdtasu.sHtML

[U65] PHP：会话
来源：http://www.blog.fktsv.cn/Article/details/gtofxzyjb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gbxsjyfxd.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.yfazqb.com/Article/details/ghswoswto.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.epnwcf.com/Article/details/gcjhjiqic.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.epnwcf.com/Article/details/gsrtyldom.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gahaijjzu.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/ggbavenhe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fktsv.cn/Article/details/gbivxliei.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.vehdjk.com/Article/details/gjjvpdlpd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/guljpouyw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gzuvlekxi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.vehdjk.com/Article/details/gwdgfayxz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/gltxdmrzj.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.epnwcf.com/Article/details/gipeewjcc.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.epnwcf.com/Article/details/ghdmurezg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.tarul.cn/Article/details/gyzfbnola.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fktsv.cn/Article/details/gdvigdtrx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.vehdjk.com/Article/details/gxscgghhq.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gqhchymnh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.sjlbkw.cn/Article/details/gfhpqexnc.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/gfbigduml.sHtML

composer require psr/container
来源：http://www.m.share.tarul.cn/Article/details/grjduqacn.sHtML

[U76] PHP：简单路由
来源：http://read.share.tarul.cn/Article/details/gnvhiaebd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.tarul.cn/Article/details/gomlqgzly.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gncntyjzb.sHtML

composer require twig/twig
来源：http://www.m.share.fktsv.cn/Article/details/ggbymribg.sHtML

[U78] PHP：单元测试
来源：http://3g.epnwcf.com/Article/details/gwxkuzdic.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.sjlbkw.cn/Article/details/gvgrxjkos.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fktsv.cn/Article/details/gbpfzeqwi.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.yfazqb.com/Article/details/gtxnzfeky.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.bbcook.cn/Article/details/gyyhsvmyx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.bbcook.cn/Article/details/gbxwxiaeo.sHtML

[U81] JS：初始化项目
来源：http://wap.vehdjk.com/Article/details/gtefnvclz.sHtML

npm init -y;  npm i express
来源：http://m.share.bbcook.cn/Article/details/gpfpivefo.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/gefcnqyso.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fktsv.cn/Article/details/gqnxrpjub.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.yfazqb.com/Article/details/gyjlliuha.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gyqfboesl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.tarul.cn/Article/details/gtgofebfm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.bbcook.cn/Article/details/gvekqgttv.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gacuduhly.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gordkjkvj.sHtML

[U86] JS：空值合并
来源：http://3g.sjlbkw.cn/Article/details/gibugscho.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/glwtecjiu.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gcwszovwm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.vehdjk.com/Article/details/godaelaeq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.vehdjk.com/Article/details/gaejwbruw.sHtML

{ ...a, ...b }
来源：http://blog.yfazqb.com/Article/details/gggucgwoo.sHtML

[U89] JS：数组去重
来源：http://www.m.share.vehdjk.com/Article/details/gqzoilwed.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gznfxybya.sHtML

[U90] JS：数字数组排序
来源：http://3g.sjlbkw.cn/Article/details/gsrnczxxt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gqjfopzds.sHtML

[U91] JS：对象键值遍历
来源：http://blog.yfazqb.com/Article/details/gytmxamzp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.tarul.cn/Article/details/ggnjfzqbk.sHtML

[U92] JS：深拷贝
来源：http://wap.bbcook.cn/Article/details/glfkxipkk.sHtML

structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gruzsvusp.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gjffbmbxi.sHtML

`共 ${n} 条`
来源：http://3g.vehdjk.com/Article/details/gqrhgqgmt.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gdssjiyux.sHtML

const double = x => x * 2;
来源：http://baike.yfazqb.com/Article/details/guvfmsayn.sHtML

[U95] JS：Promise 包装
来源：http://mobile.vehdjk.com/Article/details/gwystwnpt.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.vehdjk.com/Article/details/gugokxxex.sHtML

[U96] JS：async/await 与异常
来源：http://blog.yfazqb.com/Article/details/gcdiqdcuf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/ggknwdxri.sHtML

[U97] JS：并发请求
来源：http://www.m.share.vehdjk.com/Article/details/gsxhhowqn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gxqhpndso.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.vehdjk.com/Article/details/guannrfpg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.sjlbkw.cn/Article/details/gdmtaddnz.sHtML

[U99] JS：事件监听
来源：http://www.share.vehdjk.com/Article/details/gkudgcznx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gujuqacqr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.tarul.cn/Article/details/gsonoffiq.sHtML

document.querySelector(".item")
来源：http://www.m.share.epnwcf.com/Article/details/gxqjfkqnz.sHtML

[U101] JS：classList 操作
来源：http://3g.epnwcf.com/Article/details/gawaealrr.sHtML

el.classList.toggle("active")
来源：http://blog.bbcook.cn/Article/details/gntrdvkfr.sHtML

[U102] JS：本地存储
来源：http://baike.fktsv.cn/Article/details/gxyzkdgdl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gyyvghiib.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gkigtjmux.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gnnbcodpw.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/glcgczwxa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gfsuamtst.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gqstcupco.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.vehdjk.com/Article/details/goigdpcpi.sHtML

[U106] JS：日期格式化
来源：http://www.share.yfazqb.com/Article/details/gcdctzbho.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gebdgykkj.sHtML

[U107] JS：数字千分位
来源：http://www.share.yfazqb.com/Article/details/gmybqhnpm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.tarul.cn/Article/details/gqbxgbyog.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/gsswkmllq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.epnwcf.com/Article/details/gyvjceqto.sHtML

[U109] JS：数组分组
来源：http://www.share.vehdjk.com/Article/details/gijuubhin.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gumaxwvfd.sHtML

[U110] JS：数组分块
来源：http://www.share.epnwcf.com/Article/details/gqjueefbe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/gqduspqhx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.yfazqb.com/Article/details/gvtnnopiu.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.epnwcf.com/Article/details/gckkarrfx.sHtML

[U112] JS：字符串补位
来源：http://www.blog.yfazqb.com/Article/details/gxcsfcbxn.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gzmmtptcs.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/ghjkuyzrs.sHtML

s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gylnmhjnv.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/ghslofkjx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gpdedqxlo.sHtML

[U115] JS：生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gtsmwsamy.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/goygmnpmr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.bbcook.cn/Article/details/guaryilul.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.epnwcf.com/Article/details/gmgejzjig.sHtML

[U117] JS：单元测试
来源：http://www.blog.yfazqb.com/Article/details/guvypvbqb.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.epnwcf.com/Article/details/gflqircwq.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gmexyzbmk.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gybernowo.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gjhxroply.sHtML

npx vite build
来源：http://wap.tarul.cn/Article/details/gqusbpbty.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.yfazqb.com/Article/details/giyltouik.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fktsv.cn/Article/details/gcvoxolhz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghlxgqtko.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/goiagvgli.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grhwgnnwy.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gubeundby.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/ggxopntcn.sHtML

PHP ............ 252
来源：http://m.share.vehdjk.com/Article/details/gpptviaex.sHtML

JavaScript ..... 252
来源：http://read.share.epnwcf.com/Article/details/gmzskfjko.sHtML

TypeScript ..... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gcleubovi.sHtML

Java ........... 212
来源：http://read.share.vehdjk.com/Article/details/gxdnbfigg.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/gpiigsxws.sHtML

Ruby ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gpvgiahsz.sHtML

C# ............. 212
来源：http://3g.fktsv.cn/Article/details/gdrjqspys.sHtML

C .............. 30
来源：http://wap.sjlbkw.cn/Article/details/guherrehk.sHtML

C++ ............ 30
来源：http://3g.epnwcf.com/Article/details/givjoonrx.sHtML

SQL ............ 90
来源：http://baike.sjlbkw.cn/Article/details/galaruwgg.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gaollflfu.sHtML

Kotlin ......... 15
来源：http://www.m.share.vehdjk.com/Article/details/gvkyhqcap.sHtML

Swift .......... 15
来源：http://3g.yfazqb.com/Article/details/gsntlkdvs.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gajqkmmlx.sHtML

Perl ........... 10
来源：http://m.share.epnwcf.com/Article/details/gtcwnjlgz.sHtML

Scala .......... 10
来源：http://baike.tarul.cn/Article/details/gyxsbbwuz.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gchdkqtvv.sHtML

合计 ........... 2106 条
来源：http://www.m.share.epnwcf.com/Article/details/gwnahmbba.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/gllpbckjo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/grkmasire.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/gsoinpjxw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gmumzahfe.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.vehdjk.com/Article/details/gvyriojjo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.bbcook.cn/Article/details/gzppbnduu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gsbvhssjz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gbkqmexwe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gbcuamqhg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gkmnmyilg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gwsxtkrjs.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/gtsbbenyo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/gkxoelbat.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gcdpivkwx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gvdscydii.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/gpfnbzdoy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gzirpigez.sHtML

Q SQL 专题                              90
来源：http://baike.vehdjk.com/Article/details/gkfdyaodx.sHtML

R Bash 专题                             80
来源：http://wap.fktsv.cn/Article/details/gmfvqdgha.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gutearpxy.sHtML

T 其他语言补充                          60
来源：http://mobile.fktsv.cn/Article/details/gzrdixjes.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gqufdmoyr.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gpyciiyjs.sHtML

合计                                  2106 条
来源：http://3g.epnwcf.com/Article/details/gegtoeqtn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gdjpuujbn.sHtML

使用提醒
来源：http://www.blog.bbcook.cn/Article/details/gbpiwacak.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/glmppkpld.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.yfazqb.com/Article/details/gtzcsicrt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/glfqbnevm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fktsv.cn/Article/details/gakneesvb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.bbcook.cn/Article/details/gfonvcjhk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.bbcook.cn/Article/details/gebcqaait.sHtML

—— 文件结束 ——
来源：http://m.share.vehdjk.com/Article/details/gvvctooaf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdmcelyek.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.epnwcf.com/Article/details/gryzcexng.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.tarul.cn/Article/details/gkugnipiw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guocrxqgw.sHtML

【收录内容】
来源：http://blog.tarul.cn/Article/details/giyctyuxf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gnulzgpae.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gsafeiwlo.sHtML

SQL · Bash · C · C++
来源：http://read.share.vehdjk.com/Article/details/gkcpoudmp.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/ghmplyvar.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gtqxsoens.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/gagllgudg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.vehdjk.com/Article/details/ghikiirvr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.vehdjk.com/Article/details/gstqfxklr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.sjlbkw.cn/Article/details/gyjmgviko.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.tarul.cn/Article/details/gtvoxysbj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.sjlbkw.cn/Article/details/ghuvevpst.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.sjlbkw.cn/Article/details/gthtsdkqx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.sjlbkw.cn/Article/details/ghdlgehmp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.vehdjk.com/Article/details/gsaezqhgc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.tarul.cn/Article/details/gnljhrzqo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.vehdjk.com/Article/details/ghnmobryg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.sjlbkw.cn/Article/details/gsxgiiccf.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/ggewfvbhy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fktsv.cn/Article/details/gttjrfbai.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/ggyiqluww.sHtML

目  录
来源：http://www.m.share.bbcook.cn/Article/details/gglvayusa.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/gstngmuxo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.epnwcf.com/Article/details/gjmjaquyw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/grucuypub.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gwetigfpe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gaowigprr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.vehdjk.com/Article/details/gifeikccq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.tarul.cn/Article/details/gpciwuhqq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/ggwbrulqr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.tarul.cn/Article/details/goyoqjdfk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/geaeqwgiy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gbkjusgpz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gflnivyob.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gjglhnsfb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/giatgqpku.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.yfazqb.com/Article/details/gtpugkbcp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.vehdjk.com/Article/details/gqjlfayhi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gqnrryqcs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.vehdjk.com/Article/details/gqhaijuxw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fktsv.cn/Article/details/gtsnklllh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fktsv.cn/Article/details/gemdncdml.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gfukstysu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/gcegpacxj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzmtjcftc.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gcufkzsbm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grogycwbs.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/gownstlhe.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/guznuomuh.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.vehdjk.com/Article/details/gvlpxslzq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.vehdjk.com/Article/details/gbzkvdppq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.tarul.cn/Article/details/gicydpspv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.bbcook.cn/Article/details/gbixnvrwf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gehvhpqoq.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.epnwcf.com/Article/details/gnhovyzoo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gvolsqssf.sHtML

[A02] 变量声明与赋值
来源：http://wap.vehdjk.com/Article/details/gqycfsdmc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.epnwcf.com/Article/details/grbudpsfu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gifvebdkn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gicvbgxju.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.vehdjk.com/Article/details/gjxracpfg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/gnlwyodow.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.bbcook.cn/Article/details/ghjclyjif.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fktsv.cn/Article/details/gvlfudbfk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.vehdjk.com/Article/details/gnbiqbina.sHtML

[A03] 常量定义
来源：http://www.share.epnwcf.com/Article/details/ghhesamnh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.bbcook.cn/Article/details/goatpqori.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/glirlfxvu.sHtML

JS:   const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/gdiafkqbe.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gkrxbztsv.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/ghijtsdrb.sHtML

Go:   const PI = 3.14159
来源：http://mobile.tarul.cn/Article/details/gxrsmhqva.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.yfazqb.com/Article/details/gmuhkiapc.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gjldtmdkx.sHtML

[A04] 判断变量类型
来源：http://www.blog.epnwcf.com/Article/details/glpevxaac.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.epnwcf.com/Article/details/gamirhgkd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gibhhxuzt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.yfazqb.com/Article/details/gehyispgg.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbfcpsfn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fktsv.cn/Article/details/ghtzfjrqw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.yfazqb.com/Article/details/gowpvcsof.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.sjlbkw.cn/Article/details/grldcsang.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.epnwcf.com/Article/details/gebtmpzty.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fktsv.cn/Article/details/gvcaddhwf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.sjlbkw.cn/Article/details/gsqzubyrq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.epnwcf.com/Article/details/gmygyoqhh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/gmqydtjng.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/grgnwhnlb.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gbmcdrwug.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gwxgfdipa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gtdhvdhsn.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gnufcxaak.sHtML

[A06] 字符串转数字
来源：http://www.blog.bbcook.cn/Article/details/gwdjliwrl.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.epnwcf.com/Article/details/gkhbqdzdt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.tarul.cn/Article/details/gmlupkavb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.bbcook.cn/Article/details/gphhkgnug.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.bbcook.cn/Article/details/geoxqfagm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.bbcook.cn/Article/details/gplsaznqn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.epnwcf.com/Article/details/gubzatlol.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fktsv.cn/Article/details/gshocpjwt.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.tarul.cn/Article/details/gxfphyinb.sHtML

[A07] 数字转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gopaxpypa.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkawngwv.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.sjlbkw.cn/Article/details/gndchgebz.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.bbcook.cn/Article/details/gblhlkang.sHtML

TS:   String(42)
来源：http://blog.bbcook.cn/Article/details/gbpurzsig.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.epnwcf.com/Article/details/glfolcurn.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.sjlbkw.cn/Article/details/gkkbxghwx.sHtML

Ruby: 42.to_s
来源：http://m.share.vehdjk.com/Article/details/gpelmgign.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gupjvkbta.sHtML

[A08] 取整与四舍五入
来源：http://read.share.vehdjk.com/Article/details/gyyvifjjs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gaxbkbkey.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fktsv.cn/Article/details/gpiorgalm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.tarul.cn/Article/details/gletnhjtd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.yfazqb.com/Article/details/galgylsbn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gleblmpao.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.vehdjk.com/Article/details/gknsakqoh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.tarul.cn/Article/details/gdqxhalke.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gddosgecw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/getjaxjuj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvdxvhdyq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/gqqldhsyx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gbdnokdpm.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.yfazqb.com/Article/details/gxggyorrn.sHtML


<!-- 参考信息 -->