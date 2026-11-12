代发 wailian999

[U51] PHP：数组解构
来源：http://xbr.ydjk.org.cn

[$a, $b] = $arr;
来源：http://wfn.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://pbj.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://czq.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://vjw.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://lji.andypj.xyz

[U54] PHP：空安全调用
来源：http://rgs.guowangkeji.top

$obj?->method()
来源：http://aur.c1oappe.top

[U55] PHP：match 表达式
来源：http://mwb.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xah.iojbl.cn

[U56] PHP：命名参数
来源：http://dzi.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://ehd.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://rlv.nanxuanxn.top

"值: {$a}"
来源：http://mpw.yongpay.top

[U58] PHP：数组三件套
来源：http://dgd.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fvh.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://ccs.zhijiandao.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oab.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://jin.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jqk.zhongyouzk.top

[U61] PHP：正则
来源：http://bex.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vyy.jqgfzy.top

[U62] PHP：日期对象
来源：http://hbc.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://smb.cashguo.top

[U63] PHP：文件读写
来源：http://tql.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zco.sufxvd.cn

[U64] PHP：目录遍历
来源：http://zbk.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://lll.vqdsnc.cn

[U65] PHP：会话
来源：http://wcp.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://lrs.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://gnq.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://und.redwolf501.top

[U67] PHP：处理文件上传
来源：http://zow.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kav.bbcook.cn

[U68] PHP：PDO 连接
来源：http://ynm.guannengcc.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://etb.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://tzv.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bns.xziqi.cn

[U70] PHP：PDO 事务
来源：http://yhm.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pyb.cheryme.top

[U71] PHP：抛出异常
来源：http://axx.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://hek.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://tgc.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://mar.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://wze.c1oappe.top

parse_ini_file("config.ini", true)
来源：http://knx.aizwys.cn

[U74] PHP：读取环境变量
来源：http://yah.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://tbm.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://jxc.zdqjudy.top

composer require psr/container
来源：http://yld.jinqigfzy.top

[U76] PHP：简单路由
来源：http://urq.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pbj.yangfankeji.com

[U77] PHP：模板渲染
来源：http://eva.zdqjudy.top

composer require twig/twig
来源：http://yew.iojbl.cn

[U78] PHP：单元测试
来源：http://bcv.xylfe.cn

composer require --dev phpunit/phpunit
来源：http://aqy.9152youxi.cn

[U79] PHP：静态分析
来源：http://qyh.tanke756.top

composer require --dev phpstan/phpstan
来源：http://dpy.hesvh.cn

[U80] PHP：代码规范修复
来源：http://gkw.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xwk.ybcxt.top

[U81] JS：初始化项目
来源：http://nmb.sysykeji.top

npm init -y;  npm i express
来源：http://slx.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://yhc.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zeh.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://cen.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://cta.jinqigufen.top

[U84] JS：CommonJS 写法
来源：http://ubi.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oxt.cheryme.top

[U85] JS：可选链
来源：http://zpj.yj202588.top

a?.b?.c
来源：http://qxc.pengpengdd.cyou

[U86] JS：空值合并
来源：http://jld.bjfxy.top

a ?? b
来源：http://jtu.cqqwz.cn

[U87] JS：解构默认值
来源：http://eul.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://ury.svipenyu.cn

[U88] JS：对象展开合并
来源：http://grj.guannengcc.top

{ ...a, ...b }
来源：http://ojt.cqqwz.cn

[U89] JS：数组去重
来源：http://ocz.zdqjudy.top

[...new Set(arr)]
来源：http://rmk.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://xou.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://sbv.tanke756.top

[U91] JS：对象键值遍历
来源：http://dmj.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yxu.jlsjyb.cn

[U92] JS：深拷贝
来源：http://lnh.dashuyun.cn

structuredClone(obj)
来源：http://oxb.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://fci.zdqjudy.top

`共 ${n} 条`
来源：http://cpo.hesvh.cn

[U94] JS：箭头函数
来源：http://cly.snrcjt.cn

const double = x => x * 2;
来源：http://elf.yanxiufei.cn

[U95] JS：Promise 包装
来源：http://wop.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://yfm.havefunace.top

[U96] JS：async/await 与异常
来源：http://tpa.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xsw.yangfankeji.com

[U97] JS：并发请求
来源：http://vxu.vehdjk.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://uda.vehdjk.com

[U98] JS：fetch 带 JSON
来源：http://bdz.gotoacloud.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ugq.fzhhl.top

