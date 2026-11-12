代发 wailian999

[U59] PHP：自定义排序
来源：http://ysd.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fdy.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://fok.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kxe.yj20258888.top

[U61] PHP：正则
来源：http://wlp.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lkw.ydzc1.top

[U62] PHP：日期对象
来源：http://mge.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wwf.0kj1m.cn

[U63] PHP：文件读写
来源：http://vuw.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fmo.andypj.xyz

[U64] PHP：目录遍历
来源：http://rgh.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://agl.daxiang520.top

[U65] PHP：会话
来源：http://qfk.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ssx.meibo888.top

[U66] PHP：设置 Cookie
来源：http://jab.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hjf.redwolf501.top

[U67] PHP：处理文件上传
来源：http://etw.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uvp.yuxming.cn

[U68] PHP：PDO 连接
来源：http://hdi.fengsongda.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://civ.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://ufm.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sgs.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://yni.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nkl.dashuyun.cn

[U71] PHP：抛出异常
来源：http://ynm.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://hby.tanke756.top

[U72] PHP：写错误日志
来源：http://jjg.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://jmh.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://lrd.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://wmg.ybcxt.top

[U74] PHP：读取环境变量
来源：http://quy.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://uas.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://ssw.zhijiandao.cn

composer require psr/container
来源：http://jct.snrcjt.cn

[U76] PHP：简单路由
来源：http://pqx.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lto.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://tvu.hfpthk.cn

composer require twig/twig
来源：http://ddl.shangyingyoupin.top

[U78] PHP：单元测试
来源：http://mtj.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://rfe.ivvv.top

[U79] PHP：静态分析
来源：http://czs.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://ugn.xingfuxueyuan.xyz

[U80] PHP：代码规范修复
来源：http://xlz.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://fgc.sysykeji.top

[U81] JS：初始化项目
来源：http://kem.jqgufenzy.top

npm init -y;  npm i express
来源：http://feh.ivvv.top

[U82] JS：package.json 脚本
来源：http://zyq.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://puj.hammf.cn

[U83] JS：ES Module 导入导出
来源：http://trl.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://del.jinghuilouyu.cn

[U84] JS：CommonJS 写法
来源：http://wtd.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://xvz.zhongyouzk.top

[U85] JS：可选链
来源：http://prg.shzxlz.cn

a?.b?.c
来源：http://jyp.zhongyouzk.top

[U86] JS：空值合并
来源：http://bey.yonumen.top

a ?? b
来源：http://lxd.fengsongda.top

[U87] JS：解构默认值
来源：http://psp.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://deg.yueranfly.top

[U88] JS：对象展开合并
来源：http://oss.birdmap.top

{ ...a, ...b }
来源：http://vrk.dianchejie.cn

[U89] JS：数组去重
来源：http://qxj.hongshengwenyu.top

[...new Set(arr)]
来源：http://muc.havefunace.top

[U90] JS：数字数组排序
来源：http://bnh.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://ebf.xziqi.cn

[U91] JS：对象键值遍历
来源：http://sbx.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nuj.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://ppz.tarul.cn

structuredClone(obj)
来源：http://qux.andypj.xyz

[U93] JS：模板字符串
来源：http://gud.sweek.top

`共 ${n} 条`
来源：http://hcd.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://yus.mhx1999.top

const double = x => x * 2;
来源：http://gts.fengsongda.top

[U95] JS：Promise 包装
来源：http://ukh.ctjpmb.com

new Promise((resolve, reject) => {})
来源：http://jys.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://qrs.ybcxt.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lzc.jlsjyb.cn

[U97] JS：并发请求
来源：http://jyj.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nku.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://ztt.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://paj.tianlin.xyz

[U99] JS：事件监听
来源：http://scb.yj202588.top

el.addEventListener("click", e => {})
来源：http://aab.sufxvd.cn

[U100] JS：DOM 查询
来源：http://kwn.zhengqikj.top

document.querySelector(".item")
来源：http://zuk.xylfe.cn

[U101] JS：classList 操作
来源：http://fhw.zdqjudy.top

el.classList.toggle("active")
来源：http://cza.iojbl.cn

[U102] JS：本地存储
来源：http://pmj.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mpa.zhixingplan.top

[U103] JS：定时器
来源：http://qfk.ywan-chungtsiang.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ryu.yfazqb.com

[U104] JS：防抖
来源：http://yus.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sjg.nanxinkj.top

[U105] JS：节流
来源：http://sxa.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gkt.sxryk.cn

