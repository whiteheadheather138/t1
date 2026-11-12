代发 wailian999

[U51] PHP：数组解构
来源：http://hpl.0kj1m.cn

[$a, $b] = $arr;
来源：http://gja.smart0.xyz

[U52] PHP：箭头函数
来源：http://fmh.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://ayc.shuidangran.top

[U53] PHP：空合并运算符
来源：http://jed.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://xxd.chenlongwang.top

[U54] PHP：空安全调用
来源：http://pfw.yonumen.top

$obj?->method()
来源：http://znx.yongpay.top

[U55] PHP：match 表达式
来源：http://qrc.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jgx.fzhhl.top

[U56] PHP：命名参数
来源：http://cpj.fengsongda.top

f(a: 1, b: 2)
来源：http://kls.jiagoushi.top

[U57] PHP：字符串插值
来源：http://eiy.gogol.net.cn

"值: {$a}"
来源：http://uex.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://qyi.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lyc.sxryk.cn

[U59] PHP：自定义排序
来源：http://dcv.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cej.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://mpr.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://apg.gogol.net.cn

[U61] PHP：正则
来源：http://jkf.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gxj.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://edi.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tkr.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://hug.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pkh.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://rnj.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://duv.wangdashe.top

[U65] PHP：会话
来源：http://lob.ydjk.org.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mdx.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://uxp.birdmap.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bja.hysaishi.cn

[U67] PHP：处理文件上传
来源：http://dkx.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qsq.vqdsnc.cn

[U68] PHP：PDO 连接
来源：http://vdc.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xeq.ppjwa.cn

[U69] PHP：PDO 预处理
来源：http://bvu.xziqi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://efu.yvedp.cn

[U70] PHP：PDO 事务
来源：http://adu.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jwf.ehwqpu.com

[U71] PHP：抛出异常
来源：http://lpo.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://nxl.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://dut.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://zgv.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://lbd.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://nno.yvedp.cn

[U74] PHP：读取环境变量
来源：http://iqb.0kj1m.cn

getenv("APP_ENV") ?: "production"
来源：http://cuc.hysaishi.cn

[U75] PHP：依赖注入
来源：http://mrd.ybcxt.top

composer require psr/container
来源：http://tnq.yanxiufei.cn

[U76] PHP：简单路由
来源：http://zer.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://plz.mhx1999.top

[U77] PHP：模板渲染
来源：http://hhq.andypj.xyz

composer require twig/twig
来源：http://stf.nanxinkj.top

[U78] PHP：单元测试
来源：http://hpq.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://spl.cqqwz.cn

[U79] PHP：静态分析
来源：http://vmp.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://bie.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://jvn.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://itv.dianchejie.cn

[U81] JS：初始化项目
来源：http://tyq.jyoumei.cn

npm init -y;  npm i express
来源：http://hsr.sysykeji.top

[U82] JS：package.json 脚本
来源：http://hmu.fanxiaobao.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kva.xingfuxueyuan.xyz

[U83] JS：ES Module 导入导出
来源：http://wzy.yonumen.top

export const a = 1;  import { a } from "./m.js";
来源：http://zyc.cheryme.top

[U84] JS：CommonJS 写法
来源：http://mlz.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://dxa.hnxiangtu.top

[U85] JS：可选链
来源：http://amy.uphjek.com

a?.b?.c
来源：http://tdc.mhx1999.top

[U86] JS：空值合并
来源：http://itc.chenjidiqi.icu

a ?? b
来源：http://oxm.yj20258.top

[U87] JS：解构默认值
来源：http://pru.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://ogn.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://gin.pycfn.com

{ ...a, ...b }
来源：http://kos.0kj1m.cn

[U89] JS：数组去重
来源：http://bid.hysaishi.cn

[...new Set(arr)]
来源：http://mnh.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://gyu.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://zxb.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://uum.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mdm.hnxiangtu.top

[U92] JS：深拷贝
来源：http://urb.cucudq.cn

structuredClone(obj)
来源：http://vfl.ivvv.top

[U93] JS：模板字符串
来源：http://cfe.shangyingyoupin.top

`共 ${n} 条`
来源：http://bmg.hammf.cn

[U94] JS：箭头函数
来源：http://hpy.svipenyu.cn