[U99] JS：事件监听
来源：http://qfi.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://mdw.tian-w.cn

[U100] JS：DOM 查询
来源：http://iju.zdqjudy.top

document.querySelector(".item")
来源：http://bir.jinqigfzy.top

[U101] JS：classList 操作
来源：http://det.zhixingplan.top

el.classList.toggle("active")
来源：http://qmk.316326.xyz

[U102] JS：本地存储
来源：http://krv.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eiw.ywan-chungtsiang.top

[U103] JS：定时器
来源：http://bpg.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zri.daria6918.cn

[U104] JS：防抖
来源：http://rzw.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bna.cdnleiting.top

[U105] JS：节流
来源：http://ryf.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jde.316326.xyz

[U106] JS：日期格式化
来源：http://ubd.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qtn.bjfxy.top

[U107] JS：数字千分位
来源：http://ked.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xln.zdqjudy.top

[U108] JS：随机整数
来源：http://xfu.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sad.pycfn.com

[U109] JS：数组分组
来源：http://frk.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://mmy.jyoumei.cn

[U110] JS：数组分块
来源：http://pvw.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hds.meibo888.top

[U111] JS：对象转 Map
来源：http://zrm.ehwqpu.com

new Map(Object.entries(obj))
来源：http://wbe.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://mlj.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://ymo.smart0.xyz

[U113] JS：正则替换全部
来源：http://csu.vehdjk.com

s.replaceAll("a", "b")
来源：http://grc.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://mgz.wangdashe.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://slv.ppjwa.cn

[U115] JS：生成 UUID
来源：http://fpo.zhiwuduotai.top

crypto.randomUUID()
来源：http://qpb.fanxiaobao.xyz

[U116] JS：类型检查（JSDoc）
来源：http://qbv.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://dfz.chenjidiqi.icu

[U117] JS：单元测试
来源：http://spn.pengpengdd.cyou

npm i -D vitest;  npx vitest
来源：http://mku.xingfuxueyuan.xyz

[U118] JS：开发服务器
来源：http://fmg.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://tlj.aizwys.cn

[U119] JS：生产构建
来源：http://dtu.yueranfly.top

npx vite build
来源：http://sud.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://sah.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://zbv.sysykeji.top

================================================================================
来源：http://jie.cucudq.cn

统计汇总
来源：http://xua.gogol.net.cn

================================================================================
来源：http://vhu.316326.xyz

按语言统计（条）：
来源：http://njn.nwbrower.top

Python ......... 252
来源：http://oqh.zhiwuduotai.top

PHP ............ 252
来源：http://zif.shzxlz.cn

JavaScript ..... 252
来源：http://vmw.mhx1999.top

TypeScript ..... 212
来源：http://fns.yuanzhike.top

Java ........... 212
来源：http://qxr.xingfuxueyuan.xyz

Go ............. 212
来源：http://vuy.dianchejie.cn

Ruby ........... 212
来源：http://ihc.yj202588.top

C# ............. 212
来源：http://jgp.jlsjyb.cn

C .............. 30
来源：http://sle.guowangkeji.top

C++ ............ 30
来源：http://jfx.nanxinkj.top

SQL ............ 90
来源：http://voq.quarkkingdee.top

Bash ........... 80
来源：http://gqb.xziqi.cn

Kotlin ......... 15
来源：http://jgr.tian-w.cn

Swift .......... 15
来源：http://fem.jqgfzy.top

Lua ............ 10
来源：http://ktn.hfpthk.cn

Perl ........... 10
来源：http://vjt.xuetiantiany.cn

Scala .......... 10
来源：http://tzp.ehwqpu.com

------------------------------------
来源：http://qbh.hysaishi.cn

合计 ........... 2106 条
来源：http://bfq.shangyingyoupin.top

按章节统计：
来源：http://zoz.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ome.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://acy.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://amk.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xzt.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fbu.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rjt.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zxh.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vsw.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qxj.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nif.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yfw.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xwb.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cqx.zhiwuduotai.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rzs.meibo888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cfd.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fhl.fzhhl.top

Q SQL 专题                              90
来源：http://qwq.fzhhl.top

R Bash 专题                             80
来源：http://yiv.sjlbkw.cn

S C / C++ 专题                          60
来源：http://zxl.zhijiandao.cn

T 其他语言补充                          60
来源：http://ajv.gotoacloud.top

U 高频实用片段                         120
来源：http://vmo.xuanzx.com

------------------------------------
来源：http://uqy.guowangkeji.top