[U106] JS：日期格式化
来源：http://lrp.jlsjyb.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mos.fktsv.cn

[U107] JS：数字千分位
来源：http://zyx.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rgy.chenlongwang.top

[U108] JS：随机整数
来源：http://hso.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://unm.tianlin.xyz

[U109] JS：数组分组
来源：http://ngf.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://sok.sysykeji.top

[U110] JS：数组分块
来源：http://vgb.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sde.mhx1999.top

[U111] JS：对象转 Map
来源：http://pwe.yj20258.top

new Map(Object.entries(obj))
来源：http://ema.yuanzhike.top

[U112] JS：字符串补位
来源：http://djx.nanxuanxn.top

"7".padStart(3, "0")
来源：http://gom.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://xus.hcnkem.com

s.replaceAll("a", "b")
来源：http://paw.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://ftc.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yip.jinyuanbaomall.cn

[U115] JS：生成 UUID
来源：http://dbp.smart0.xyz

crypto.randomUUID()
来源：http://llp.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://gnm.tanke756.top

/** @param {string} name */ function f(name) {}
来源：http://mid.gzhubu.top

[U117] JS：单元测试
来源：http://utb.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://ens.9152youxi.cn

[U118] JS：开发服务器
来源：http://bhw.yueranfly.top

npm i -D vite;  npx vite
来源：http://ehf.vqdsnc.cn

[U119] JS：生产构建
来源：http://rgh.xinyue.icu

npx vite build
来源：http://pft.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://quc.tanke756.top

import.meta.env.VITE_API_URL
来源：http://hoj.tian-w.cn

================================================================================
来源：http://wsm.iojbl.cn

统计汇总
来源：http://wjx.shzxlz.cn

================================================================================
来源：http://gah.yj20258888.top

按语言统计（条）：
来源：http://aor.dashuyun.cn

Python ......... 252
来源：http://quk.tarul.cn

PHP ............ 252
来源：http://ocf.daxiang520.top

JavaScript ..... 252
来源：http://vzq.yfazqb.com

TypeScript ..... 212
来源：http://jym.daxiang520.top

Java ........... 212
来源：http://yiq.haohaochexian.top

Go ............. 212
来源：http://vfy.fktsv.cn

Ruby ........... 212
来源：http://cun.iojbl.cn

C# ............. 212
来源：http://geg.jqgfzy.top

C .............. 30
来源：http://fbn.tian-w.cn

C++ ............ 30
来源：http://fyp.yj202588.top

SQL ............ 90
来源：http://bmf.jinqigufen.top

Bash ........... 80
来源：http://trd.tanke756.top

Kotlin ......... 15
来源：http://dxp.havefunace.top

Swift .......... 15
来源：http://ook.guowangkeji.top

Lua ............ 10
来源：http://jvz.zdbjq.cn

Perl ........... 10
来源：http://nuz.zhiwuduotai.top

Scala .......... 10
来源：http://dlc.zhengqikj.top

------------------------------------
来源：http://ils.hnxiangtu.top

合计 ........... 2106 条
来源：http://wia.xuetiantiany.cn

按章节统计：
来源：http://jbq.tianlin.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wky.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xqn.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rrb.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tqx.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ksr.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kzm.ppjwa.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://idc.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yxq.yonumen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sfg.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://byw.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://brh.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qvn.sysykeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://auf.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kza.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cwz.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://atn.mhx1999.top

Q SQL 专题                              90
来源：http://mlp.epnwcf.com

R Bash 专题                             80
来源：http://ehx.gaohongyu789.top

S C / C++ 专题                          60
来源：http://psp.jiagoushi.top

T 其他语言补充                          60
来源：http://aji.yangfankeji.com

U 高频实用片段                         120
来源：http://bwj.hcnkem.com

------------------------------------
来源：http://kem.kuanghao11.cn

合计                                  2106 条
来源：http://gtl.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://sdp.zycfv.cn

使用提醒
来源：http://vny.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://yue.yj202588.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://unc.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bxg.gzhubu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lex.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kov.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oeo.jinqigfzy.top

—— 文件结束 ——
来源：http://ban.epnwcf.com

================================================================================
来源：http://nnv.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://bjw.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://jca.quarkkingdee.top

================================================================================
来源：http://nym.52xcode.cn

【收录内容】
来源：http://onk.52xcode.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dwe.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cwj.yangfankeji.com

SQL · Bash · C · C++
来源：http://ocd.jinghuilouyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nav.shanyushiyangtech.top

