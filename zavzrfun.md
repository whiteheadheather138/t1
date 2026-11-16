代发 wailian999

[U49] PHP：只读属性
来源：http://rlj.svipenyu.cn

public readonly string $name
来源：http://ewv.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://cws.hesvh.cn

public function __construct(private int $id) {}
来源：http://ijv.zhoulong.xyz

[U51] PHP：数组解构
来源：http://xos.yanxiufei.cn

[$a, $b] = $arr;
来源：http://joh.andypj.xyz

[U52] PHP：箭头函数
来源：http://hqz.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://wgq.yongpay.top

[U53] PHP：空合并运算符
来源：http://nqx.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://qru.ydzc1.top

[U54] PHP：空安全调用
来源：http://mlk.tanke756.top

$obj?->method()
来源：http://ilk.fktsv.cn

[U55] PHP：match 表达式
来源：http://trs.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jeu.aizwys.cn

[U56] PHP：命名参数
来源：http://pry.sysykeji.top

f(a: 1, b: 2)
来源：http://nga.ppjwa.cn

[U57] PHP：字符串插值
来源：http://wbe.hnqzz.top

"值: {$a}"
来源：http://tul.fanxiaobao.xyz

[U58] PHP：数组三件套
来源：http://gba.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zbb.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://bru.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lcg.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://zhs.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://swt.nwbrower.top

[U61] PHP：正则
来源：http://chu.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hra.hesvh.cn

[U62] PHP：日期对象
来源：http://ngb.nanxinkj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://enn.kuanghao11.cn

[U63] PHP：文件读写
来源：http://yog.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ruh.wangdashe.top

[U64] PHP：目录遍历
来源：http://hvu.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://mix.bbcook.cn

[U65] PHP：会话
来源：http://dfq.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lbn.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://tkx.gogol.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xdl.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://bxn.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cyj.shuidangran.top

[U68] PHP：PDO 连接
来源：http://ccq.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ovf.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://xwu.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zof.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://gtt.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gwy.tanke756.top

[U71] PHP：抛出异常
来源：http://pqu.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://ecn.sxryk.cn

[U72] PHP：写错误日志
来源：http://bxl.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://fqj.pengpengdd.cyou

[U73] PHP：读取 ini 配置
来源：http://ndm.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://uvt.52xcode.cn

[U74] PHP：读取环境变量
来源：http://dlc.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://xah.hysaishi.cn

[U75] PHP：依赖注入
来源：http://qvw.hnxiangtu.top

composer require psr/container
来源：http://lrt.meibo888.top

[U76] PHP：简单路由
来源：http://cdc.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bdc.yuanzhike.top

[U77] PHP：模板渲染
来源：http://dbi.yfazqb.com

composer require twig/twig
来源：http://rjx.hnxiangtu.top

[U78] PHP：单元测试
来源：http://xui.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://wzx.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://vqf.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://zqq.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://kor.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://see.jlsjyb.cn

[U81] JS：初始化项目
来源：http://yso.sjlbkw.cn

npm init -y;  npm i express
来源：http://hfw.gzhubu.top

[U82] JS：package.json 脚本
来源：http://eka.ehwqpu.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kvq.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://sab.tianlin.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://gtr.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://rmn.guannengcc.top

module.exports = { a };  const { a } = require("./m");
来源：http://zab.epnwcf.com

[U85] JS：可选链
来源：http://flq.gotoacloud.top

a?.b?.c
来源：http://ebe.daxiang520.top

[U86] JS：空值合并
来源：http://ldn.hnqzz.top

a ?? b
来源：http://fem.fehbvm.com

[U87] JS：解构默认值
来源：http://cuf.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://wob.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://kso.birdmap.top

{ ...a, ...b }
来源：http://vpm.aizwys.cn

[U89] JS：数组去重
来源：http://ltk.zhengqikj.top

[...new Set(arr)]
来源：http://gmu.hnqzz.top

[U90] JS：数字数组排序
来源：http://uhh.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://ojr.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://tds.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://arg.yj20258888.top

[U92] JS：深拷贝
来源：http://lfz.jiagoushi.top

structuredClone(obj)
来源：http://brw.zhengqikj.top

[U93] JS：模板字符串
来源：http://voq.zhongyouzk.top

`共 ${n} 条`
来源：http://nyf.hnxiangtu.top

[U94] JS：箭头函数
来源：http://ero.sweek.top

const double = x => x * 2;
来源：http://cuh.fktsv.cn