合计                                  2106 条
来源：http://fjn.nwbrower.top

--------------------------------------------------------------------------------
来源：http://shw.cucudq.cn

使用提醒
来源：http://lry.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://gze.shuidangran.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gys.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ztl.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gbz.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lwi.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ypg.yj20258.top

—— 文件结束 ——
来源：http://jqt.epnwcf.com

================================================================================
来源：http://rsh.zdbjq.cn

程序语言常见例子速查手册（2024 版）
来源：http://vyx.birdmap.top

Common Programming Examples Cheat Book
来源：http://slz.vqdsnc.cn

================================================================================
来源：http://ewo.ehwqpu.com

【收录内容】
来源：http://cpq.xinyue.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://xsv.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cni.yvedp.cn

SQL · Bash · C · C++
来源：http://kmn.svipenyu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kky.vqdsnc.cn

【使用说明】
来源：http://vsv.fengsongda.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kor.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zzd.nanxuanxn.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hgd.zhijiandao.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nyx.feifeiyinyue.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qdo.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qev.ywan-chungtsiang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zuw.fktsv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vpw.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vye.cdnleiting.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ysi.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ilj.vqdsnc.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kbn.chenzaomai.com

【文件统计】
来源：http://abd.tanke756.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vvc.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://cmk.sysykeji.top

目  录
来源：http://fnt.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://yll.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tgh.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yoy.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ixn.yangfankeji.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dmu.cqqwz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://upv.zhongyouzk.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uyu.9152youxi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sly.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nhj.zhaomingkeji.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fxq.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oxe.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ssk.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ibp.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bys.cqqwz.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ysy.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wsb.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ywl.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qah.svipenyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yif.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zlx.cdnleiting.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lks.zhoulong.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jpp.nanxuanxn.top

================================================================================
来源：http://wus.ctjpmb.com

A. 基础语法与类型
来源：http://fnq.ywan-chungtsiang.top

================================================================================
来源：http://vlr.jyoumei.cn

[A01] Hello World
来源：http://bhm.ywan-chungtsiang.top

Py:   print("Hello, World!")
来源：http://ywf.hongshengwenyu.top

PHP:  echo "Hello, World!";
来源：http://rsv.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://ycy.chenlongwang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jjv.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://ejq.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://ikf.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://vkk.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://byj.gaohongyu789.top

[A02] 变量声明与赋值
来源：http://ben.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zkp.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://muo.hnxiangtu.top

JS:   let name = "Alex"; const age = 20;
来源：http://tqb.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kyl.vehdjk.com

Java: String name = "Alex"; int age = 20;
来源：http://nac.vqdsnc.cn

Go:   name := "Alex"; age := 20
来源：http://epd.jinqigufen.top

Ruby: name = "Alex"; age = 20
来源：http://fas.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://jqi.jyoumei.cn

[A03] 常量定义
来源：http://bcn.chenzaomai.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nrm.sufxvd.cn

PHP:  const PI = 3.14159;
来源：http://mgu.aibaodan.cn

JS:   const PI = 3.14159;
来源：http://fng.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://gul.gaohongyu789.top

Java: static final double PI = 3.14159;
来源：http://ycj.yongpay.top

Go:   const PI = 3.14159
来源：http://fsy.havefunace.top

Ruby: PI = 3.14159
来源：http://ntp.bbcook.cn

C#:   const double PI = 3.14159;
来源：http://qgm.yuanzhike.top

[A04] 判断变量类型
来源：http://gqn.nanxinkj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xuf.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ren.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zae.fengsongda.top

TS:   typeof x; x instanceof Date
来源：http://csv.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zfd.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://xin.redwolf501.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rcl.nwbrower.top

C#:   x.GetType().Name; x is int
来源：http://qyx.zhoulong.xyz

[A05] 整数除法与取模
来源：http://jug.snrcjt.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lgy.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cbj.hywenlv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://evq.daria6918.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rut.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://urs.haohaochexian.top

Go:   7 / 2; 7 % 2
来源：http://fhr.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://exq.zycfv.cn

C#:   7 / 2; 7 % 2
来源：http://xhm.yj20258888.top

[A06] 字符串转数字
来源：http://uyu.cheryme.top

Py:   int("42"); float("3.14")
来源：http://mgj.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pje.xylfe.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qda.zhaomingkeji.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://jmy.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uhj.xingfuxueyuan.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eop.zycfv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dhc.ctjpmb.com


<!-- 参考信息 -->