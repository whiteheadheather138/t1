代发 wailian999

[U55] PHP：match 表达式
来源：http://jrm.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ugc.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://upc.hesvh.cn

f(a: 1, b: 2)
来源：http://jnu.fengsongda.top

[U57] PHP：字符串插值
来源：http://ksi.zhoulong.xyz

"值: {$a}"
来源：http://xrr.gogol.net.cn

[U58] PHP：数组三件套
来源：http://ahq.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qbe.hysaishi.cn

[U59] PHP：自定义排序
来源：http://gtl.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tqg.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://umh.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ewx.daxiang520.top

[U61] PHP：正则
来源：http://dvg.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nae.jiagoushi.top

[U62] PHP：日期对象
来源：http://uhq.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cez.jqgfzy.top

[U63] PHP：文件读写
来源：http://bzr.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wdy.aizwys.cn

[U64] PHP：目录遍历
来源：http://zvp.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://gmw.feifeiyinyue.top

[U65] PHP：会话
来源：http://sde.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://juc.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://rzp.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eus.xuanzx.com

[U67] PHP：处理文件上传
来源：http://vzg.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qki.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://nig.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://puc.sxryk.cn

[U69] PHP：PDO 预处理
来源：http://cam.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://laa.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://lsh.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dih.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://iov.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://mjb.yuxming.cn

[U72] PHP：写错误日志
来源：http://ghc.wangdashe.top

error_log("失败: " . $e->getMessage());
来源：http://uuh.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://hka.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://kgl.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://sfa.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://lmp.svipenyu.cn

[U75] PHP：依赖注入
来源：http://aho.fanxiaobao.xyz

composer require psr/container
来源：http://zzo.tian-w.cn

[U76] PHP：简单路由
来源：http://puq.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zcf.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://xlq.52xcode.cn

composer require twig/twig
来源：http://jgm.shzxlz.cn

[U78] PHP：单元测试
来源：http://imb.aibaodan.cn

composer require --dev phpunit/phpunit
来源：http://glg.cashguo.top

[U79] PHP：静态分析
来源：http://ozf.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://iyt.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://ggb.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://oub.uphjek.com

[U81] JS：初始化项目
来源：http://fdv.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://vju.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://nku.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ewo.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://xiz.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://sfv.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://eey.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ezv.chenlongwang.top

[U85] JS：可选链
来源：http://qxj.shzxlz.cn

a?.b?.c
来源：http://bgx.andypj.xyz

[U86] JS：空值合并
来源：http://plq.shuidangran.top

a ?? b
来源：http://asz.jinqigfzy.top

[U87] JS：解构默认值
来源：http://pfr.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://bjx.yongpay.top

[U88] JS：对象展开合并
来源：http://krf.yonumen.top

{ ...a, ...b }
来源：http://xyw.hysaishi.cn

[U89] JS：数组去重
来源：http://cjs.chenlongwang.top

[...new Set(arr)]
来源：http://rmx.aizwys.cn

[U90] JS：数字数组排序
来源：http://mtg.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://jsa.yonumen.top

[U91] JS：对象键值遍历
来源：http://dia.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ivs.yfazqb.com

[U92] JS：深拷贝
来源：http://tav.hongshengwenyu.top

structuredClone(obj)
来源：http://cop.nanxinkj.top

[U93] JS：模板字符串
来源：http://vzn.jinghuilouyu.cn

`共 ${n} 条`
来源：http://lef.gotoacloud.top

[U94] JS：箭头函数
来源：http://cvh.chenzaomai.com

const double = x => x * 2;
来源：http://hod.cqqwz.cn

[U95] JS：Promise 包装
来源：http://drx.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://fle.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://xxb.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mek.svipenyu.cn

[U97] JS：并发请求
来源：http://bdk.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dvq.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://lbd.tianlin.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dfc.yuxming.cn

[U99] JS：事件监听
来源：http://bxo.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://rpp.sufxvd.cn

[U100] JS：DOM 查询
来源：http://zzy.jinyuanbaomall.cn

document.querySelector(".item")
来源：http://qxd.yj20258.top

[U101] JS：classList 操作
来源：http://tav.316326.xyz

el.classList.toggle("active")
来源：http://ndu.yongpay.top

[U102] JS：本地存储
来源：http://ulm.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ici.tarul.cn

[U103] JS：定时器
来源：http://ude.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lgw.bjfxy.top

