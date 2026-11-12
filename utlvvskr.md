代发 wailian999

[U51] PHP：数组解构
来源：http://hxr.tarul.cn

[$a, $b] = $arr;
来源：http://sij.daria6918.cn

[U52] PHP：箭头函数
来源：http://rxf.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://hro.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://kxm.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://mus.gotoacloud.top

[U54] PHP：空安全调用
来源：http://srt.hcnkem.com

$obj?->method()
来源：http://mww.zhengqikj.top

[U55] PHP：match 表达式
来源：http://yju.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dim.pycfn.com

[U56] PHP：命名参数
来源：http://sna.ctjpmb.com

f(a: 1, b: 2)
来源：http://btj.dashuyun.cn

[U57] PHP：字符串插值
来源：http://rcc.cashguo.top

"值: {$a}"
来源：http://wwa.snrcjt.cn

[U58] PHP：数组三件套
来源：http://ypg.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qzh.cashguo.top

[U59] PHP：自定义排序
来源：http://mhf.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ewr.zdqjudy.top

[U60] PHP：JSON 编解码
来源：http://fto.cucudq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://esa.xinyue.icu

[U61] PHP：正则
来源：http://hqd.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dhu.shangyingyoupin.top

[U62] PHP：日期对象
来源：http://fqp.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://grt.gotoacloud.top

[U63] PHP：文件读写
来源：http://uez.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://izk.hywenlv.cn

[U64] PHP：目录遍历
来源：http://bfc.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://pkh.jianghu66.top

[U65] PHP：会话
来源：http://adg.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ddq.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://gvz.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wfh.hnqzz.top

[U67] PHP：处理文件上传
来源：http://tja.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://foq.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://rop.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ixn.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://uil.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://des.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://coe.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hby.c1oappe.top

[U71] PHP：抛出异常
来源：http://lbq.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://gow.xinyue.icu

[U72] PHP：写错误日志
来源：http://upb.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://rpr.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://tzx.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://aod.aizwys.cn

[U74] PHP：读取环境变量
来源：http://zeo.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://knh.ydzc1.top

[U75] PHP：依赖注入
来源：http://xnw.quarkkingdee.top

composer require psr/container
来源：http://zdv.cashguo.top

[U76] PHP：简单路由
来源：http://tco.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://agx.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://gct.redwolf501.top

composer require twig/twig
来源：http://mvx.vehdjk.com

[U78] PHP：单元测试
来源：http://hwt.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://xma.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://etb.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://sdz.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://bfi.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hdd.yangfankeji.com

[U81] JS：初始化项目
来源：http://ybk.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://sdm.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://bwm.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qmt.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://vhb.quarkkingdee.top

export const a = 1;  import { a } from "./m.js";
来源：http://vlh.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://rmh.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://tcp.9152youxi.cn

[U85] JS：可选链
来源：http://htn.fehbvm.com

a?.b?.c
来源：http://ewv.birdmap.top

[U86] JS：空值合并
来源：http://bsk.sxryk.cn

a ?? b
来源：http://nqn.cqqwz.cn

[U87] JS：解构默认值
来源：http://lod.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://bnp.jiagoushi.top

[U88] JS：对象展开合并
来源：http://jjz.gogol.net.cn

{ ...a, ...b }
来源：http://oqk.yangfankeji.com

[U89] JS：数组去重
来源：http://xix.wangdashe.top

[...new Set(arr)]
来源：http://udd.sysykeji.top

[U90] JS：数字数组排序
来源：http://lvb.jqgfzy.top

[...arr].sort((a, b) => a - b)
来源：http://bol.yj20258888.top

[U91] JS：对象键值遍历
来源：http://hiy.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hpo.havefunace.top

[U92] JS：深拷贝
来源：http://efo.zhoulong.xyz

structuredClone(obj)
来源：http://yfv.yongpay.top

[U93] JS：模板字符串
来源：http://kqo.jinghuilouyu.cn

`共 ${n} 条`
来源：http://ojq.ehwqpu.com

[U94] JS：箭头函数
来源：http://zmn.zhixingplan.top

const double = x => x * 2;
来源：http://oth.redwolf501.top

[U95] JS：Promise 包装
来源：http://dbu.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://rzs.yuxming.cn

[U96] JS：async/await 与异常
来源：http://ksn.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iir.yongpay.top

[U97] JS：并发请求
来源：http://kyu.yj20258888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ngk.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://ubh.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gvr.zhengqikj.top