const double = x => x * 2;
来源：http://bpi.ppjwa.cn

[U95] JS：Promise 包装
来源：http://yza.yonumen.top

new Promise((resolve, reject) => {})
来源：http://inw.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://dgi.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oad.ybcxt.top

[U97] JS：并发请求
来源：http://vau.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vlt.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://rdf.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yzu.zdqjudy.top

[U99] JS：事件监听
来源：http://ncp.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://njw.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://vzq.jqgfzy.top

document.querySelector(".item")
来源：http://wes.9152youxi.cn

[U101] JS：classList 操作
来源：http://vig.tarul.cn

el.classList.toggle("active")
来源：http://vls.sweek.top

[U102] JS：本地存储
来源：http://epb.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rbr.shangyingyoupin.top

[U103] JS：定时器
来源：http://bia.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gae.zdbjq.cn

[U104] JS：防抖
来源：http://rjz.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntt.fengsongda.top

[U105] JS：节流
来源：http://imx.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://icn.zhixingplan.top

[U106] JS：日期格式化
来源：http://hva.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rmq.quarkkingdee.top

[U107] JS：数字千分位
来源：http://ffq.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://abk.jiagoushi.top

[U108] JS：随机整数
来源：http://qqt.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gkg.yfazqb.com

[U109] JS：数组分组
来源：http://pmp.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://shy.c1oappe.top

[U110] JS：数组分块
来源：http://kgr.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://glw.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://hql.yongpay.top

new Map(Object.entries(obj))
来源：http://khu.aizwys.cn

[U112] JS：字符串补位
来源：http://ycy.ehwqpu.com

"7".padStart(3, "0")
来源：http://xpr.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://psy.hfpthk.cn

s.replaceAll("a", "b")
来源：http://epd.316326.xyz

[U114] JS：JSON 深比较
来源：http://vmj.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nyb.wangshuangyany.cn

[U115] JS：生成 UUID
来源：http://lqd.hnxiangtu.top

crypto.randomUUID()
来源：http://fza.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://vim.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://hep.hammf.cn

[U117] JS：单元测试
来源：http://sgh.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://itt.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://ndh.jqgfzy.top

npm i -D vite;  npx vite
来源：http://ila.9152youxi.cn

[U119] JS：生产构建
来源：http://nyc.guowangkeji.top

npx vite build
来源：http://svo.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://tgz.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://sdi.xylfe.cn

================================================================================
来源：http://bqd.gotoacloud.top

统计汇总
来源：http://sqs.tianlin.xyz

================================================================================
来源：http://lsn.gaohongyu789.top

按语言统计（条）：
来源：http://xzf.zhiwuduotai.top

Python ......... 252
来源：http://pac.nanxinkj.top

PHP ............ 252
来源：http://zcg.guannengcc.top

JavaScript ..... 252
来源：http://igk.epnwcf.com

TypeScript ..... 212
来源：http://yiu.nanxinkj.top

Java ........... 212
来源：http://vhu.uphjek.com

Go ............. 212
来源：http://igx.nanxinkj.top

Ruby ........... 212
来源：http://lnt.yangfankeji.com

C# ............. 212
来源：http://vyh.bjfxy.top

C .............. 30
来源：http://snb.mhx1999.top

C++ ............ 30
来源：http://bdu.yvedp.cn

SQL ............ 90
来源：http://eaf.9152youxi.cn

Bash ........... 80
来源：http://pym.jinghuilouyu.cn

Kotlin ......... 15
来源：http://ozx.yj202588.top

Swift .......... 15
来源：http://abs.jiagoushi.top

Lua ............ 10
来源：http://iga.snrcjt.cn

Perl ........... 10
来源：http://eah.ppjwa.cn

Scala .......... 10
来源：http://wir.yuanzhike.top

------------------------------------
来源：http://ywg.kuanghao11.cn

合计 ........... 2106 条
来源：http://fva.daxiang520.top

按章节统计：
来源：http://olt.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bdg.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wxy.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xls.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://unr.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xxs.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://apy.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pir.yfazqb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bgm.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zjc.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jgn.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fjo.jlsjyb.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dve.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xxj.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mrj.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hnd.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://szo.shanyushiyangtech.top

Q SQL 专题                              90
来源：http://imn.yueranfly.top

