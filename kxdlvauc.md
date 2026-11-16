代发 wailian999

[U53] PHP：空合并运算符
来源：http://ans.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://pth.zdqjudy.top

[U54] PHP：空安全调用
来源：http://prt.yuxming.cn

$obj?->method()
来源：http://cns.tianlin.xyz

[U55] PHP：match 表达式
来源：http://zwd.kuanghao11.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zjd.sxryk.cn

[U56] PHP：命名参数
来源：http://lwr.gotoacloud.top

f(a: 1, b: 2)
来源：http://hrh.guannengcc.top

[U57] PHP：字符串插值
来源：http://bei.dianchejie.cn

"值: {$a}"
来源：http://jrq.aibaodan.cn

[U58] PHP：数组三件套
来源：http://ula.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fmw.nanxinkj.top

[U59] PHP：自定义排序
来源：http://cfq.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iwa.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://gyw.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nbk.jianghu66.top

[U61] PHP：正则
来源：http://knz.guowangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fns.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://bkt.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://srz.ydjk.org.cn

[U63] PHP：文件读写
来源：http://vgm.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://klz.52xcode.cn

[U64] PHP：目录遍历
来源：http://zpj.andypj.xyz

glob("dir/*.php");  scandir("dir");
来源：http://amw.xuetiantiany.cn

[U65] PHP：会话
来源：http://yzz.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hvh.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://xnv.kuanghao11.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ovp.sxryk.cn

[U67] PHP：处理文件上传
来源：http://wqy.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://frm.316326.xyz

[U68] PHP：PDO 连接
来源：http://jod.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sjk.jiagoushi.top

[U69] PHP：PDO 预处理
来源：http://fuw.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nok.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://khk.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fgx.gzhubu.top

[U71] PHP：抛出异常
来源：http://ril.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://sko.cucudq.cn

[U72] PHP：写错误日志
来源：http://ubn.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://yns.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://jhw.tianlin.xyz

parse_ini_file("config.ini", true)
来源：http://avs.hesvh.cn

[U74] PHP：读取环境变量
来源：http://wmp.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://nad.xziqi.cn

[U75] PHP：依赖注入
来源：http://gmr.pycfn.com

composer require psr/container
来源：http://ytq.chenzaomai.com

[U76] PHP：简单路由
来源：http://djb.epnwcf.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zew.jinqigufen.top

[U77] PHP：模板渲染
来源：http://gvw.tian-w.cn

composer require twig/twig
来源：http://eqx.yanxiufei.cn

[U78] PHP：单元测试
来源：http://lmj.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://rdm.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://mis.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://tlo.bbcook.cn

[U80] PHP：代码规范修复
来源：http://gok.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dix.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://roo.hysaishi.cn

npm init -y;  npm i express
来源：http://ohc.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://chw.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://inw.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://nyj.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xzk.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://dcl.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://ddz.cheryme.top

[U85] JS：可选链
来源：http://bgj.cheryme.top

a?.b?.c
来源：http://ozt.ydzc1.top

[U86] JS：空值合并
来源：http://usm.gaohongyu789.top

a ?? b
来源：http://mmq.ctjpmb.com

[U87] JS：解构默认值
来源：http://ycm.smart0.xyz

const { a = 1, b = 2 } = obj;
来源：http://elq.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://tse.hcnkem.com

{ ...a, ...b }
来源：http://pqe.shuidangran.top

[U89] JS：数组去重
来源：http://cmf.pengpengdd.cyou

[...new Set(arr)]
来源：http://gqs.epnwcf.com

[U90] JS：数字数组排序
来源：http://pzs.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://tqc.aizwys.cn

[U91] JS：对象键值遍历
来源：http://sml.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xmo.andypj.xyz

[U92] JS：深拷贝
来源：http://jqa.wangshuangyany.cn

structuredClone(obj)
来源：http://sca.jianghu66.top

[U93] JS：模板字符串
来源：http://yll.ivvv.top

`共 ${n} 条`
来源：http://nkr.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://qpq.shzxlz.cn

const double = x => x * 2;
来源：http://lyv.fanxiaobao.xyz

[U95] JS：Promise 包装
来源：http://nnu.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://jvw.wangdashe.top

[U96] JS：async/await 与异常
来源：http://ryh.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dxt.zhiwuduotai.top

[U97] JS：并发请求
来源：http://ooj.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://djp.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://wxk.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxu.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://hxt.tarul.cn

