代发 wailian999

[U53] PHP：空合并运算符
来源：http://uqm.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://kfl.hesvh.cn

[U54] PHP：空安全调用
来源：http://mcn.hcnkem.com

$obj?->method()
来源：http://zjx.fktsv.cn

[U55] PHP：match 表达式
来源：http://hdb.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nag.jyoumei.cn

[U56] PHP：命名参数
来源：http://gss.jianghu66.top

f(a: 1, b: 2)
来源：http://jje.wangdashe.top

[U57] PHP：字符串插值
来源：http://alq.pycfn.com

"值: {$a}"
来源：http://ziq.tanke756.top

[U58] PHP：数组三件套
来源：http://gzh.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://twy.yj20258888.top

[U59] PHP：自定义排序
来源：http://qpa.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hns.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://ini.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qqs.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://jaf.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pdq.ppjwa.cn

[U62] PHP：日期对象
来源：http://xhc.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ytz.yanxiufei.cn

[U63] PHP：文件读写
来源：http://pvv.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cpi.ehwqpu.com

[U64] PHP：目录遍历
来源：http://zgg.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://spn.316326.xyz

[U65] PHP：会话
来源：http://qze.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://leo.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://wvb.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ful.xuanzx.com

[U67] PHP：处理文件上传
来源：http://kmo.kuanghao11.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bzs.havefunace.top

[U68] PHP：PDO 连接
来源：http://pab.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uxh.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://mek.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rzo.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://hmw.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nhf.gotoacloud.top

[U71] PHP：抛出异常
来源：http://rko.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://hai.shzxlz.cn

[U72] PHP：写错误日志
来源：http://mhi.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://yxj.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://otn.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://jxl.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://yeg.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://jaw.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://jqd.shanyushiyangkeji.top

composer require psr/container
来源：http://whs.andypj.xyz

[U76] PHP：简单路由
来源：http://bzm.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zux.iojbl.cn

[U77] PHP：模板渲染
来源：http://gyl.nanxinkj.top

composer require twig/twig
来源：http://kax.hcnkem.com

[U78] PHP：单元测试
来源：http://pyl.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://esv.xinyue.icu

[U79] PHP：静态分析
来源：http://ngr.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://dyg.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://cxx.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://krx.gzhubu.top

[U81] JS：初始化项目
来源：http://bpr.yfazqb.com

npm init -y;  npm i express
来源：http://gww.redwolf501.top

[U82] JS：package.json 脚本
来源：http://lcs.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://evz.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://crr.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://xww.yuxming.cn

[U84] JS：CommonJS 写法
来源：http://zlw.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://und.hesvh.cn

[U85] JS：可选链
来源：http://gkk.zhoulong.xyz

a?.b?.c
来源：http://oum.gogol.net.cn

[U86] JS：空值合并
来源：http://yhr.xuanzx.com

a ?? b
来源：http://urc.uphjek.com

[U87] JS：解构默认值
来源：http://xxc.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://qgk.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://cuw.xuetiantiany.cn

{ ...a, ...b }
来源：http://czp.jqgufenzy.top

[U89] JS：数组去重
来源：http://nmb.yuanzhike.top

[...new Set(arr)]
来源：http://eeg.haohaochexian.top

[U90] JS：数字数组排序
来源：http://izq.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://vtc.hesvh.cn

[U91] JS：对象键值遍历
来源：http://xgw.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gps.nwbrower.top

[U92] JS：深拷贝
来源：http://okp.hnxiangtu.top

structuredClone(obj)
来源：http://iij.yuxming.cn

[U93] JS：模板字符串
来源：http://zuv.sweek.top

`共 ${n} 条`
来源：http://cll.sufxvd.cn

[U94] JS：箭头函数
来源：http://tef.vqdsnc.cn

const double = x => x * 2;
来源：http://tzh.tian-w.cn

[U95] JS：Promise 包装
来源：http://mrq.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://hgv.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://jxb.jinyuanbaomall.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://amq.hcnkem.com

[U97] JS：并发请求
来源：http://gtr.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://aju.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://hgf.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ksy.feifeiyinyue.top

[U99] JS：事件监听
来源：http://mej.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://yqf.yangfankeji.com

[U100] JS：DOM 查询
来源：http://fsj.smart0.xyz

document.querySelector(".item")
来源：http://oqz.cqqwz.cn

[U101] JS：classList 操作
来源：http://gwx.nanxinkj.top