R Bash 专题                             80
来源：http://rfx.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://lzx.xylfe.cn

T 其他语言补充                          60
来源：http://vci.iojbl.cn

U 高频实用片段                         120
来源：http://cfh.aibaodan.cn

------------------------------------
来源：http://sbp.tian-w.cn

合计                                  2106 条
来源：http://xsj.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://qql.dashuyun.cn

使用提醒
来源：http://bnz.xinyue.icu

--------------------------------------------------------------------------------
来源：http://vuz.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nko.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bff.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kqp.zhengqikj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://djm.chenzaomai.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ffm.guowangkeji.top

—— 文件结束 ——
来源：http://svt.snrcjt.cn

================================================================================
来源：http://luf.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://nce.shanyushiyangtech.top

Common Programming Examples Cheat Book
来源：http://dhp.aizwys.cn

================================================================================
来源：http://iic.zhiwuduotai.top

【收录内容】
来源：http://paa.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hse.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nmw.vehdjk.com

SQL · Bash · C · C++
来源：http://rso.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tcj.yuanzhike.top

【使用说明】
来源：http://zad.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rlu.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yqv.daria6918.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bvy.zhongyouzk.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nbx.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://zez.xingfuxueyuan.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pqi.pengpengdd.cyou

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://msa.52xcode.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dql.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://efd.hesvh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ioy.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://meb.tarul.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dxr.redwolf501.top

【文件统计】
来源：http://cbp.aibaodan.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nuv.pycfn.com

--------------------------------------------------------------------------------
来源：http://baj.mhx1999.top

目  录
来源：http://czi.tanke756.top

--------------------------------------------------------------------------------
来源：http://cuj.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rkf.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kts.ivvv.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hhm.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ezv.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hil.fzhhl.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rzb.hywenlv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rmc.aizwys.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ajw.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qki.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tir.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ckq.yonumen.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aes.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tjc.dianchejie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xhj.tanke756.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://crr.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nos.ehwqpu.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vkx.52xcode.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wyg.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uui.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sol.nwbrower.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ncm.bjfxy.top

================================================================================
来源：http://lks.sxryk.cn

A. 基础语法与类型
来源：http://zov.meibo888.top

================================================================================
来源：http://sjn.yueranfly.top

[A01] Hello World
来源：http://dnn.jiagoushi.top

Py:   print("Hello, World!")
来源：http://hhs.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://exe.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://bhl.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fkn.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://oiq.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://cbw.zhongyouzk.top

Ruby: puts "Hello, World!"
来源：http://lkv.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hik.ivvv.top

[A02] 变量声明与赋值
来源：http://cgw.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://igo.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://aba.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://gds.uphjek.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pfc.yvedp.cn

Java: String name = "Alex"; int age = 20;
来源：http://mpb.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://thk.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://tfi.epnwcf.com

C#:   string name = "Alex"; int age = 20;
来源：http://gud.yueranfly.top

[A03] 常量定义
来源：http://rgz.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qhg.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://xhz.sxryk.cn

JS:   const PI = 3.14159;
来源：http://eog.9152youxi.cn

TS:   const PI: number = 3.14159;
来源：http://ypl.tarul.cn

Java: static final double PI = 3.14159;
来源：http://dxi.hnqzz.top

Go:   const PI = 3.14159
来源：http://grp.xziqi.cn

Ruby: PI = 3.14159
来源：http://slt.dianchejie.cn

C#:   const double PI = 3.14159;
来源：http://etu.shanyushiyangtech.top

[A04] 判断变量类型
来源：http://ugr.kuanghao11.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mla.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://egu.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ckc.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://isd.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jav.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kyu.wangshuangyany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pzz.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://bll.fehbvm.com

[A05] 整数除法与取模
来源：http://zxz.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eih.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://qas.zhoulong.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kiw.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qpm.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://qfl.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://yxh.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://whx.hnxiangtu.top

C#:   7 / 2; 7 % 2
来源：http://ixt.haohaochexian.top

[A06] 字符串转数字
来源：http://mxv.yongpay.top

Py:   int("42"); float("3.14")
来源：http://lfu.chenlongwang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rop.chenzaomai.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yzq.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://oii.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://amr.cucudq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://grb.fzhhl.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jnp.xinyue.icu


<!-- 参考信息 -->