el.addEventListener("click", e => {})
来源：http://udh.hammf.cn

[U100] JS：DOM 查询
来源：http://rfy.havefunace.top

document.querySelector(".item")
来源：http://nid.c1oappe.top

[U101] JS：classList 操作
来源：http://iol.jianghu66.top

el.classList.toggle("active")
来源：http://esz.xuetiantiany.cn

[U102] JS：本地存储
来源：http://ptq.shangyingyoupin.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ipw.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://ypk.tarul.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mhr.chenzaomai.com

[U104] JS：防抖
来源：http://afp.yonumen.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://noq.meibo888.top

[U105] JS：节流
来源：http://bqr.birdmap.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bey.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://umd.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eex.svipenyu.cn

[U107] JS：数字千分位
来源：http://ljc.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nky.zycfv.cn

[U108] JS：随机整数
来源：http://yhd.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://raz.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://dmp.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://spo.9152youxi.cn

[U110] JS：数组分块
来源：http://wqw.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ovq.hcnkem.com

[U111] JS：对象转 Map
来源：http://ssh.vehdjk.com

new Map(Object.entries(obj))
来源：http://acx.0kj1m.cn

[U112] JS：字符串补位
来源：http://isl.iojbl.cn

"7".padStart(3, "0")
来源：http://inw.9152youxi.cn

[U113] JS：正则替换全部
来源：http://was.yj202588.top

s.replaceAll("a", "b")
来源：http://aru.ydzc1.top

[U114] JS：JSON 深比较
来源：http://bfe.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://wsv.sysykeji.top

[U115] JS：生成 UUID
来源：http://qmr.haohaochexian.top

crypto.randomUUID()
来源：http://yuy.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://sto.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://qvg.tian-w.cn

[U117] JS：单元测试
来源：http://ldy.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://nqg.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://mbq.zdqjudy.top

npm i -D vite;  npx vite
来源：http://ncd.chenjidiqi.icu

[U119] JS：生产构建
来源：http://cnu.316326.xyz

npx vite build
来源：http://tkr.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://hug.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://gkv.xylfe.cn

================================================================================
来源：http://voa.daria6918.cn

统计汇总
来源：http://txz.chenzaomai.com

================================================================================
来源：http://jdw.zhijiandao.cn

按语言统计（条）：
来源：http://vwa.mhx1999.top

Python ......... 252
来源：http://kzj.jqgfzy.top

PHP ............ 252
来源：http://kyq.wangshuangyany.cn

JavaScript ..... 252
来源：http://ggx.hnxiangtu.top

TypeScript ..... 212
来源：http://awy.shanyushiyangtech.top

Java ........... 212
来源：http://duv.hnxiangtu.top

Go ............. 212
来源：http://oek.svipenyu.cn

Ruby ........... 212
来源：http://eru.vehdjk.com

C# ............. 212
来源：http://jsw.dianchejie.cn

C .............. 30
来源：http://qio.jqgufenzy.top

C++ ............ 30
来源：http://qrq.smart0.xyz

SQL ............ 90
来源：http://exd.bjfxy.top

Bash ........... 80
来源：http://axh.hysaishi.cn

Kotlin ......... 15
来源：http://jlb.chenzaomai.com

Swift .......... 15
来源：http://mio.ywan-chungtsiang.top

Lua ............ 10
来源：http://qiy.zycfv.cn

Perl ........... 10
来源：http://muk.sufxvd.cn

Scala .......... 10
来源：http://wad.hcnkem.com

------------------------------------
来源：http://zjx.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://giz.zhengqikj.top

按章节统计：
来源：http://rly.jinqigfzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jfx.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aud.vqdsnc.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://frf.ybcxt.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ris.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mek.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jgv.nanxuanxn.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://quq.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vzr.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uxt.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zrg.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rvb.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vvj.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ykr.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fbz.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pqh.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nqv.xuanzx.com

Q SQL 专题                              90
来源：http://alx.ydjk.org.cn

R Bash 专题                             80
来源：http://yei.mhx1999.top

S C / C++ 专题                          60
来源：http://ncr.gzhubu.top

T 其他语言补充                          60
来源：http://prn.tianlin.xyz

U 高频实用片段                         120
来源：http://tab.iojbl.cn

------------------------------------
来源：http://rnn.9152youxi.cn

合计                                  2106 条
来源：http://mgk.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://pxs.gotoacloud.top

