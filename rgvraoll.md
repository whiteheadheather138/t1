代发 wailian999

[U51] PHP：数组解构
来源：http://bar.hfpthk.cn

[$a, $b] = $arr;
来源：http://aug.xziqi.cn

[U52] PHP：箭头函数
来源：http://bgw.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://lbu.yj202588.top

[U53] PHP：空合并运算符
来源：http://zwn.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://bvz.tian-w.cn

[U54] PHP：空安全调用
来源：http://fuo.jinqigufen.top

$obj?->method()
来源：http://ebd.fktsv.cn

[U55] PHP：match 表达式
来源：http://pvk.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://adw.andypj.xyz

[U56] PHP：命名参数
来源：http://qtk.jiagoushi.top

f(a: 1, b: 2)
来源：http://dim.hfpthk.cn

[U57] PHP：字符串插值
来源：http://igi.fehbvm.com

"值: {$a}"
来源：http://hga.0kj1m.cn

[U58] PHP：数组三件套
来源：http://mjx.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://stf.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://bfq.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xlk.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://boe.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lxs.yuanzhike.top

[U61] PHP：正则
来源：http://hvu.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbu.jinqigfzy.top

[U62] PHP：日期对象
来源：http://kja.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ipm.c1oappe.top

[U63] PHP：文件读写
来源：http://mqo.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rcy.yj202588.top

[U64] PHP：目录遍历
来源：http://dsl.aizwys.cn

glob("dir/*.php");  scandir("dir");
来源：http://pdl.xylfe.cn

[U65] PHP：会话
来源：http://tay.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lia.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://wsy.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vlq.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://vti.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mrl.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://xjz.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tie.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://tsx.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://abb.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://utu.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wnm.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://ycz.chenjidiqi.icu

throw new RuntimeException("失败", 500);
来源：http://wem.cheryme.top

[U72] PHP：写错误日志
来源：http://fkf.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://fht.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://qkp.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://tyv.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://vdj.0kj1m.cn

getenv("APP_ENV") ?: "production"
来源：http://bes.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://aof.xinyue.icu

composer require psr/container
来源：http://ohs.gaohongyu789.top

[U76] PHP：简单路由
来源：http://obq.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uyw.yueranfly.top

[U77] PHP：模板渲染
来源：http://uak.fzhhl.top

composer require twig/twig
来源：http://ebf.yuxming.cn

[U78] PHP：单元测试
来源：http://gxl.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://mvd.guowangkeji.top

[U79] PHP：静态分析
来源：http://mzp.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://bsv.shzxlz.cn

[U80] PHP：代码规范修复
来源：http://xdq.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ddn.aizwys.cn

[U81] JS：初始化项目
来源：http://rck.yj20258.top

npm init -y;  npm i express
来源：http://fxz.uphjek.com

[U82] JS：package.json 脚本
来源：http://ozs.yangfankeji.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tmh.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://bww.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://gpi.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://heh.guannengcc.top

module.exports = { a };  const { a } = require("./m");
来源：http://buw.jyoumei.cn

[U85] JS：可选链
来源：http://lnw.hnxiangtu.top

a?.b?.c
来源：http://pdr.aizwys.cn

[U86] JS：空值合并
来源：http://vlo.ppjwa.cn

a ?? b
来源：http://sex.9152youxi.cn

[U87] JS：解构默认值
来源：http://cmq.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://uqy.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://aar.9152youxi.cn

{ ...a, ...b }
来源：http://jqk.jlsjyb.cn

[U89] JS：数组去重
来源：http://bgc.chenjidiqi.icu

[...new Set(arr)]
来源：http://zoc.jqgfzy.top

[U90] JS：数字数组排序
来源：http://yhz.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://uha.hammf.cn

[U91] JS：对象键值遍历
来源：http://gch.hysaishi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hpc.ivvv.top

[U92] JS：深拷贝
来源：http://xsc.jyoumei.cn

structuredClone(obj)
来源：http://uhj.ctjpmb.com

[U93] JS：模板字符串
来源：http://ibf.gotoacloud.top

`共 ${n} 条`
来源：http://lkd.yangfankeji.com

[U94] JS：箭头函数
来源：http://miv.nanxuanxn.top

const double = x => x * 2;
来源：http://wcr.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://tbw.daxiang520.top

new Promise((resolve, reject) => {})
来源：http://hul.uphjek.com

[U96] JS：async/await 与异常
来源：http://orz.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vzr.9152youxi.cn

[U97] JS：并发请求
来源：http://xas.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qev.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://byy.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zem.yj20258888.top

