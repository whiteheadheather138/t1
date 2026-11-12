代发 wailian999

[U55] PHP：match 表达式
来源：http://bbs.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ewx.sufxvd.cn

[U56] PHP：命名参数
来源：http://inr.xziqi.cn

f(a: 1, b: 2)
来源：http://hcv.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://dlh.hysaishi.cn

"值: {$a}"
来源：http://wpr.shuidangran.top

[U58] PHP：数组三件套
来源：http://pbm.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ege.jqgfzy.top

[U59] PHP：自定义排序
来源：http://vbx.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://obf.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://nxy.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ejx.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://gdu.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iuj.jyoumei.cn

[U62] PHP：日期对象
来源：http://bxh.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zjl.nanxuanxn.top

[U63] PHP：文件读写
来源：http://xbp.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wjm.jyoumei.cn

[U64] PHP：目录遍历
来源：http://qho.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://yij.redwolf501.top

[U65] PHP：会话
来源：http://ftu.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kva.fengsongda.top

[U66] PHP：设置 Cookie
来源：http://mkb.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gof.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://azt.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tbk.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://cra.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uxg.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://fej.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jaq.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://bls.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rgy.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://fwi.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://gkl.haohaochexian.top

[U72] PHP：写错误日志
来源：http://yas.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://utv.nanxinkj.top

[U73] PHP：读取 ini 配置
来源：http://ixp.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://niv.vehdjk.com

[U74] PHP：读取环境变量
来源：http://nqo.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://pgt.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://kzz.hesvh.cn

composer require psr/container
来源：http://qhj.ywan-chungtsiang.top

[U76] PHP：简单路由
来源：http://bhz.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yzp.dianchejie.cn

[U77] PHP：模板渲染
来源：http://bbg.shangyingyoupin.top

composer require twig/twig
来源：http://uwa.9152youxi.cn

[U78] PHP：单元测试
来源：http://wkx.havefunace.top

composer require --dev phpunit/phpunit
来源：http://rxe.ctjpmb.com

[U79] PHP：静态分析
来源：http://orr.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://jmq.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://jng.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ovj.yvedp.cn

[U81] JS：初始化项目
来源：http://sne.yj20258888.top

npm init -y;  npm i express
来源：http://njj.fktsv.cn

[U82] JS：package.json 脚本
来源：http://uwx.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nxj.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://vza.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://emh.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://zct.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://kbm.guowangkeji.top

[U85] JS：可选链
来源：http://fcx.feifeiyinyue.top

a?.b?.c
来源：http://mxr.hongshengwenyu.top

[U86] JS：空值合并
来源：http://jbd.shanyushiyangkeji.top

a ?? b
来源：http://hus.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://sln.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://mzy.iojbl.cn

[U88] JS：对象展开合并
来源：http://omj.aibaodan.cn

{ ...a, ...b }
来源：http://vwp.nwbrower.top

[U89] JS：数组去重
来源：http://ssf.jianghu66.top

[...new Set(arr)]
来源：http://bla.shuidangran.top

[U90] JS：数字数组排序
来源：http://abx.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://jcr.fengsongda.top

[U91] JS：对象键值遍历
来源：http://smf.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mnb.c1oappe.top

[U92] JS：深拷贝
来源：http://egw.jqgufenzy.top

structuredClone(obj)
来源：http://pkj.ppjwa.cn

[U93] JS：模板字符串
来源：http://rtb.feifeiyinyue.top

`共 ${n} 条`
来源：http://mkk.jiagoushi.top

[U94] JS：箭头函数
来源：http://wan.yonumen.top

const double = x => x * 2;
来源：http://igt.tarul.cn

[U95] JS：Promise 包装
来源：http://uai.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://ltk.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://vxp.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://deg.jinqigfzy.top

[U97] JS：并发请求
来源：http://sjg.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bsx.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://ira.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cpy.chenzaomai.com

[U99] JS：事件监听
来源：http://rmf.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://tjs.hesvh.cn

[U100] JS：DOM 查询
来源：http://fmv.sufxvd.cn

document.querySelector(".item")
来源：http://dsf.xinyue.icu

[U101] JS：classList 操作
来源：http://iqw.guannengcc.top

el.classList.toggle("active")
来源：http://kjf.fzhhl.top

[U102] JS：本地存储
来源：http://bop.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pzg.shuidangran.top

[U103] JS：定时器
来源：http://rnb.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rmh.0kj1m.cn