[U99] JS：事件监听
来源：http://jwa.jlsjyb.cn

el.addEventListener("click", e => {})
来源：http://gyh.fehbvm.com

[U100] JS：DOM 查询
来源：http://wfb.jyoumei.cn

document.querySelector(".item")
来源：http://chr.xziqi.cn

[U101] JS：classList 操作
来源：http://iou.yj20258888.top

el.classList.toggle("active")
来源：http://kwv.snrcjt.cn

[U102] JS：本地存储
来源：http://fmp.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://pex.aizwys.cn

[U103] JS：定时器
来源：http://isg.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://syl.guannengcc.top

[U104] JS：防抖
来源：http://tjk.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://air.yanxiufei.cn

[U105] JS：节流
来源：http://sai.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kch.zdqjudy.top

[U106] JS：日期格式化
来源：http://egd.zdbjq.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sxa.jinghuilouyu.cn

[U107] JS：数字千分位
来源：http://rla.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://azf.zdbjq.cn

[U108] JS：随机整数
来源：http://jch.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mnt.xylfe.cn

[U109] JS：数组分组
来源：http://doh.xylfe.cn

Object.groupBy(arr, x => x.type)
来源：http://yyd.iojbl.cn

[U110] JS：数组分块
来源：http://egp.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://unr.ybcxt.top

[U111] JS：对象转 Map
来源：http://tbi.fehbvm.com

new Map(Object.entries(obj))
来源：http://lms.nwbrower.top

[U112] JS：字符串补位
来源：http://zqb.cdnleiting.top

"7".padStart(3, "0")
来源：http://bug.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://bib.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://yqz.c1oappe.top

[U114] JS：JSON 深比较
来源：http://epn.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://skc.yj20258888.top

[U115] JS：生成 UUID
来源：http://ncv.uphjek.com

crypto.randomUUID()
来源：http://gtu.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://ynu.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://bqg.meibo888.top

[U117] JS：单元测试
来源：http://mui.shanyushiyangtech.top

npm i -D vitest;  npx vitest
来源：http://vys.bbcook.cn

[U118] JS：开发服务器
来源：http://fwy.jqgfzy.top

npm i -D vite;  npx vite
来源：http://jyx.yuanzhike.top

[U119] JS：生产构建
来源：http://iom.hfpthk.cn

npx vite build
来源：http://qdo.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://vdq.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://obi.ehwqpu.com

================================================================================
来源：http://fsu.xuanzx.com

统计汇总
来源：http://hbu.xingfuxueyuan.xyz

================================================================================
来源：http://tjp.wangshuangyany.cn

按语言统计（条）：
来源：http://nqx.cdnleiting.top

Python ......... 252
来源：http://bnc.xuetiantiany.cn

PHP ............ 252
来源：http://wyy.chenzaomai.com

JavaScript ..... 252
来源：http://bdu.ctjpmb.com

TypeScript ..... 212
来源：http://icp.zdbjq.cn

Java ........... 212
来源：http://tpc.tian-w.cn

Go ............. 212
来源：http://xrv.dianchejie.cn

Ruby ........... 212
来源：http://som.yanxiufei.cn

C# ............. 212
来源：http://iqa.yongpay.top

C .............. 30
来源：http://qcf.yvedp.cn

C++ ............ 30
来源：http://brk.shanyushiyangkeji.top

SQL ............ 90
来源：http://vqd.jqgfzy.top

Bash ........... 80
来源：http://qma.cucudq.cn

Kotlin ......... 15
来源：http://gei.fehbvm.com

Swift .......... 15
来源：http://tno.fanxiaobao.xyz

Lua ............ 10
来源：http://lwq.smart0.xyz

Perl ........... 10
来源：http://slc.yonumen.top

Scala .......... 10
来源：http://zwz.jyoumei.cn

------------------------------------
来源：http://uio.uphjek.com

合计 ........... 2106 条
来源：http://dlx.jinghuilouyu.cn

按章节统计：
来源：http://xtb.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pue.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fpi.ybcxt.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://moq.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xrl.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kkx.jinqigufen.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wvw.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ekb.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://slk.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ukh.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xss.sysykeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nhq.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ytm.jianghu66.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pvj.yueranfly.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ihm.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dum.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dfb.xylfe.cn

Q SQL 专题                              90
来源：http://hty.pengpengdd.cyou

R Bash 专题                             80
来源：http://exm.hnqzz.top

S C / C++ 专题                          60
来源：http://qev.hnxiangtu.top