[U99] JS：事件监听
来源：http://gfr.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://hqx.tanke756.top

[U100] JS：DOM 查询
来源：http://jor.jqgfzy.top

document.querySelector(".item")
来源：http://cfc.hnxiangtu.top

[U101] JS：classList 操作
来源：http://tyy.ydzc1.top

el.classList.toggle("active")
来源：http://erm.wangshuangyany.cn

[U102] JS：本地存储
来源：http://sdm.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://thw.jyoumei.cn

[U103] JS：定时器
来源：http://gkm.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xlr.nanxinkj.top

[U104] JS：防抖
来源：http://yjf.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srp.snrcjt.cn

[U105] JS：节流
来源：http://ifo.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dln.jianghu66.top

[U106] JS：日期格式化
来源：http://mzm.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uwq.jianghu66.top

[U107] JS：数字千分位
来源：http://kco.zhiwuduotai.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kdm.aizwys.cn

[U108] JS：随机整数
来源：http://wgr.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ttf.0kj1m.cn

[U109] JS：数组分组
来源：http://hra.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://phh.aibaodan.cn

[U110] JS：数组分块
来源：http://cqr.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fch.c1oappe.top

[U111] JS：对象转 Map
来源：http://zyq.ybcxt.top

new Map(Object.entries(obj))
来源：http://dni.zhijiandao.cn

[U112] JS：字符串补位
来源：http://vxu.0kj1m.cn

"7".padStart(3, "0")
来源：http://wca.gzhubu.top

[U113] JS：正则替换全部
来源：http://cqp.kuanghao11.cn

s.replaceAll("a", "b")
来源：http://iid.c1oappe.top

[U114] JS：JSON 深比较
来源：http://aeb.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cvg.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://coc.pengpengdd.cyou

crypto.randomUUID()
来源：http://mnh.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://mud.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://epe.birdmap.top

[U117] JS：单元测试
来源：http://xmr.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://esd.jiagoushi.top

[U118] JS：开发服务器
来源：http://ttz.hywenlv.cn

npm i -D vite;  npx vite
来源：http://dkh.xuetiantiany.cn

[U119] JS：生产构建
来源：http://rpz.sweek.top

npx vite build
来源：http://orq.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://iai.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://vbo.316326.xyz

================================================================================
来源：http://wex.yanxiufei.cn

统计汇总
来源：http://wng.birdmap.top

================================================================================
来源：http://sde.ydjk.org.cn

按语言统计（条）：
来源：http://exu.ehwqpu.com

Python ......... 252
来源：http://bwc.sjlbkw.cn

PHP ............ 252
来源：http://ijp.tianlin.xyz

JavaScript ..... 252
来源：http://epb.ehwqpu.com

TypeScript ..... 212
来源：http://hvb.fengsongda.top

Java ........... 212
来源：http://kco.chenjidiqi.icu

Go ............. 212
来源：http://hjj.jinyuanbaomall.cn

Ruby ........... 212
来源：http://kel.zycfv.cn

C# ............. 212
来源：http://rfl.zdqjudy.top

C .............. 30
来源：http://wyt.bbcook.cn

C++ ............ 30
来源：http://yzf.ybcxt.top

SQL ............ 90
来源：http://hle.pycfn.com

Bash ........... 80
来源：http://mej.hammf.cn

Kotlin ......... 15
来源：http://mvy.shuidangran.top

Swift .......... 15
来源：http://bav.shangyingyoupin.top

Lua ............ 10
来源：http://fiz.jinghuilouyu.cn

Perl ........... 10
来源：http://wvm.hesvh.cn

Scala .......... 10
来源：http://ynn.yfazqb.com

------------------------------------
来源：http://hto.ybcxt.top

合计 ........... 2106 条
来源：http://efd.sweek.top

按章节统计：
来源：http://krw.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pep.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tyn.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hbw.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pxv.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://trv.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jiu.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hrv.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ulb.sysykeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://piy.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wez.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jis.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nbz.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zoe.xinyue.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://faq.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eba.jqgfzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rvz.vehdjk.com

Q SQL 专题                              90
来源：http://yfd.pycfn.com

R Bash 专题                             80
来源：http://xsf.dianchejie.cn

S C / C++ 专题                          60
来源：http://exe.shangyingyoupin.top

T 其他语言补充                          60
来源：http://qvs.yj20258888.top

U 高频实用片段                         120
来源：http://tus.wangdashe.top

------------------------------------
来源：http://uqm.xylfe.cn