[U104] JS：防抖
来源：http://gwh.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oct.52xcode.cn

[U105] JS：节流
来源：http://tks.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pov.vqdsnc.cn

[U106] JS：日期格式化
来源：http://hzh.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ntr.pengpengdd.cyou

[U107] JS：数字千分位
来源：http://gwz.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vdx.zdbjq.cn

[U108] JS：随机整数
来源：http://kam.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xfs.meibo888.top

[U109] JS：数组分组
来源：http://ghq.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://rlr.shangyingyoupin.top

[U110] JS：数组分块
来源：http://ddz.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wir.fktsv.cn

[U111] JS：对象转 Map
来源：http://nnx.shuidangran.top

new Map(Object.entries(obj))
来源：http://pmg.jinqigfzy.top

[U112] JS：字符串补位
来源：http://dfo.zhoulong.xyz

"7".padStart(3, "0")
来源：http://oyk.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://sld.jyoumei.cn

s.replaceAll("a", "b")
来源：http://tfy.aizwys.cn

[U114] JS：JSON 深比较
来源：http://phn.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vfp.chenzaomai.com

[U115] JS：生成 UUID
来源：http://olb.ctjpmb.com

crypto.randomUUID()
来源：http://eux.ctjpmb.com

[U116] JS：类型检查（JSDoc）
来源：http://mjg.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://rga.zhengqikj.top

[U117] JS：单元测试
来源：http://dys.tian-w.cn

npm i -D vitest;  npx vitest
来源：http://ryo.zdbjq.cn

[U118] JS：开发服务器
来源：http://cat.svipenyu.cn

npm i -D vite;  npx vite
来源：http://zcy.yj20258.top

[U119] JS：生产构建
来源：http://tmq.shanyushiyangkeji.top

npx vite build
来源：http://xng.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://ohq.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://vqc.jinqigfzy.top

================================================================================
来源：http://cer.9152youxi.cn

统计汇总
来源：http://mpt.shangyingyoupin.top

================================================================================
来源：http://fqh.zhaomingkeji.xyz

按语言统计（条）：
来源：http://zao.cqqwz.cn

Python ......... 252
来源：http://aur.pycfn.com

PHP ............ 252
来源：http://dvg.fengsongda.top

JavaScript ..... 252
来源：http://yed.andypj.xyz

TypeScript ..... 212
来源：http://guw.xuanzx.com

Java ........... 212
来源：http://rom.c1oappe.top

Go ............. 212
来源：http://uhu.xylfe.cn

Ruby ........... 212
来源：http://ciw.xinyue.icu

C# ............. 212
来源：http://rjd.jyoumei.cn

C .............. 30
来源：http://sqb.yueranfly.top

C++ ............ 30
来源：http://wvt.snrcjt.cn

SQL ............ 90
来源：http://hkk.cashguo.top

Bash ........... 80
来源：http://ymi.zhaomingkeji.xyz

Kotlin ......... 15
来源：http://wzt.jinqigfzy.top

Swift .......... 15
来源：http://mpa.chenjidiqi.icu

Lua ............ 10
来源：http://srj.sweek.top

Perl ........... 10
来源：http://pji.cucudq.cn

Scala .......... 10
来源：http://qcp.guowangkeji.top

------------------------------------
来源：http://efi.zhijiandao.cn

合计 ........... 2106 条
来源：http://jam.9152youxi.cn

按章节统计：
来源：http://qjq.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lla.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sqm.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vif.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kiz.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kub.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zwk.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zpf.redwolf501.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hcc.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cnj.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rgn.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uwf.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://apz.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hph.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bcq.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cab.fengsongda.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xrg.shuidangran.top

Q SQL 专题                              90
来源：http://aiu.c1oappe.top

R Bash 专题                             80
来源：http://jbu.andypj.xyz

S C / C++ 专题                          60
来源：http://jqh.hongshengwenyu.top

T 其他语言补充                          60
来源：http://tab.zhongyouzk.top

U 高频实用片段                         120
来源：http://uzi.dianchejie.cn

------------------------------------
来源：http://jnw.vqdsnc.cn

合计                                  2106 条
来源：http://fth.yj20258.top

--------------------------------------------------------------------------------
来源：http://grk.zhijiandao.cn

使用提醒
来源：http://tcq.cucudq.cn

--------------------------------------------------------------------------------
来源：http://tng.0kj1m.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fxc.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zxp.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xpm.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://cgy.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ywh.uphjek.com

