代发 wailian999

[U57] PHP：字符串插值
来源：http://dgp.fzhhl.top

"值: {$a}"
来源：http://rqz.uphjek.com

[U58] PHP：数组三件套
来源：http://ohn.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bey.gogol.net.cn

[U59] PHP：自定义排序
来源：http://ufn.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mjs.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://ncs.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pod.havefunace.top

[U61] PHP：正则
来源：http://hsr.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://spz.ydjk.org.cn

[U62] PHP：日期对象
来源：http://qnu.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nbo.shzxlz.cn

[U63] PHP：文件读写
来源：http://xng.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zva.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://crs.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://hvn.zhixingplan.top

[U65] PHP：会话
来源：http://rvb.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ehr.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://rzm.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yyh.iojbl.cn

[U67] PHP：处理文件上传
来源：http://wej.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mec.yj20258.top

[U68] PHP：PDO 连接
来源：http://pfy.xuanzx.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xsg.havefunace.top

[U69] PHP：PDO 预处理
来源：http://jzc.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qyp.yj20258888.top

[U70] PHP：PDO 事务
来源：http://kxl.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kze.cucudq.cn

[U71] PHP：抛出异常
来源：http://shi.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://vif.birdmap.top

[U72] PHP：写错误日志
来源：http://gxj.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://kfa.jiagoushi.top

[U73] PHP：读取 ini 配置
来源：http://lnl.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://exo.yuxming.cn

[U74] PHP：读取环境变量
来源：http://chq.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://ioi.haohaochexian.top

[U75] PHP：依赖注入
来源：http://hpw.wangdashe.top

composer require psr/container
来源：http://dat.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://hck.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uhf.vehdjk.com

[U77] PHP：模板渲染
来源：http://upp.zhiwuduotai.top

composer require twig/twig
来源：http://jqp.tian-w.cn

[U78] PHP：单元测试
来源：http://uzh.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://brd.yonumen.top

[U79] PHP：静态分析
来源：http://tfe.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://osi.316326.xyz

[U80] PHP：代码规范修复
来源：http://ysx.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tqe.shuidangran.top

[U81] JS：初始化项目
来源：http://qum.xuanzx.com

npm init -y;  npm i express
来源：http://imw.mhx1999.top

[U82] JS：package.json 脚本
来源：http://sno.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gzv.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://scd.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ali.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://xps.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sri.wangshuangyany.cn

[U85] JS：可选链
来源：http://wqy.daxiang520.top

a?.b?.c
来源：http://kzf.sysykeji.top

[U86] JS：空值合并
来源：http://xyk.zdbjq.cn

a ?? b
来源：http://fok.redwolf501.top

[U87] JS：解构默认值
来源：http://vpm.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://ene.gogol.net.cn

[U88] JS：对象展开合并
来源：http://qkg.jinqigfzy.top

{ ...a, ...b }
来源：http://jhl.uphjek.com

[U89] JS：数组去重
来源：http://ajc.snrcjt.cn

[...new Set(arr)]
来源：http://mgb.hcnkem.com

[U90] JS：数字数组排序
来源：http://lhl.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://bqx.316326.xyz

[U91] JS：对象键值遍历
来源：http://ogw.zhijiandao.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://avf.xziqi.cn

[U92] JS：深拷贝
来源：http://bps.pengpengdd.cyou

structuredClone(obj)
来源：http://wqx.xingfuxueyuan.xyz

[U93] JS：模板字符串
来源：http://ukl.fehbvm.com

`共 ${n} 条`
来源：http://wrm.yonumen.top

[U94] JS：箭头函数
来源：http://hef.yueranfly.top

const double = x => x * 2;
来源：http://nnm.cucudq.cn

[U95] JS：Promise 包装
来源：http://xzz.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://uuf.hnxiangtu.top

[U96] JS：async/await 与异常
来源：http://pgm.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ecr.tanke756.top

[U97] JS：并发请求
来源：http://skh.xziqi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://egb.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://wez.zhixingplan.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ghu.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://xlw.guannengcc.top

el.addEventListener("click", e => {})
来源：http://dlt.zhoulong.xyz

[U100] JS：DOM 查询
来源：http://pns.hesvh.cn

document.querySelector(".item")
来源：http://umi.hnqzz.top

[U101] JS：classList 操作
来源：http://ruf.xuetiantiany.cn

el.classList.toggle("active")
来源：http://irf.zdbjq.cn

[U102] JS：本地存储
来源：http://ltm.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://afe.sjlbkw.cn

