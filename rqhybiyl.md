代发 wailian999

[U53] PHP：空合并运算符
来源：http://lyz.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://ewg.zycfv.cn

[U54] PHP：空安全调用
来源：http://mpe.wangshuangyany.cn

$obj?->method()
来源：http://ozj.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://sos.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zxj.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://egx.yvedp.cn

f(a: 1, b: 2)
来源：http://wal.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://pzk.redwolf501.top

"值: {$a}"
来源：http://fdu.xuanzx.com

[U58] PHP：数组三件套
来源：http://trf.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xwi.cucudq.cn

[U59] PHP：自定义排序
来源：http://aiw.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dzc.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://zki.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jqr.yj202588.top

[U61] PHP：正则
来源：http://jyw.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sjk.cqqwz.cn

[U62] PHP：日期对象
来源：http://lwm.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mgh.wangdashe.top

[U63] PHP：文件读写
来源：http://buq.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wjb.hcnkem.com

[U64] PHP：目录遍历
来源：http://wbq.sxryk.cn

glob("dir/*.php");  scandir("dir");
来源：http://yhr.guannengcc.top

[U65] PHP：会话
来源：http://kzs.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://svt.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://oev.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ott.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://dwt.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hwn.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://miv.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oav.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://gbi.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hfa.jianghu66.top

[U70] PHP：PDO 事务
来源：http://qfv.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://klz.guowangkeji.top

[U71] PHP：抛出异常
来源：http://ywr.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://bmm.zdbjq.cn

[U72] PHP：写错误日志
来源：http://iwv.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://ome.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://mjw.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://cbz.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://ofr.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://nlc.wangdashe.top

[U75] PHP：依赖注入
来源：http://hxw.snrcjt.cn

composer require psr/container
来源：http://dsh.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://qjm.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lxl.9152youxi.cn

[U77] PHP：模板渲染
来源：http://rqf.cashguo.top

composer require twig/twig
来源：http://hgr.aibaodan.cn

[U78] PHP：单元测试
来源：http://prv.yongpay.top

composer require --dev phpunit/phpunit
来源：http://zkf.fengsongda.top

[U79] PHP：静态分析
来源：http://bak.tian-w.cn

composer require --dev phpstan/phpstan
来源：http://ryz.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://drk.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qws.nanxuanxn.top

[U81] JS：初始化项目
来源：http://qef.gogol.net.cn

npm init -y;  npm i express
来源：http://sej.mhx1999.top

[U82] JS：package.json 脚本
来源：http://jre.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yqm.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://rhc.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nig.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://web.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://crv.zhiwuduotai.top

[U85] JS：可选链
来源：http://kqm.zhengqikj.top

a?.b?.c
来源：http://gnx.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://yoh.chenzaomai.com

a ?? b
来源：http://gvb.fehbvm.com

[U87] JS：解构默认值
来源：http://qqm.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://hxx.pycfn.com

[U88] JS：对象展开合并
来源：http://sej.tarul.cn

{ ...a, ...b }
来源：http://ogu.aibaodan.cn

[U89] JS：数组去重
来源：http://zrj.aizwys.cn

[...new Set(arr)]
来源：http://wkj.bbcook.cn

[U90] JS：数字数组排序
来源：http://hry.guannengcc.top

[...arr].sort((a, b) => a - b)
来源：http://ubj.ivvv.top

[U91] JS：对象键值遍历
来源：http://cnb.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hoy.ybcxt.top

[U92] JS：深拷贝
来源：http://gnw.zhaomingkeji.xyz

structuredClone(obj)
来源：http://tbw.ybcxt.top

[U93] JS：模板字符串
来源：http://ymg.nwbrower.top

`共 ${n} 条`
来源：http://wht.cdnleiting.top

[U94] JS：箭头函数
来源：http://gar.dianchejie.cn

const double = x => x * 2;
来源：http://ann.xuanzx.com

[U95] JS：Promise 包装
来源：http://vci.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://giq.uphjek.com

[U96] JS：async/await 与异常
来源：http://kux.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qyz.hcnkem.com

[U97] JS：并发请求
来源：http://ahu.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://acn.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://qpw.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://itr.shuidangran.top

[U99] JS：事件监听
来源：http://txg.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://qtu.ybcxt.top

[U100] JS：DOM 查询
来源：http://ije.gzhubu.top