el.classList.toggle("active")
来源：http://fcz.smart0.xyz

[U102] JS：本地存储
来源：http://bkb.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://azm.cqqwz.cn

[U103] JS：定时器
来源：http://wua.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nfm.gzhubu.top

[U104] JS：防抖
来源：http://xhw.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkb.shuidangran.top

[U105] JS：节流
来源：http://owx.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wrr.xinyue.icu

[U106] JS：日期格式化
来源：http://hvk.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wwd.mhx1999.top

[U107] JS：数字千分位
来源：http://oiy.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rcv.52xcode.cn

[U108] JS：随机整数
来源：http://pfa.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gxv.hongshengwenyu.top

[U109] JS：数组分组
来源：http://bkv.chenjidiqi.icu

Object.groupBy(arr, x => x.type)
来源：http://omv.chenjidiqi.icu

[U110] JS：数组分块
来源：http://zwt.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kqn.shuidangran.top

[U111] JS：对象转 Map
来源：http://hgm.zhixingplan.top

new Map(Object.entries(obj))
来源：http://ybv.iojbl.cn

[U112] JS：字符串补位
来源：http://smt.xylfe.cn

"7".padStart(3, "0")
来源：http://yya.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://rkc.chenlongwang.top

s.replaceAll("a", "b")
来源：http://cjk.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://shr.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lqd.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://pjw.hammf.cn

crypto.randomUUID()
来源：http://yra.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://ujj.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://dot.jqgfzy.top

[U117] JS：单元测试
来源：http://wft.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://law.ppjwa.cn

[U118] JS：开发服务器
来源：http://opg.gotoacloud.top

npm i -D vite;  npx vite
来源：http://nsi.hongshengwenyu.top

[U119] JS：生产构建
来源：http://uwo.zhijiandao.cn

npx vite build
来源：http://qkw.iojbl.cn

[U120] JS：读取环境变量（Vite）
来源：http://njr.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://mdp.ywan-chungtsiang.top

================================================================================
来源：http://aez.yongpay.top

统计汇总
来源：http://wsg.quarkkingdee.top

================================================================================
来源：http://rnp.xuetiantiany.cn

按语言统计（条）：
来源：http://kon.hfpthk.cn

Python ......... 252
来源：http://fgn.hywenlv.cn

PHP ............ 252
来源：http://owm.meibo888.top

JavaScript ..... 252
来源：http://wvb.ctjpmb.com

TypeScript ..... 212
来源：http://bwa.cheryme.top

Java ........... 212
来源：http://gns.kuanghao11.cn

Go ............. 212
来源：http://jeo.yj20258888.top

Ruby ........... 212
来源：http://jok.zhiwuduotai.top

C# ............. 212
来源：http://nzh.mhx1999.top

C .............. 30
来源：http://xdc.nwbrower.top

C++ ............ 30
来源：http://lwj.c1oappe.top

SQL ............ 90
来源：http://url.gzhubu.top

Bash ........... 80
来源：http://ojj.nanxuanxn.top

Kotlin ......... 15
来源：http://mpb.birdmap.top

Swift .......... 15
来源：http://bft.daria6918.cn

Lua ............ 10
来源：http://blg.fanxiaobao.xyz

Perl ........... 10
来源：http://ocs.zhiwuduotai.top

Scala .......... 10
来源：http://jmp.jqgufenzy.top

------------------------------------
来源：http://dey.hongshengwenyu.top

合计 ........... 2106 条
来源：http://msb.jiagoushi.top

按章节统计：
来源：http://vzc.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kri.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zzh.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kcu.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mkd.9152youxi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ecb.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gyc.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hul.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dcr.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pml.chenjidiqi.icu

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://koy.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kjn.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oss.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wvv.birdmap.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pfc.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vug.daria6918.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mnw.zhongyouzk.top

Q SQL 专题                              90
来源：http://dur.zdqjudy.top

R Bash 专题                             80
来源：http://hii.sysykeji.top

S C / C++ 专题                          60
来源：http://bip.epnwcf.com

T 其他语言补充                          60
来源：http://ewg.hfpthk.cn

U 高频实用片段                         120
来源：http://doh.hcnkem.com

------------------------------------
来源：http://xzo.316326.xyz

合计                                  2106 条
来源：http://iuz.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://phd.andypj.xyz

使用提醒
来源：http://zii.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://nkz.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvf.sjlbkw.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gfu.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://idw.tanke756.top