【使用说明】
来源：http://ywb.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ugw.xziqi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wwj.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xgz.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://use.quarkkingdee.top

Bash:  Shell         C:     C             C++:   C++
来源：http://imq.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ecz.cashguo.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://svm.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xag.xuanzx.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rev.hongshengwenyu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zhn.guannengcc.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fwu.zhaomingkeji.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ccn.uphjek.com

【文件统计】
来源：http://muk.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sfk.pycfn.com

--------------------------------------------------------------------------------
来源：http://gzy.nanxinkj.top

目  录
来源：http://dih.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://icc.sjlbkw.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xvh.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rnu.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jpb.aibaodan.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://noe.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://txe.hesvh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gbo.0kj1m.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ryv.kuanghao11.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rjt.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pwm.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dqb.fengsongda.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eex.zhixingplan.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nzl.vehdjk.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://emg.yongpay.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://opg.zhiwuduotai.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jmf.c1oappe.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://njc.hnxiangtu.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ysh.yj202588.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://puv.sxryk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://llx.hfpthk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvt.quarkkingdee.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cjy.tarul.cn

================================================================================
来源：http://cmn.chenjidiqi.icu

A. 基础语法与类型
来源：http://rvl.tarul.cn

================================================================================
来源：http://zbf.fktsv.cn

[A01] Hello World
来源：http://igi.ivvv.top

Py:   print("Hello, World!")
来源：http://meh.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://xlu.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://pda.jqgfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://toa.jianghu66.top

Java: System.out.println("Hello, World!");
来源：http://vgx.shanyushiyangtech.top

Go:   fmt.Println("Hello, World!")
来源：http://tdy.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://jrs.ywan-chungtsiang.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mdb.c1oappe.top

[A02] 变量声明与赋值
来源：http://vcc.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uqb.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zzt.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://jpk.daxiang520.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pyv.fzhhl.top

Java: String name = "Alex"; int age = 20;
来源：http://sha.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://exc.zhengqikj.top

Ruby: name = "Alex"; age = 20
来源：http://avi.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aqw.jinghuilouyu.cn

[A03] 常量定义
来源：http://pwr.wangshuangyany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uxd.ybcxt.top

PHP:  const PI = 3.14159;
来源：http://epl.yfazqb.com

JS:   const PI = 3.14159;
来源：http://ohg.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://pfd.shangyingyoupin.top

Java: static final double PI = 3.14159;
来源：http://bwr.zdbjq.cn

Go:   const PI = 3.14159
来源：http://xav.jinqigufen.top

Ruby: PI = 3.14159
来源：http://ybl.hfpthk.cn

C#:   const double PI = 3.14159;
来源：http://kwo.cashguo.top

[A04] 判断变量类型
来源：http://kzc.xuanzx.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://mza.zhijiandao.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hra.mhx1999.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zcc.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://wba.hnqzz.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tob.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rkc.aibaodan.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tvo.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://rmp.cqqwz.cn

[A05] 整数除法与取模
来源：http://viy.yangfankeji.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ges.nanxinkj.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xso.xuetiantiany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jnd.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qaj.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://qhd.cashguo.top

Go:   7 / 2; 7 % 2
来源：http://vvr.shzxlz.cn

Ruby: 7 / 2; 7 % 2
来源：http://vcf.zhengqikj.top

C#:   7 / 2; 7 % 2
来源：http://bol.jinqigufen.top

[A06] 字符串转数字
来源：http://dcf.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://dea.sjlbkw.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://joj.andypj.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cdf.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://woq.yvedp.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yom.meibo888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yjh.cashguo.top

Ruby: "42".to_i; "3.14".to_f
来源：http://imc.yj20258888.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://onm.hammf.cn

[A07] 数字转字符串
来源：http://jys.9152youxi.cn

Py:   str(42)
来源：http://oqb.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://hby.fehbvm.com

JS:   String(42); (42).toString()
来源：http://uhn.chenlongwang.top

TS:   String(42)
来源：http://zml.fktsv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://pat.birdmap.top

Go:   strconv.Itoa(42)
来源：http://ean.aibaodan.cn

Ruby: 42.to_s
来源：http://vue.yj20258.top

C#:   42.ToString()
来源：http://lso.ydjk.org.cn

[A08] 取整与四舍五入
来源：http://zok.jiagoushi.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bhl.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xdx.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xqf.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lmp.ybcxt.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://see.bbcook.cn


<!-- 参考信息 -->