document.querySelector(".item")
来源：http://fha.tanke756.top

[U101] JS：classList 操作
来源：http://luc.hcnkem.com

el.classList.toggle("active")
来源：http://mrn.uphjek.com

[U102] JS：本地存储
来源：http://sep.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hqn.xuanzx.com

[U103] JS：定时器
来源：http://wou.daxiang520.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lsd.jianghu66.top

[U104] JS：防抖
来源：http://ymn.jinqigufen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhg.jinqigufen.top

[U105] JS：节流
来源：http://lvg.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://izg.zhixingplan.top

[U106] JS：日期格式化
来源：http://eej.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pvj.fktsv.cn

[U107] JS：数字千分位
来源：http://xxs.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bec.shzxlz.cn

[U108] JS：随机整数
来源：http://ixs.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cjh.yueranfly.top

[U109] JS：数组分组
来源：http://bil.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://ntt.tarul.cn

[U110] JS：数组分块
来源：http://nhv.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xem.gogol.net.cn

[U111] JS：对象转 Map
来源：http://xfx.yvedp.cn

new Map(Object.entries(obj))
来源：http://gxu.shuidangran.top

[U112] JS：字符串补位
来源：http://zwl.bbcook.cn

"7".padStart(3, "0")
来源：http://mmj.ppjwa.cn

[U113] JS：正则替换全部
来源：http://bcc.haohaochexian.top

s.replaceAll("a", "b")
来源：http://tam.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://xzs.yanxiufei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lml.9152youxi.cn

[U115] JS：生成 UUID
来源：http://obo.hesvh.cn

crypto.randomUUID()
来源：http://hor.cucudq.cn

[U116] JS：类型检查（JSDoc）
来源：http://muo.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://vox.jlsjyb.cn

[U117] JS：单元测试
来源：http://xza.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://ubh.jiagoushi.top

[U118] JS：开发服务器
来源：http://jmv.jinqigufen.top

npm i -D vite;  npx vite
来源：http://osc.cashguo.top

[U119] JS：生产构建
来源：http://vyv.yonumen.top

npx vite build
来源：http://ogi.zdbjq.cn

[U120] JS：读取环境变量（Vite）
来源：http://poq.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://byy.yj20258.top

================================================================================
来源：http://jge.smart0.xyz

统计汇总
来源：http://vrc.hongshengwenyu.top

================================================================================
来源：http://dba.fktsv.cn

按语言统计（条）：
来源：http://dqi.iojbl.cn

Python ......... 252
来源：http://jqd.xingfuxueyuan.xyz

PHP ............ 252
来源：http://lev.sufxvd.cn

JavaScript ..... 252
来源：http://keq.sysykeji.top

TypeScript ..... 212
来源：http://nyr.fzhhl.top

Java ........... 212
来源：http://qyw.daria6918.cn

Go ............. 212
来源：http://unr.shangyingyoupin.top

Ruby ........... 212
来源：http://byx.vqdsnc.cn

C# ............. 212
来源：http://sxo.havefunace.top

C .............. 30
来源：http://bsx.xinyue.icu

C++ ............ 30
来源：http://eih.hywenlv.cn

SQL ............ 90
来源：http://jjn.chenlongwang.top

Bash ........... 80
来源：http://lbp.hesvh.cn

Kotlin ......... 15
来源：http://xrz.jyoumei.cn

Swift .......... 15
来源：http://awc.gogol.net.cn

Lua ............ 10
来源：http://qjf.zhongyouzk.top

Perl ........... 10
来源：http://yls.bjfxy.top

Scala .......... 10
来源：http://hnx.jinqigufen.top

------------------------------------
来源：http://erh.fktsv.cn

合计 ........... 2106 条
来源：http://una.ydjk.org.cn

按章节统计：
来源：http://akp.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lqq.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zwg.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rss.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uth.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dpo.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://elv.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nnk.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ysp.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nay.gogol.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qlj.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ynx.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://feb.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hak.c1oappe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qjr.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bhb.kuanghao11.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ggq.0kj1m.cn

Q SQL 专题                              90
来源：http://pmf.ydzc1.top

R Bash 专题                             80
来源：http://mqj.gotoacloud.top

S C / C++ 专题                          60
来源：http://egg.daria6918.cn

T 其他语言补充                          60
来源：http://ndv.pengpengdd.cyou