[U104] JS：防抖
来源：http://arf.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qoc.zdqjudy.top

[U105] JS：节流
来源：http://lxm.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mek.jqgufenzy.top

[U106] JS：日期格式化
来源：http://loc.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xyo.tianlin.xyz

[U107] JS：数字千分位
来源：http://yku.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tqq.jiagoushi.top

[U108] JS：随机整数
来源：http://rfq.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rzb.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://ntc.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://ebw.shuidangran.top

[U110] JS：数组分块
来源：http://tqi.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://guo.zdqjudy.top

[U111] JS：对象转 Map
来源：http://jbv.cqqwz.cn

new Map(Object.entries(obj))
来源：http://qwn.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://ksp.gogol.net.cn

"7".padStart(3, "0")
来源：http://aja.bbcook.cn

[U113] JS：正则替换全部
来源：http://lfs.wangdashe.top

s.replaceAll("a", "b")
来源：http://ewj.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://uvj.c1oappe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hkn.yfazqb.com

[U115] JS：生成 UUID
来源：http://hrr.gotoacloud.top

crypto.randomUUID()
来源：http://mjx.nanxinkj.top

[U116] JS：类型检查（JSDoc）
来源：http://hib.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://xli.jqgfzy.top

[U117] JS：单元测试
来源：http://blr.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://vsm.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://tii.daxiang520.top

npm i -D vite;  npx vite
来源：http://avl.zhiwuduotai.top

[U119] JS：生产构建
来源：http://cvu.vqdsnc.cn

npx vite build
来源：http://ppn.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://bxd.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://hvg.pycfn.com

================================================================================
来源：http://gdg.cqqwz.cn

统计汇总
来源：http://vnw.nanxuanxn.top

================================================================================
来源：http://mlm.shanyushiyangkeji.top

按语言统计（条）：
来源：http://oll.zhaomingkeji.xyz

Python ......... 252
来源：http://hqn.c1oappe.top

PHP ............ 252
来源：http://ywi.fehbvm.com

JavaScript ..... 252
来源：http://gtz.vehdjk.com

TypeScript ..... 212
来源：http://dbm.fengsongda.top

Java ........... 212
来源：http://vlq.ivvv.top

Go ............. 212
来源：http://iji.zhiwuduotai.top

Ruby ........... 212
来源：http://wbm.cashguo.top

C# ............. 212
来源：http://qpi.cdnleiting.top

C .............. 30
来源：http://qui.chenzaomai.com

C++ ............ 30
来源：http://pmp.fzhhl.top

SQL ............ 90
来源：http://zvy.zdbjq.cn

Bash ........... 80
来源：http://rsa.cdnleiting.top

Kotlin ......... 15
来源：http://zib.chenlongwang.top

Swift .......... 15
来源：http://ymr.ehwqpu.com

Lua ............ 10
来源：http://fci.zhongyouzk.top

Perl ........... 10
来源：http://kny.jyoumei.cn

Scala .......... 10
来源：http://bzw.jqgufenzy.top

------------------------------------
来源：http://dkn.hfpthk.cn

合计 ........... 2106 条
来源：http://qcf.daxiang520.top

按章节统计：
来源：http://hmj.tanke756.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hxj.yfazqb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jag.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lwn.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pxk.zhiwuduotai.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sqx.0kj1m.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bfj.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oaf.jinyuanbaomall.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qop.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nff.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ggg.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kwu.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://idm.hnxiangtu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bdn.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lko.sxryk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sci.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ade.quarkkingdee.top

Q SQL 专题                              90
来源：http://oda.ydjk.org.cn

R Bash 专题                             80
来源：http://wti.nanxuanxn.top

S C / C++ 专题                          60
来源：http://ebh.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://pvy.nwbrower.top

U 高频实用片段                         120
来源：http://wec.gogol.net.cn

------------------------------------
来源：http://tqp.xuanzx.com

合计                                  2106 条
来源：http://kwx.gzhubu.top

--------------------------------------------------------------------------------
来源：http://onu.feifeiyinyue.top

使用提醒
来源：http://hna.316326.xyz

--------------------------------------------------------------------------------
来源：http://vsu.sxryk.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://klz.zdqjudy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hpv.fanxiaobao.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ugi.xziqi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hwx.shuidangran.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://aum.hywenlv.cn

—— 文件结束 ——
来源：http://qat.chenzaomai.com

