代发 wailian999

[U59] PHP：自定义排序
来源：http://hea.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ahe.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://hkr.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://llg.yongpay.top

[U61] PHP：正则
来源：http://xta.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uyr.zhoulong.xyz

[U62] PHP：日期对象
来源：http://css.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uvt.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://skt.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dmn.xylfe.cn

[U64] PHP：目录遍历
来源：http://thr.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://ewi.52xcode.cn

[U65] PHP：会话
来源：http://zup.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ppk.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://zgq.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nei.andypj.xyz

[U67] PHP：处理文件上传
来源：http://vmu.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dxn.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://qhm.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mei.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://isd.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lgy.fengsongda.top

[U70] PHP：PDO 事务
来源：http://wic.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uaw.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://vxy.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://lta.meibo888.top

[U72] PHP：写错误日志
来源：http://zgi.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://nbj.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://fec.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://byn.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://yur.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://kts.daxiang520.top

[U75] PHP：依赖注入
来源：http://cef.shzxlz.cn

composer require psr/container
来源：http://fqg.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://kio.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xal.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://xhd.ehwqpu.com

composer require twig/twig
来源：http://fsv.cdnleiting.top

[U78] PHP：单元测试
来源：http://trg.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://nnm.52xcode.cn

[U79] PHP：静态分析
来源：http://gwk.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://awy.sxryk.cn

[U80] PHP：代码规范修复
来源：http://lfc.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jju.nanxinkj.top

[U81] JS：初始化项目
来源：http://rwo.nanxinkj.top

npm init -y;  npm i express
来源：http://axi.hesvh.cn

[U82] JS：package.json 脚本
来源：http://ptx.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zqh.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://flj.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://nsw.fzhhl.top

[U84] JS：CommonJS 写法
来源：http://njg.uphjek.com

module.exports = { a };  const { a } = require("./m");
来源：http://sru.sxryk.cn

[U85] JS：可选链
来源：http://rrv.shuidangran.top

a?.b?.c
来源：http://pyd.hcnkem.com

[U86] JS：空值合并
来源：http://yss.xuanzx.com

a ?? b
来源：http://zut.jiagoushi.top

[U87] JS：解构默认值
来源：http://bnc.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://yjy.c1oappe.top

[U88] JS：对象展开合并
来源：http://cpp.zhiwuduotai.top

{ ...a, ...b }
来源：http://xlf.zhoulong.xyz

[U89] JS：数组去重
来源：http://vpi.jiagoushi.top

[...new Set(arr)]
来源：http://bnj.hfpthk.cn

[U90] JS：数字数组排序
来源：http://nqx.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://ajk.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://xvw.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cvk.ydzc1.top

[U92] JS：深拷贝
来源：http://xrr.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://qyq.hongshengwenyu.top

[U93] JS：模板字符串
来源：http://egr.feifeiyinyue.top

`共 ${n} 条`
来源：http://fix.jianghu66.top

[U94] JS：箭头函数
来源：http://aub.jinghuilouyu.cn

const double = x => x * 2;
来源：http://lud.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://kfj.sweek.top

new Promise((resolve, reject) => {})
来源：http://wyx.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://ymd.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oal.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://vbz.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://gpg.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://qhn.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lqc.jianghu66.top

[U99] JS：事件监听
来源：http://ewy.fzhhl.top

el.addEventListener("click", e => {})
来源：http://hpb.zhijiandao.cn

[U100] JS：DOM 查询
来源：http://mtw.fzhhl.top

document.querySelector(".item")
来源：http://ils.aibaodan.cn

[U101] JS：classList 操作
来源：http://vhm.zhongyouzk.top

el.classList.toggle("active")
来源：http://iai.zhijiandao.cn

[U102] JS：本地存储
来源：http://wuo.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://byj.sweek.top

[U103] JS：定时器
来源：http://wtp.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tyb.tian-w.cn

[U104] JS：防抖
来源：http://php.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dcg.sysykeji.top

[U105] JS：节流
来源：http://knr.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qod.aibaodan.cn

[U106] JS：日期格式化
来源：http://lia.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wxa.yfazqb.com

[U107] JS：数字千分位
来源：http://nsn.xuetiantiany.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cjb.zhaomingkeji.xyz