使用提醒
来源：http://gvy.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://scw.yonumen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dau.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qco.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bhi.dashuyun.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pxc.cdnleiting.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vej.pycfn.com

—— 文件结束 ——
来源：http://qmt.fehbvm.com

================================================================================
来源：http://xlh.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://uea.jyoumei.cn

Common Programming Examples Cheat Book
来源：http://lro.hammf.cn

================================================================================
来源：http://cze.cucudq.cn

【收录内容】
来源：http://gbj.jianghu66.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ego.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jxd.guannengcc.top

SQL · Bash · C · C++
来源：http://ngq.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zbk.xylfe.cn

【使用说明】
来源：http://qfo.zhoulong.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mdt.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dsp.zhongyouzk.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zva.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tdf.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://iua.vqdsnc.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://omq.meibo888.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oxd.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yfu.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zvk.ppjwa.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rqq.jinqigufen.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://snx.iojbl.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qif.chenlongwang.top

【文件统计】
来源：http://uyc.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zom.redwolf501.top

--------------------------------------------------------------------------------
来源：http://nrq.ydjk.org.cn

目  录
来源：http://fpt.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://llg.yanxiufei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fod.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ity.mhx1999.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://agv.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ybl.shangyingyoupin.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jmv.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wsj.gogol.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bmb.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iqj.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yfz.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://utz.sufxvd.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gjo.sxryk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://evf.jianghu66.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zsk.jqgfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rvu.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ogx.cdnleiting.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xej.yuanzhike.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cvl.pycfn.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://gak.yj20258.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mqh.yj20258888.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://abj.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sxg.jinqigufen.top

================================================================================
来源：http://wdu.yvedp.cn

A. 基础语法与类型
来源：http://mwj.shangyingyoupin.top

================================================================================
来源：http://rlr.xinyue.icu

[A01] Hello World
来源：http://ckk.tarul.cn

Py:   print("Hello, World!")
来源：http://qet.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://bzx.ydjk.org.cn

JS:   console.log("Hello, World!");
来源：http://inc.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qep.xingfuxueyuan.xyz

Java: System.out.println("Hello, World!");
来源：http://yvh.sweek.top

Go:   fmt.Println("Hello, World!")
来源：http://epo.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://cih.redwolf501.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ggb.iojbl.cn

[A02] 变量声明与赋值
来源：http://lgo.xingfuxueyuan.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yoq.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://iuv.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://doh.jinyuanbaomall.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://czv.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://exm.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://juu.cashguo.top

Ruby: name = "Alex"; age = 20
来源：http://ajw.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://pxd.zhongyouzk.top

[A03] 常量定义
来源：http://qyz.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://smt.fktsv.cn

PHP:  const PI = 3.14159;
来源：http://ycp.tanke756.top

JS:   const PI = 3.14159;
来源：http://vns.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://wcx.sufxvd.cn

Java: static final double PI = 3.14159;
来源：http://afr.cucudq.cn

Go:   const PI = 3.14159
来源：http://xvd.yongpay.top

Ruby: PI = 3.14159
来源：http://prk.ywan-chungtsiang.top

C#:   const double PI = 3.14159;
来源：http://jzs.haohaochexian.top

[A04] 判断变量类型
来源：http://jmd.yfazqb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://wsp.chenlongwang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zph.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qze.jlsjyb.cn

TS:   typeof x; x instanceof Date
来源：http://nbm.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cik.xingfuxueyuan.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://fun.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ryp.xinyue.icu

C#:   x.GetType().Name; x is int
来源：http://kkp.pengpengdd.cyou

[A05] 整数除法与取模
来源：http://zlo.svipenyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jaq.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://sod.hnqzz.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lsx.shuidangran.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tac.aibaodan.cn

Java: 7 / 2; 7 % 2
来源：http://dal.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://lma.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://uie.yj20258888.top

C#:   7 / 2; 7 % 2
来源：http://anh.yj20258888.top

[A06] 字符串转数字
来源：http://kxr.nanxuanxn.top

Py:   int("42"); float("3.14")
来源：http://xvg.yfazqb.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ozl.yj202588.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wjd.yvedp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pkt.fzhhl.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ttx.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ewd.feifeiyinyue.top

Ruby: "42".to_i; "3.14".to_f
来源：http://igt.jlsjyb.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fpt.sxryk.cn

[A07] 数字转字符串
来源：http://nus.c1oappe.top

Py:   str(42)
来源：http://dqy.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://dyb.birdmap.top


<!-- 参考信息 -->