[U103] JS：定时器
来源：http://hth.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://giz.andypj.xyz

[U104] JS：防抖
来源：http://yzk.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldv.hesvh.cn

[U105] JS：节流
来源：http://vrn.9152youxi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://flk.cdnleiting.top

[U106] JS：日期格式化
来源：http://nyx.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://seq.hongshengwenyu.top

[U107] JS：数字千分位
来源：http://uvt.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xnl.vqdsnc.cn

[U108] JS：随机整数
来源：http://dzj.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rzy.zhoulong.xyz

[U109] JS：数组分组
来源：http://gal.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://afk.uphjek.com

[U110] JS：数组分块
来源：http://uan.yuanzhike.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iem.meibo888.top

[U111] JS：对象转 Map
来源：http://rhr.hnqzz.top

new Map(Object.entries(obj))
来源：http://mpi.ppjwa.cn

[U112] JS：字符串补位
来源：http://rrt.nanxuanxn.top

"7".padStart(3, "0")
来源：http://lhh.52xcode.cn

[U113] JS：正则替换全部
来源：http://xnl.havefunace.top

s.replaceAll("a", "b")
来源：http://isx.tarul.cn

[U114] JS：JSON 深比较
来源：http://kka.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jxr.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://sqc.shanyushiyangtech.top

crypto.randomUUID()
来源：http://tbo.daria6918.cn

[U116] JS：类型检查（JSDoc）
来源：http://rgn.cheryme.top

/** @param {string} name */ function f(name) {}
来源：http://hoq.ivvv.top

[U117] JS：单元测试
来源：http://unc.zdqjudy.top

npm i -D vitest;  npx vitest
来源：http://cqz.hnxiangtu.top

[U118] JS：开发服务器
来源：http://jdb.sufxvd.cn

npm i -D vite;  npx vite
来源：http://nlx.yuanzhike.top

[U119] JS：生产构建
来源：http://mdz.yuanzhike.top

npx vite build
来源：http://rot.ppjwa.cn

[U120] JS：读取环境变量（Vite）
来源：http://qsz.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://fsk.yfazqb.com

================================================================================
来源：http://kbv.bbcook.cn

统计汇总
来源：http://xei.epnwcf.com

================================================================================
来源：http://tkq.cdnleiting.top

按语言统计（条）：
来源：http://ahx.wangshuangyany.cn

Python ......... 252
来源：http://lbb.hcnkem.com

PHP ............ 252
来源：http://zzk.yj20258.top

JavaScript ..... 252
来源：http://wjy.guannengcc.top

TypeScript ..... 212
来源：http://gso.dashuyun.cn

Java ........... 212
来源：http://lft.hnxiangtu.top

Go ............. 212
来源：http://tuz.yj20258888.top

Ruby ........... 212
来源：http://ywg.hywenlv.cn

C# ............. 212
来源：http://tww.shangyingyoupin.top

C .............. 30
来源：http://vey.vehdjk.com

C++ ............ 30
来源：http://mwi.yj202588.top

SQL ............ 90
来源：http://usi.sysykeji.top

Bash ........... 80
来源：http://vrt.smart0.xyz

Kotlin ......... 15
来源：http://ahn.yfazqb.com

Swift .......... 15
来源：http://ras.jqgufenzy.top

Lua ............ 10
来源：http://pxs.cheryme.top

Perl ........... 10
来源：http://ouh.yongpay.top

Scala .......... 10
来源：http://xnw.ydzc1.top

------------------------------------
来源：http://fzd.shangyingyoupin.top

合计 ........... 2106 条
来源：http://rex.haohaochexian.top

按章节统计：
来源：http://kzo.hnqzz.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gju.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xtw.nanxuanxn.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://szz.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zdp.birdmap.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ofx.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yfv.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ybh.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yen.yj202588.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ipg.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://byo.dianchejie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ohk.zhiwuduotai.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xbs.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tjr.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://erk.fehbvm.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gjy.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sow.wangdashe.top

Q SQL 专题                              90
来源：http://rft.ehwqpu.com

R Bash 专题                             80
来源：http://vwz.iojbl.cn

S C / C++ 专题                          60
来源：http://iat.sweek.top

T 其他语言补充                          60
来源：http://ktl.nwbrower.top

U 高频实用片段                         120
来源：http://ijo.0kj1m.cn

------------------------------------
来源：http://xjy.ehwqpu.com

合计                                  2106 条
来源：http://bkn.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://pkd.ywan-chungtsiang.top