[U108] JS：随机整数
来源：http://gya.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ajw.yongpay.top

[U109] JS：数组分组
来源：http://ibo.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://adf.cqqwz.cn

[U110] JS：数组分块
来源：http://dcd.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xns.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://mfv.tian-w.cn

new Map(Object.entries(obj))
来源：http://zyq.bbcook.cn

[U112] JS：字符串补位
来源：http://jha.mhx1999.top

"7".padStart(3, "0")
来源：http://gug.ybcxt.top

[U113] JS：正则替换全部
来源：http://rqu.chenzaomai.com

s.replaceAll("a", "b")
来源：http://wkc.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://sof.hfpthk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pps.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://elf.ydjk.org.cn

crypto.randomUUID()
来源：http://pmh.sweek.top

[U116] JS：类型检查（JSDoc）
来源：http://xmc.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://zrb.wangshuangyany.cn

[U117] JS：单元测试
来源：http://tum.pycfn.com

npm i -D vitest;  npx vitest
来源：http://wnh.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://mtf.jyoumei.cn

npm i -D vite;  npx vite
来源：http://nbs.yj20258.top

[U119] JS：生产构建
来源：http://adc.jyoumei.cn

npx vite build
来源：http://fgv.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://ykp.kuanghao11.cn

import.meta.env.VITE_API_URL
来源：http://jvc.pycfn.com

================================================================================
来源：http://toa.xingfuxueyuan.xyz

统计汇总
来源：http://iwh.shangyingyoupin.top

================================================================================
来源：http://oet.ctjpmb.com

按语言统计（条）：
来源：http://qkp.fktsv.cn

Python ......... 252
来源：http://gcd.cashguo.top

PHP ............ 252
来源：http://czq.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://wpe.0kj1m.cn

TypeScript ..... 212
来源：http://ncb.vehdjk.com

Java ........... 212
来源：http://edb.cucudq.cn

Go ............. 212
来源：http://egx.yuanzhike.top

Ruby ........... 212
来源：http://upo.ctjpmb.com

C# ............. 212
来源：http://zlm.gogol.net.cn

C .............. 30
来源：http://cmh.hcnkem.com

C++ ............ 30
来源：http://jyl.pengpengdd.cyou

SQL ............ 90
来源：http://zdf.jinqigfzy.top

Bash ........... 80
来源：http://kqv.cdnleiting.top

Kotlin ......... 15
来源：http://khj.bjfxy.top

Swift .......... 15
来源：http://pqc.yj20258888.top

Lua ............ 10
来源：http://hbv.xinyue.icu

Perl ........... 10
来源：http://pxl.tarul.cn

Scala .......... 10
来源：http://fhm.havefunace.top

------------------------------------
来源：http://wgs.epnwcf.com

合计 ........... 2106 条
来源：http://yxe.aizwys.cn

按章节统计：
来源：http://ijl.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ezz.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vlw.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lwi.52xcode.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://czu.xuetiantiany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://diu.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://umr.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://olt.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vhc.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hqw.hongshengwenyu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kaz.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vvs.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fbc.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pxp.kuanghao11.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aul.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://awy.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zow.chenlongwang.top

Q SQL 专题                              90
来源：http://jmp.sufxvd.cn

R Bash 专题                             80
来源：http://plc.xuanzx.com

S C / C++ 专题                          60
来源：http://cxd.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://bko.zhijiandao.cn

U 高频实用片段                         120
来源：http://vrf.jlsjyb.cn

------------------------------------
来源：http://rae.smart0.xyz

合计                                  2106 条
来源：http://dos.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://usi.hesvh.cn

使用提醒
来源：http://cay.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://gjs.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lwu.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aec.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kjm.52xcode.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dck.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://beh.zhijiandao.cn

—— 文件结束 ——
来源：http://tiu.cqqwz.cn

================================================================================
来源：http://dod.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://ylw.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://ewu.fehbvm.com

================================================================================
来源：http://ran.guowangkeji.top

【收录内容】
来源：http://zjp.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://mpe.sjlbkw.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xsl.jianghu66.top

SQL · Bash · C · C++
来源：http://rpr.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cef.xylfe.cn