合计                                  2106 条
来源：http://hkr.yuxming.cn

--------------------------------------------------------------------------------
来源：http://fre.sysykeji.top

使用提醒
来源：http://xsr.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://cvy.zhiwuduotai.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvi.fengsongda.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xah.ppjwa.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://daf.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vgz.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rsb.hesvh.cn

—— 文件结束 ——
来源：http://jjz.hysaishi.cn

================================================================================
来源：http://vjh.sysykeji.top

程序语言常见例子速查手册（2024 版）
来源：http://tnd.tanke756.top

Common Programming Examples Cheat Book
来源：http://dlm.yanxiufei.cn

================================================================================
来源：http://dus.xingfuxueyuan.xyz

【收录内容】
来源：http://sjl.wangshuangyany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vys.ehwqpu.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wzz.hcnkem.com

SQL · Bash · C · C++
来源：http://fhc.wangshuangyany.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://suw.xziqi.cn

【使用说明】
来源：http://mqi.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wdo.sufxvd.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zge.gzhubu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lwm.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vld.fktsv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hbv.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oer.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ncn.bbcook.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mcy.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iob.daria6918.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vch.zhiwuduotai.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://smp.chenlongwang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dyj.kuanghao11.cn

【文件统计】
来源：http://jlu.zhiwuduotai.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qqo.yuxming.cn

--------------------------------------------------------------------------------
来源：http://qks.wangshuangyany.cn

目  录
来源：http://cni.tanke756.top

--------------------------------------------------------------------------------
来源：http://ozu.hcnkem.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zoh.shangyingyoupin.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rua.yangfankeji.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pls.gzhubu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gpt.nanxinkj.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rib.tarul.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qoo.wangshuangyany.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xue.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bfe.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qta.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://btt.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nyp.pengpengdd.cyou

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://atu.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://egz.yj20258888.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nlt.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mkz.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rcr.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cks.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ezh.shanyushiyangkeji.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ozb.cqqwz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://eet.fengsongda.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yhm.xinyue.icu

================================================================================
来源：http://zoa.feifeiyinyue.top

A. 基础语法与类型
来源：http://lmc.nanxinkj.top

================================================================================
来源：http://fnr.jlsjyb.cn

[A01] Hello World
来源：http://wqa.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://lol.nanxuanxn.top

PHP:  echo "Hello, World!";
来源：http://cft.hammf.cn

JS:   console.log("Hello, World!");
来源：http://lek.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aic.jlsjyb.cn

Java: System.out.println("Hello, World!");
来源：http://mca.cdnleiting.top

Go:   fmt.Println("Hello, World!")
来源：http://kpk.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://mzs.ybcxt.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cgc.0kj1m.cn

[A02] 变量声明与赋值
来源：http://era.hywenlv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ubw.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://rkj.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://hem.zdqjudy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cha.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://pua.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://vxo.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://awv.shanyushiyangkeji.top

C#:   string name = "Alex"; int age = 20;
来源：http://tcp.hongshengwenyu.top

[A03] 常量定义
来源：http://gfw.gogol.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://etr.feifeiyinyue.top

PHP:  const PI = 3.14159;
来源：http://ymo.uphjek.com

JS:   const PI = 3.14159;
来源：http://cdb.ppjwa.cn

TS:   const PI: number = 3.14159;
来源：http://qpi.chenlongwang.top

Java: static final double PI = 3.14159;
来源：http://cer.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://flc.jianghu66.top

Ruby: PI = 3.14159
来源：http://tui.shanyushiyangkeji.top

C#:   const double PI = 3.14159;
来源：http://vrw.nwbrower.top

[A04] 判断变量类型
来源：http://ssc.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xbv.xingfuxueyuan.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hwb.vehdjk.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mqa.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://ubb.zhongyouzk.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://adi.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tzh.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yvi.xingfuxueyuan.xyz

C#:   x.GetType().Name; x is int
来源：http://udr.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://jqa.wangshuangyany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://meg.zhiwuduotai.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://szv.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ctw.tian-w.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tib.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://vxj.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://zlk.tanke756.top

Ruby: 7 / 2; 7 % 2
来源：http://dzo.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://auq.fehbvm.com

[A06] 字符串转数字
来源：http://prx.chenzaomai.com

Py:   int("42"); float("3.14")
来源：http://qpo.fzhhl.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://msx.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xnm.gaohongyu789.top

TS:   parseInt("42", 10); Number("42")
来源：http://jkn.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ivx.xuanzx.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kyf.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ivo.uphjek.com


<!-- 参考信息 -->