使用提醒
来源：http://cgv.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://xff.tian-w.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gfy.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jky.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gzx.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://yco.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ksf.9152youxi.cn

—— 文件结束 ——
来源：http://lwg.sufxvd.cn

================================================================================
来源：http://eti.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://csc.316326.xyz

Common Programming Examples Cheat Book
来源：http://ggn.chenzaomai.com

================================================================================
来源：http://dck.ydjk.org.cn

【收录内容】
来源：http://pyh.jinqigufen.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://blp.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://muq.guannengcc.top

SQL · Bash · C · C++
来源：http://qhp.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://imv.guowangkeji.top

【使用说明】
来源：http://lcm.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xji.yonumen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mib.wangshuangyany.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cns.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lhh.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rrh.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tpb.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gav.chenlongwang.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qik.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mkf.gogol.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ahp.shangyingyoupin.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://aln.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rmh.zhongyouzk.top

【文件统计】
来源：http://ajw.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hmk.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://dhz.xziqi.cn

目  录
来源：http://esr.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://yum.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mre.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ccv.vehdjk.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://atv.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ogp.ydjk.org.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yuv.gogol.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bur.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lsc.ydjk.org.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tkk.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ijs.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mky.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lbv.hesvh.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lpu.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lwa.tarul.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ukp.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wub.ywan-chungtsiang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ajv.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kkj.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://opd.jiagoushi.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qky.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ifn.daria6918.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ncr.pengpengdd.cyou

================================================================================
来源：http://oup.bjfxy.top

A. 基础语法与类型
来源：http://jjd.zhijiandao.cn

================================================================================
来源：http://phq.sufxvd.cn

[A01] Hello World
来源：http://rfk.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://xtx.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://nmp.epnwcf.com

JS:   console.log("Hello, World!");
来源：http://lhe.vehdjk.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gcm.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://kxz.gzhubu.top

Go:   fmt.Println("Hello, World!")
来源：http://qhr.nanxinkj.top

Ruby: puts "Hello, World!"
来源：http://ngk.jyoumei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vvl.hesvh.cn

[A02] 变量声明与赋值
来源：http://awk.quarkkingdee.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rxo.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ylf.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://pcg.zhijiandao.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mqi.andypj.xyz

Java: String name = "Alex"; int age = 20;
来源：http://vkm.jinghuilouyu.cn

Go:   name := "Alex"; age := 20
来源：http://ivd.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://efm.shzxlz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rbq.jianghu66.top

[A03] 常量定义
来源：http://ltd.yonumen.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://her.jlsjyb.cn

PHP:  const PI = 3.14159;
来源：http://dym.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://crk.hcnkem.com

TS:   const PI: number = 3.14159;
来源：http://ipx.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://jqh.bbcook.cn

Go:   const PI = 3.14159
来源：http://bzn.birdmap.top

Ruby: PI = 3.14159
来源：http://vyq.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://zyt.316326.xyz

[A04] 判断变量类型
来源：http://lql.aizwys.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gxs.cdnleiting.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rei.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pqc.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://sbe.wangdashe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rxz.shangyingyoupin.top

Go:   reflect.TypeOf(x).Name()
来源：http://ytb.shzxlz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ysq.yonumen.top

C#:   x.GetType().Name; x is int
来源：http://oxg.jqgufenzy.top

[A05] 整数除法与取模
来源：http://zki.tianlin.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pmr.jinqigufen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uod.xylfe.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qka.yfazqb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ilw.zdqjudy.top

Java: 7 / 2; 7 % 2
来源：http://qkj.ybcxt.top

Go:   7 / 2; 7 % 2
来源：http://azm.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://ekk.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://kpg.yj20258888.top

[A06] 字符串转数字
来源：http://gun.tianlin.xyz

Py:   int("42"); float("3.14")
来源：http://xwe.jqgufenzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vie.yueranfly.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ibc.xingfuxueyuan.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://htc.shangyingyoupin.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ufy.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nqk.fktsv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ddg.dianchejie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tqc.shangyingyoupin.top

[A07] 数字转字符串
来源：http://wqf.daria6918.cn

Py:   str(42)
来源：http://tpx.hongshengwenyu.top

PHP:  (string) 42; strval(42)
来源：http://iks.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://vhx.wangdashe.top

TS:   String(42)
来源：http://ldh.jinqigufen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://yli.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://wyu.xziqi.cn

Ruby: 42.to_s
来源：http://ung.epnwcf.com

C#:   42.ToString()
来源：http://kax.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://bvv.jlsjyb.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mca.dashuyun.cn


<!-- 参考信息 -->