—— 文件结束 ——
来源：http://aui.jlsjyb.cn

================================================================================
来源：http://efy.zhijiandao.cn

程序语言常见例子速查手册（2024 版）
来源：http://yfj.ybcxt.top

Common Programming Examples Cheat Book
来源：http://avw.yvedp.cn

================================================================================
来源：http://hxj.yvedp.cn

【收录内容】
来源：http://kbb.jyoumei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bwu.cashguo.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cxw.nwbrower.top

SQL · Bash · C · C++
来源：http://qtz.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sro.jiagoushi.top

【使用说明】
来源：http://xaa.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rme.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rlq.cheryme.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fec.yueranfly.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qkr.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://krt.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mzu.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wcv.ehwqpu.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://enz.xuanzx.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nod.yj20258888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wma.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yqu.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rfi.fanxiaobao.xyz

【文件统计】
来源：http://wnb.zycfv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qtq.epnwcf.com

--------------------------------------------------------------------------------
来源：http://fxp.cashguo.top

目  录
来源：http://bzt.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://guu.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bhm.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://paj.dashuyun.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://myv.aizwys.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bjt.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uan.shangyingyoupin.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://efw.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qwa.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tci.zhiwuduotai.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://unm.zdqjudy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vwn.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gye.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xhx.nanxinkj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cav.c1oappe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wug.tarul.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hyc.chenzaomai.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dex.c1oappe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ran.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mal.zhongyouzk.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xxr.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gza.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dkq.zhaomingkeji.xyz

================================================================================
来源：http://csi.dashuyun.cn

A. 基础语法与类型
来源：http://qfd.jiagoushi.top

================================================================================
来源：http://frh.haohaochexian.top

[A01] Hello World
来源：http://udd.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://mpl.yanxiufei.cn

PHP:  echo "Hello, World!";
来源：http://gpi.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://fji.9152youxi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ngp.dashuyun.cn

Java: System.out.println("Hello, World!");
来源：http://xun.cheryme.top

Go:   fmt.Println("Hello, World!")
来源：http://guy.mhx1999.top

Ruby: puts "Hello, World!"
来源：http://iwm.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jle.havefunace.top

[A02] 变量声明与赋值
来源：http://khm.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jbl.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ftn.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://nbs.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rsl.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://lpo.chenzaomai.com

Go:   name := "Alex"; age := 20
来源：http://uxm.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://qle.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://ehl.yueranfly.top

[A03] 常量定义
来源：http://mnp.fengsongda.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mvr.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://pdi.yueranfly.top

JS:   const PI = 3.14159;
来源：http://joq.zhaomingkeji.xyz

TS:   const PI: number = 3.14159;
来源：http://red.aibaodan.cn

Java: static final double PI = 3.14159;
来源：http://thr.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://aqw.daxiang520.top

Ruby: PI = 3.14159
来源：http://wau.xinyue.icu

C#:   const double PI = 3.14159;
来源：http://xvn.cucudq.cn

[A04] 判断变量类型
来源：http://gth.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hpd.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jdc.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cft.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://ked.gotoacloud.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nqk.316326.xyz

Go:   reflect.TypeOf(x).Name()
来源：http://oiu.jinghuilouyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mbs.andypj.xyz

C#:   x.GetType().Name; x is int
来源：http://gfp.cucudq.cn

[A05] 整数除法与取模
来源：http://uou.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://whu.pycfn.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://zrk.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qnf.fengsongda.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fyg.xinyue.icu

Java: 7 / 2; 7 % 2
来源：http://hro.hongshengwenyu.top

Go:   7 / 2; 7 % 2
来源：http://ugd.yongpay.top

Ruby: 7 / 2; 7 % 2
来源：http://tmy.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://utv.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://ymj.ydzc1.top

Py:   int("42"); float("3.14")
来源：http://ktd.shanyushiyangtech.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bjg.epnwcf.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kjc.hcnkem.com

TS:   parseInt("42", 10); Number("42")
来源：http://dyl.xuetiantiany.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cdx.yanxiufei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bat.c1oappe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nnc.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kus.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://xif.hywenlv.cn

Py:   str(42)
来源：http://sgh.daria6918.cn

PHP:  (string) 42; strval(42)
来源：http://joe.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://iso.haohaochexian.top

TS:   String(42)
来源：http://hyp.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rib.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://ijt.bjfxy.top


<!-- 参考信息 -->