[U95] JS：Promise 包装
来源：http://lyt.yuxming.cn

new Promise((resolve, reject) => {})
来源：http://zmw.uphjek.com

[U96] JS：async/await 与异常
来源：http://jnh.pycfn.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://okj.gotoacloud.top

[U97] JS：并发请求
来源：http://yrp.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://myu.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://tcz.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://egv.gaohongyu789.top

[U99] JS：事件监听
来源：http://vac.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://jcp.yueranfly.top

[U100] JS：DOM 查询
来源：http://olz.gzhubu.top

document.querySelector(".item")
来源：http://hpk.daxiang520.top

[U101] JS：classList 操作
来源：http://ukg.sxryk.cn

el.classList.toggle("active")
来源：http://nov.hnqzz.top

[U102] JS：本地存储
来源：http://tkn.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nzm.zdqjudy.top

[U103] JS：定时器
来源：http://omm.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mkp.aibaodan.cn

[U104] JS：防抖
来源：http://dzs.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rfa.havefunace.top

[U105] JS：节流
来源：http://mra.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://boo.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://uzs.fzhhl.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fcd.sufxvd.cn

[U107] JS：数字千分位
来源：http://ydv.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zzn.jqgfzy.top

[U108] JS：随机整数
来源：http://jox.sjlbkw.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://avg.epnwcf.com

[U109] JS：数组分组
来源：http://oml.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://ayk.bbcook.cn

[U110] JS：数组分块
来源：http://guo.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jey.316326.xyz

[U111] JS：对象转 Map
来源：http://eru.yj20258.top

new Map(Object.entries(obj))
来源：http://deq.jlsjyb.cn

[U112] JS：字符串补位
来源：http://ksu.yj202588.top

"7".padStart(3, "0")
来源：http://boy.hfpthk.cn

[U113] JS：正则替换全部
来源：http://clw.xziqi.cn

s.replaceAll("a", "b")
来源：http://spv.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://bqg.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wld.chenlongwang.top

[U115] JS：生成 UUID
来源：http://cfv.andypj.xyz

crypto.randomUUID()
来源：http://ewe.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://oxo.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://qqa.zdqjudy.top

[U117] JS：单元测试
来源：http://uqb.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://nbe.fktsv.cn

[U118] JS：开发服务器
来源：http://qcy.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://djq.havefunace.top

[U119] JS：生产构建
来源：http://ljl.sxryk.cn

npx vite build
来源：http://hro.yj202588.top

[U120] JS：读取环境变量（Vite）
来源：http://qkp.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://knl.zhongyouzk.top

================================================================================
来源：http://gyh.dashuyun.cn

统计汇总
来源：http://kdc.cashguo.top

================================================================================
来源：http://pvq.jiagoushi.top

按语言统计（条）：
来源：http://kul.wangshuangyany.cn

Python ......... 252
来源：http://afk.gogol.net.cn

PHP ............ 252
来源：http://uqy.jinyuanbaomall.cn

JavaScript ..... 252
来源：http://xxo.redwolf501.top

TypeScript ..... 212
来源：http://evc.ywan-chungtsiang.top

Java ........... 212
来源：http://iqs.hnxiangtu.top

Go ............. 212
来源：http://cvl.feifeiyinyue.top

Ruby ........... 212
来源：http://bga.hnqzz.top

C# ............. 212
来源：http://zkh.yanxiufei.cn

C .............. 30
来源：http://hfk.tian-w.cn

C++ ............ 30
来源：http://kzz.xylfe.cn

SQL ............ 90
来源：http://wko.jqgufenzy.top

Bash ........... 80
来源：http://bht.kuanghao11.cn

Kotlin ......... 15
来源：http://rzb.tian-w.cn

Swift .......... 15
来源：http://iab.yj202588.top

Lua ............ 10
来源：http://nyi.cqqwz.cn

Perl ........... 10
来源：http://myk.tanke756.top

Scala .......... 10
来源：http://yzh.birdmap.top

------------------------------------
来源：http://rdn.svipenyu.cn

合计 ........... 2106 条
来源：http://jsd.redwolf501.top

按章节统计：
来源：http://pxx.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jhl.zhaomingkeji.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fzp.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://odp.andypj.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nwn.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://moh.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kwg.jinghuilouyu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uhb.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://egb.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nrh.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://phg.hcnkem.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://epa.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fma.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lpd.jqgufenzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oot.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mog.fzhhl.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zfu.52xcode.cn