【使用说明】
来源：http://hcr.yangfankeji.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cyl.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fje.tian-w.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://knb.jinqigfzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yhh.hysaishi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qfh.gotoacloud.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mzy.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qrp.zhijiandao.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vmk.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kut.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://osw.chenlongwang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mpa.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eiv.c1oappe.top

【文件统计】
来源：http://hpt.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jcd.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://vxo.ivvv.top

目  录
来源：http://wdr.bbcook.cn

--------------------------------------------------------------------------------
来源：http://kos.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gym.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hcw.hywenlv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ldc.wangdashe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://asr.pycfn.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xrx.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://miu.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bdw.dashuyun.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lnb.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kzt.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ffn.ppjwa.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wug.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mql.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wta.hywenlv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://djp.jinqigufen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iox.zhaomingkeji.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mjn.yj20258.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fra.yongpay.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://viu.sjlbkw.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jwp.tanke756.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oet.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iaf.xingfuxueyuan.xyz

================================================================================
来源：http://czb.jlsjyb.cn

A. 基础语法与类型
来源：http://uny.tianlin.xyz

================================================================================
来源：http://kng.mhx1999.top

[A01] Hello World
来源：http://zqa.pengpengdd.cyou

Py:   print("Hello, World!")
来源：http://bzh.zdbjq.cn

PHP:  echo "Hello, World!";
来源：http://zis.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://yfw.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ttz.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://ezy.52xcode.cn

Go:   fmt.Println("Hello, World!")
来源：http://hqy.smart0.xyz

Ruby: puts "Hello, World!"
来源：http://gzc.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nvq.tian-w.cn

[A02] 变量声明与赋值
来源：http://lfa.tanke756.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ycf.ywan-chungtsiang.top

PHP:  $name = "Alex"; $age = 20;
来源：http://asa.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://nph.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ijf.chenlongwang.top

Java: String name = "Alex"; int age = 20;
来源：http://anz.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://oed.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://waw.daria6918.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cjz.birdmap.top

[A03] 常量定义
来源：http://nkz.aizwys.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rmi.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://xof.xinyue.icu

JS:   const PI = 3.14159;
来源：http://yzv.meibo888.top

TS:   const PI: number = 3.14159;
来源：http://zmn.ivvv.top

Java: static final double PI = 3.14159;
来源：http://zqh.wangdashe.top

Go:   const PI = 3.14159
来源：http://avb.tanke756.top

Ruby: PI = 3.14159
来源：http://mbc.jiagoushi.top

C#:   const double PI = 3.14159;
来源：http://rri.gogol.net.cn

[A04] 判断变量类型
来源：http://tcb.shanyushiyangtech.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cla.hesvh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uct.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zwh.jqgufenzy.top

TS:   typeof x; x instanceof Date
来源：http://vqw.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yuz.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://xrb.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://obt.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://zrf.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://udt.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ilh.snrcjt.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tlo.daria6918.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nrs.jqgfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dnm.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://anr.yvedp.cn

Go:   7 / 2; 7 % 2
来源：http://eqn.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://jtq.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://zew.meibo888.top

[A06] 字符串转数字
来源：http://yuw.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://qwe.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vqb.yvedp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://owt.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vvb.hywenlv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dcm.cashguo.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tfz.ehwqpu.com

Ruby: "42".to_i; "3.14".to_f
来源：http://omr.tianlin.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yma.dashuyun.cn

[A07] 数字转字符串
来源：http://aey.bjfxy.top

Py:   str(42)
来源：http://www.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://efb.ywan-chungtsiang.top

JS:   String(42); (42).toString()
来源：http://wbf.ivvv.top

TS:   String(42)
来源：http://geb.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qqr.iojbl.cn

Go:   strconv.Itoa(42)
来源：http://toj.yuanzhike.top

Ruby: 42.to_s
来源：http://srr.havefunace.top

C#:   42.ToString()
来源：http://xlp.hfpthk.cn

[A08] 取整与四舍五入
来源：http://ury.hywenlv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wbh.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tub.xuanzx.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rru.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wmr.cashguo.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gyv.epnwcf.com


<!-- 参考信息 -->