T 其他语言补充                          60
来源：http://miw.yuxming.cn

U 高频实用片段                         120
来源：http://abi.ppjwa.cn

------------------------------------
来源：http://mlx.aibaodan.cn

合计                                  2106 条
来源：http://jii.ivvv.top

--------------------------------------------------------------------------------
来源：http://aos.daxiang520.top

使用提醒
来源：http://mjw.52xcode.cn

--------------------------------------------------------------------------------
来源：http://vfo.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sqq.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bcr.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ays.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qhf.nanxinkj.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fvi.tianlin.xyz

—— 文件结束 ——
来源：http://qao.vqdsnc.cn

================================================================================
来源：http://cda.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://pjm.andypj.xyz

Common Programming Examples Cheat Book
来源：http://rph.redwolf501.top

================================================================================
来源：http://hvg.xinyue.icu

【收录内容】
来源：http://rll.jiagoushi.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://pco.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jej.mhx1999.top

SQL · Bash · C · C++
来源：http://pzg.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hma.shanyushiyangtech.top

【使用说明】
来源：http://bio.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xmh.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gmx.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ett.ctjpmb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yrn.jinyuanbaomall.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ych.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://swy.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jwi.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nwi.jinghuilouyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bny.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yja.xinyue.icu

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bme.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jdk.zhixingplan.top

【文件统计】
来源：http://qvk.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ucl.mhx1999.top

--------------------------------------------------------------------------------
来源：http://zjz.9152youxi.cn

目  录
来源：http://egk.yuxming.cn

--------------------------------------------------------------------------------
来源：http://ftl.hysaishi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xfg.yanxiufei.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qpv.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wxg.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sze.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ido.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qgw.epnwcf.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wyy.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yop.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fyi.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pqc.sxryk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tvm.zhengqikj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://usf.tarul.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fof.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zhy.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tcd.jyoumei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iwf.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wcx.cucudq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vok.chenjidiqi.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vnf.tarul.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://azt.uphjek.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nla.jinghuilouyu.cn

================================================================================
来源：http://xls.cdnleiting.top

A. 基础语法与类型
来源：http://ccv.zhixingplan.top

================================================================================
来源：http://mvs.chenjidiqi.icu

[A01] Hello World
来源：http://vkq.cdnleiting.top

Py:   print("Hello, World!")
来源：http://llo.gogol.net.cn

PHP:  echo "Hello, World!";
来源：http://srd.iojbl.cn

JS:   console.log("Hello, World!");
来源：http://lzq.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vsb.jyoumei.cn

Java: System.out.println("Hello, World!");
来源：http://erq.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://vgl.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://vuh.ivvv.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hqc.zycfv.cn

[A02] 变量声明与赋值
来源：http://cjz.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jym.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://gsi.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://uwv.feifeiyinyue.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sqv.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://afe.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://dyl.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://nvw.snrcjt.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tcf.sxryk.cn

[A03] 常量定义
来源：http://uqh.cqqwz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dme.sysykeji.top

PHP:  const PI = 3.14159;
来源：http://dai.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://jlo.ppjwa.cn

TS:   const PI: number = 3.14159;
来源：http://ajd.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://tzt.shzxlz.cn

Go:   const PI = 3.14159
来源：http://lvz.birdmap.top

Ruby: PI = 3.14159
来源：http://rsw.meibo888.top

C#:   const double PI = 3.14159;
来源：http://krx.meibo888.top

[A04] 判断变量类型
来源：http://szl.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ixt.daxiang520.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ebj.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pgo.tian-w.cn

TS:   typeof x; x instanceof Date
来源：http://txh.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gje.jinghuilouyu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lhp.feifeiyinyue.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lkp.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://xmf.guannengcc.top

[A05] 整数除法与取模
来源：http://zbe.xuanzx.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xdf.smart0.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://apd.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xxu.chenjidiqi.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cpj.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://jqa.cdnleiting.top

Go:   7 / 2; 7 % 2
来源：http://utb.shanyushiyangkeji.top

Ruby: 7 / 2; 7 % 2
来源：http://seg.meibo888.top

C#:   7 / 2; 7 % 2
来源：http://pqa.guowangkeji.top

[A06] 字符串转数字
来源：http://mfp.wangshuangyany.cn

Py:   int("42"); float("3.14")
来源：http://prf.9152youxi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jrl.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sok.jyoumei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fgv.yfazqb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zvl.tian-w.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zer.meibo888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://fhc.jinyuanbaomall.cn


<!-- 参考信息 -->