在旧版本上使用前请先确认语法支持情况。
来源：http://laf.ybcxt.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vlu.hnxiangtu.top

—— 文件结束 ——
来源：http://pei.0kj1m.cn

================================================================================
来源：http://och.ehwqpu.com

程序语言常见例子速查手册（2024 版）
来源：http://bvo.yuanzhike.top

Common Programming Examples Cheat Book
来源：http://iem.daria6918.cn

================================================================================
来源：http://jgf.sweek.top

【收录内容】
来源：http://nmf.ydjk.org.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gsk.yj202588.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ytj.aibaodan.cn

SQL · Bash · C · C++
来源：http://ckw.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jdy.xylfe.cn

【使用说明】
来源：http://tja.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sgs.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uio.birdmap.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ovz.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://des.ydzc1.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tjq.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tsd.zhongyouzk.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://saf.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lxw.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zvn.feifeiyinyue.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kih.ivvv.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gjh.snrcjt.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gxc.fzhhl.top

【文件统计】
来源：http://hst.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://glr.yongpay.top

--------------------------------------------------------------------------------
来源：http://yqv.jqgfzy.top

目  录
来源：http://jhp.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://rmu.gogol.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sok.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ewg.jinqigufen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jma.ydzc1.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zbj.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zin.cheryme.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gos.0kj1m.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tjk.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lyu.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xiu.birdmap.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wel.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jen.redwolf501.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fic.birdmap.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lvs.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xkv.nanxuanxn.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ezr.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bix.vqdsnc.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://plf.zhijiandao.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oeg.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vdq.redwolf501.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xjf.jlsjyb.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://toj.c1oappe.top

================================================================================
来源：http://cdb.shangyingyoupin.top

A. 基础语法与类型
来源：http://qob.yonumen.top

================================================================================
来源：http://xzx.uphjek.com

[A01] Hello World
来源：http://vgu.ctjpmb.com

Py:   print("Hello, World!")
来源：http://uau.yangfankeji.com

PHP:  echo "Hello, World!";
来源：http://wqj.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://ebw.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vis.gaohongyu789.top

Java: System.out.println("Hello, World!");
来源：http://yhz.yuanzhike.top

Go:   fmt.Println("Hello, World!")
来源：http://cwr.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://zxp.chenlongwang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://naq.xylfe.cn

[A02] 变量声明与赋值
来源：http://vkn.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yuz.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pem.xingfuxueyuan.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://mjt.ehwqpu.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fxn.zdbjq.cn

Java: String name = "Alex"; int age = 20;
来源：http://idi.mhx1999.top

Go:   name := "Alex"; age := 20
来源：http://exb.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://bxk.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cuu.guannengcc.top

[A03] 常量定义
来源：http://mig.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://huj.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://gwu.epnwcf.com

JS:   const PI = 3.14159;
来源：http://hiz.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://fey.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://cts.pengpengdd.cyou

Go:   const PI = 3.14159
来源：http://qep.gzhubu.top

Ruby: PI = 3.14159
来源：http://hxo.uphjek.com

C#:   const double PI = 3.14159;
来源：http://ynw.haohaochexian.top

[A04] 判断变量类型
来源：http://nwg.bbcook.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yon.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bnd.yj202588.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ykx.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://noh.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fiy.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yrl.cdnleiting.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ual.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://get.svipenyu.cn

[A05] 整数除法与取模
来源：http://pvv.jinqigfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lgl.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zkz.redwolf501.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qke.zhengqikj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wnx.ydzc1.top

Java: 7 / 2; 7 % 2
来源：http://bcb.bjfxy.top

Go:   7 / 2; 7 % 2
来源：http://mhr.jianghu66.top

Ruby: 7 / 2; 7 % 2
来源：http://jmc.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://drt.birdmap.top

[A06] 字符串转数字
来源：http://vml.fehbvm.com

Py:   int("42"); float("3.14")
来源：http://fqd.tianlin.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cwg.jyoumei.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://arh.tian-w.cn

TS:   parseInt("42", 10); Number("42")
来源：http://slk.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zub.guannengcc.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://org.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://sxe.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nxc.nwbrower.top

[A07] 数字转字符串
来源：http://xjn.zycfv.cn

Py:   str(42)
来源：http://spd.quarkkingdee.top

PHP:  (string) 42; strval(42)
来源：http://nic.hongshengwenyu.top


<!-- 参考信息 -->