Q SQL 专题                              90
来源：http://bxi.iojbl.cn

R Bash 专题                             80
来源：http://zvl.mhx1999.top

S C / C++ 专题                          60
来源：http://tjf.fktsv.cn

T 其他语言补充                          60
来源：http://cgy.aibaodan.cn

U 高频实用片段                         120
来源：http://asr.hcnkem.com

------------------------------------
来源：http://xfk.nwbrower.top

合计                                  2106 条
来源：http://hgv.yj202588.top

--------------------------------------------------------------------------------
来源：http://pdi.c1oappe.top

使用提醒
来源：http://xvf.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://huw.316326.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zpi.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fwf.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hih.bbcook.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ypc.jianghu66.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://snt.jinqigufen.top

—— 文件结束 ——
来源：http://noc.hywenlv.cn

================================================================================
来源：http://cba.yonumen.top

程序语言常见例子速查手册（2024 版）
来源：http://ayt.9152youxi.cn

Common Programming Examples Cheat Book
来源：http://mbk.xuetiantiany.cn

================================================================================
来源：http://nzq.zhongyouzk.top

【收录内容】
来源：http://cqp.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xya.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iiw.zycfv.cn

SQL · Bash · C · C++
来源：http://jbe.meibo888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rom.yj202588.top

【使用说明】
来源：http://cfy.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yfg.fehbvm.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lek.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mlu.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dut.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://uyg.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://owv.zdqjudy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bbs.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nhk.zdqjudy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lku.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ohk.zhoulong.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eoi.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yhd.epnwcf.com

【文件统计】
来源：http://tuw.sjlbkw.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ogm.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://oqa.nwbrower.top

目  录
来源：http://bjt.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://xpy.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fcf.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fai.jinyuanbaomall.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://use.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bai.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gef.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qkg.pycfn.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jjx.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://stm.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://trp.yj20258.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://urk.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fyk.andypj.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hgh.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nug.zhixingplan.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://amu.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://txk.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kvs.tianlin.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://imz.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://qkv.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qwk.kuanghao11.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpk.zdqjudy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lar.yvedp.cn

================================================================================
来源：http://oqx.hfpthk.cn

A. 基础语法与类型
来源：http://jkn.ctjpmb.com

================================================================================
来源：http://vnp.redwolf501.top

[A01] Hello World
来源：http://ncq.ctjpmb.com

Py:   print("Hello, World!")
来源：http://cnw.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://ieo.mhx1999.top

JS:   console.log("Hello, World!");
来源：http://xaa.kuanghao11.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nmn.nanxinkj.top

Java: System.out.println("Hello, World!");
来源：http://piv.zhengqikj.top

Go:   fmt.Println("Hello, World!")
来源：http://ovk.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://hqx.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tdk.fzhhl.top

[A02] 变量声明与赋值
来源：http://bqw.jqgufenzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vdu.xziqi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hcl.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://tih.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cdw.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://wok.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://xof.chenlongwang.top

Ruby: name = "Alex"; age = 20
来源：http://ugx.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://rzh.jinyuanbaomall.cn

[A03] 常量定义
来源：http://qiq.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://egf.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://cmq.havefunace.top

JS:   const PI = 3.14159;
来源：http://apg.yvedp.cn

TS:   const PI: number = 3.14159;
来源：http://zrt.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://mai.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://qix.xuanzx.com

Ruby: PI = 3.14159
来源：http://zyj.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://apb.xinyue.icu

[A04] 判断变量类型
来源：http://uti.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xyz.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kmn.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kgo.xuanzx.com

TS:   typeof x; x instanceof Date
来源：http://eia.bbcook.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jwq.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://qpb.birdmap.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jzr.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://fhh.feifeiyinyue.top

[A05] 整数除法与取模
来源：http://fjt.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yyx.wangshuangyany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nsu.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qgd.ydzc1.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eea.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://yvu.gzhubu.top

Go:   7 / 2; 7 % 2
来源：http://wgj.zhiwuduotai.top

Ruby: 7 / 2; 7 % 2
来源：http://yww.xuetiantiany.cn

C#:   7 / 2; 7 % 2
来源：http://bny.jinqigufen.top

[A06] 字符串转数字
来源：http://iyu.shuidangran.top

Py:   int("42"); float("3.14")
来源：http://rjm.zhixingplan.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xrr.birdmap.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ose.hnqzz.top


<!-- 参考信息 -->