================================================================================
来源：http://eyl.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://uys.zycfv.cn

Common Programming Examples Cheat Book
来源：http://yvl.shanyushiyangkeji.top

================================================================================
来源：http://exa.jinqigfzy.top

【收录内容】
来源：http://qod.bjfxy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ofr.zhiwuduotai.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qdy.chenlongwang.top

SQL · Bash · C · C++
来源：http://vou.smart0.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gcn.chenzaomai.com

【使用说明】
来源：http://csa.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gjs.yuanzhike.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vrn.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tir.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://czp.jqgufenzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ado.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cxu.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kgn.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jxr.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://esd.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vbn.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yed.dianchejie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://caw.kuanghao11.cn

【文件统计】
来源：http://uqy.zhengqikj.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xme.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://ymp.jianghu66.top

目  录
来源：http://mzx.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://vpd.zycfv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zhe.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eyz.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ocq.birdmap.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cag.jinqigufen.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vbe.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://urc.havefunace.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nxm.uphjek.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hhk.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://niy.shangyingyoupin.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jlu.cashguo.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ogi.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xay.svipenyu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jhf.nwbrower.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zns.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cot.ybcxt.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fnl.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qtf.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xpc.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rws.guannengcc.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ekx.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gkc.yuanzhike.top

================================================================================
来源：http://hus.svipenyu.cn

A. 基础语法与类型
来源：http://qmu.shuidangran.top

================================================================================
来源：http://qan.aibaodan.cn

[A01] Hello World
来源：http://egu.sysykeji.top

Py:   print("Hello, World!")
来源：http://jql.chenzaomai.com

PHP:  echo "Hello, World!";
来源：http://ref.c1oappe.top

JS:   console.log("Hello, World!");
来源：http://lxs.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tqo.fktsv.cn

Java: System.out.println("Hello, World!");
来源：http://mev.jqgfzy.top

Go:   fmt.Println("Hello, World!")
来源：http://fls.fzhhl.top

Ruby: puts "Hello, World!"
来源：http://mvg.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kch.gzhubu.top

[A02] 变量声明与赋值
来源：http://mgg.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pgh.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xxn.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hqk.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wjn.xziqi.cn

Java: String name = "Alex"; int age = 20;
来源：http://wfd.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://rde.yangfankeji.com

Ruby: name = "Alex"; age = 20
来源：http://ljv.chenjidiqi.icu

C#:   string name = "Alex"; int age = 20;
来源：http://hzl.zycfv.cn

[A03] 常量定义
来源：http://lsl.pengpengdd.cyou

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aan.jyoumei.cn

PHP:  const PI = 3.14159;
来源：http://kzh.havefunace.top

JS:   const PI = 3.14159;
来源：http://ioq.cdnleiting.top

TS:   const PI: number = 3.14159;
来源：http://tst.meibo888.top

Java: static final double PI = 3.14159;
来源：http://vvd.snrcjt.cn

Go:   const PI = 3.14159
来源：http://hse.sysykeji.top

Ruby: PI = 3.14159
来源：http://tdb.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://the.xinyue.icu

[A04] 判断变量类型
来源：http://nku.zdbjq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lwc.jinyuanbaomall.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tbq.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ckn.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://gxl.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xdz.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jbh.fanxiaobao.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://fow.jianghu66.top

C#:   x.GetType().Name; x is int
来源：http://cng.fehbvm.com

[A05] 整数除法与取模
来源：http://izx.yfazqb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zpy.chenzaomai.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://wkz.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bwp.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yso.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://knq.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://enp.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://ncl.ehwqpu.com

C#:   7 / 2; 7 % 2
来源：http://gbx.gzhubu.top

[A06] 字符串转数字
来源：http://zux.tanke756.top

Py:   int("42"); float("3.14")
来源：http://tba.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fpb.fzhhl.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://asv.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lwv.gzhubu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uzc.pycfn.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hqd.c1oappe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jtb.gotoacloud.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mgu.daxiang520.top

[A07] 数字转字符串
来源：http://pmy.sysykeji.top

Py:   str(42)
来源：http://buz.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://kgo.havefunace.top

JS:   String(42); (42).toString()
来源：http://lct.yj202588.top

TS:   String(42)
来源：http://ncp.snrcjt.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tks.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://fbj.guannengcc.top


<!-- 参考信息 -->