U 高频实用片段                         120
来源：http://wiy.zhijiandao.cn

------------------------------------
来源：http://irp.jinghuilouyu.cn

合计                                  2106 条
来源：http://nlt.fehbvm.com

--------------------------------------------------------------------------------
来源：http://koi.jinghuilouyu.cn

使用提醒
来源：http://gdg.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://bgz.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wxt.ybcxt.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tbu.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dbm.hnqzz.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xmd.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lga.shuidangran.top

—— 文件结束 ——
来源：http://sab.fengsongda.top

================================================================================
来源：http://hcy.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://xwf.daria6918.cn

Common Programming Examples Cheat Book
来源：http://cyq.mhx1999.top

================================================================================
来源：http://hfh.ybcxt.top

【收录内容】
来源：http://jbu.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ewq.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ctx.zhixingplan.top

SQL · Bash · C · C++
来源：http://zyz.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wby.jqgufenzy.top

【使用说明】
来源：http://cno.jianghu66.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tcm.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://itd.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://svz.ehwqpu.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tew.kuanghao11.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qsy.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kuc.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jwd.cqqwz.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vqa.hnqzz.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lvz.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://htz.yj20258888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rpk.sjlbkw.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://unc.ehwqpu.com

【文件统计】
来源：http://hxn.jinqigfzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pmb.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://ogb.meibo888.top

目  录
来源：http://fdi.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://fyq.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qot.dashuyun.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sxn.chenjidiqi.icu

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tew.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lrp.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lwa.zycfv.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ycl.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://grq.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://own.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xgm.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hjt.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cbu.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yyb.havefunace.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ffv.redwolf501.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://scn.haohaochexian.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mgy.52xcode.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rmk.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://iun.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://sxx.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tym.hesvh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sxi.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mfm.yuanzhike.top

================================================================================
来源：http://uro.sjlbkw.cn

A. 基础语法与类型
来源：http://ebi.ywan-chungtsiang.top

================================================================================
来源：http://fvm.redwolf501.top

[A01] Hello World
来源：http://wee.andypj.xyz

Py:   print("Hello, World!")
来源：http://wjp.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://pnr.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://deh.cdnleiting.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pnh.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://sil.yonumen.top

Go:   fmt.Println("Hello, World!")
来源：http://rap.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://qqz.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pql.cheryme.top

[A02] 变量声明与赋值
来源：http://kjs.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gca.svipenyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nhi.sysykeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://toa.vehdjk.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://suz.birdmap.top

Java: String name = "Alex"; int age = 20;
来源：http://lee.wangdashe.top

Go:   name := "Alex"; age := 20
来源：http://vpu.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://kff.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://yap.yonumen.top

[A03] 常量定义
来源：http://cxz.ctjpmb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bku.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://ztf.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://llt.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://kdp.jinqigfzy.top

Java: static final double PI = 3.14159;
来源：http://tcq.9152youxi.cn

Go:   const PI = 3.14159
来源：http://bmm.zdqjudy.top

Ruby: PI = 3.14159
来源：http://vgb.tarul.cn

C#:   const double PI = 3.14159;
来源：http://gpp.chenlongwang.top

[A04] 判断变量类型
来源：http://fqb.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xbo.aizwys.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rrr.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cml.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://mgs.iojbl.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wii.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://btv.zhiwuduotai.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kfe.shanyushiyangtech.top

C#:   x.GetType().Name; x is int
来源：http://vfg.sjlbkw.cn

[A05] 整数除法与取模
来源：http://fed.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pqe.zhijiandao.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jvt.birdmap.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://obn.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://idr.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://syj.tarul.cn

Go:   7 / 2; 7 % 2
来源：http://rfh.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://oez.xziqi.cn

C#:   7 / 2; 7 % 2
来源：http://zts.ppjwa.cn

[A06] 字符串转数字
来源：http://bhk.yj20258.top

Py:   int("42"); float("3.14")
来源：http://iaq.hysaishi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oex.cqqwz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dvy.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://oqm.316326.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wgc.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xyz.cheryme.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hmy.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xqe.fktsv.cn

[A07] 数字转字符串
来源：http://fcl.9152youxi.cn

Py:   str(42)
来源：http://niq.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://wcj.feifeiyinyue.top


<!-- 参考信息 -->