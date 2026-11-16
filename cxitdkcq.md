代发 wailian999

[U47] PHP：联合类型
来源：http://fpz.ivvv.top

int|string $id
来源：http://zgp.ehwqpu.com

[U48] PHP：纯枚举
来源：http://xul.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lnl.wangdashe.top

[U49] PHP：只读属性
来源：http://pls.yanxiufei.cn

public readonly string $name
来源：http://mro.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://lvm.gotoacloud.top

public function __construct(private int $id) {}
来源：http://edi.jqgfzy.top

[U51] PHP：数组解构
来源：http://hgr.tian-w.cn

[$a, $b] = $arr;
来源：http://hjz.vehdjk.com

[U52] PHP：箭头函数
来源：http://sbf.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://gmx.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://qdy.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://qyi.birdmap.top

[U54] PHP：空安全调用
来源：http://tlf.yuanzhike.top

$obj?->method()
来源：http://aug.iojbl.cn

[U55] PHP：match 表达式
来源：http://dks.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nxn.fktsv.cn

[U56] PHP：命名参数
来源：http://ozw.yangfankeji.com

f(a: 1, b: 2)
来源：http://tuh.svipenyu.cn

[U57] PHP：字符串插值
来源：http://kqu.meibo888.top

"值: {$a}"
来源：http://xsr.yonumen.top

[U58] PHP：数组三件套
来源：http://lad.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jxe.iojbl.cn

[U59] PHP：自定义排序
来源：http://vml.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dtg.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://hur.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cyg.guannengcc.top

[U61] PHP：正则
来源：http://ycf.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kqb.shuidangran.top

[U62] PHP：日期对象
来源：http://dlx.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wxw.yj20258.top

[U63] PHP：文件读写
来源：http://sij.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dpj.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://fpb.xinyue.icu

glob("dir/*.php");  scandir("dir");
来源：http://vgt.xziqi.cn

[U65] PHP：会话
来源：http://add.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rpt.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://cvm.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jet.guannengcc.top

[U67] PHP：处理文件上传
来源：http://nfz.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jxi.c1oappe.top

[U68] PHP：PDO 连接
来源：http://afv.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://evr.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://ees.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kyr.havefunace.top

[U70] PHP：PDO 事务
来源：http://ajn.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vfs.ctjpmb.com

[U71] PHP：抛出异常
来源：http://wes.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://qqm.svipenyu.cn

[U72] PHP：写错误日志
来源：http://cpl.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://uxu.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://xnz.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://ujo.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://puc.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://mjg.ybcxt.top

[U75] PHP：依赖注入
来源：http://zkv.xuanzx.com

composer require psr/container
来源：http://hqp.cdnleiting.top

[U76] PHP：简单路由
来源：http://ipy.sxryk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ebf.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://qqf.jqgufenzy.top

composer require twig/twig
来源：http://eay.cucudq.cn

[U78] PHP：单元测试
来源：http://sex.hongshengwenyu.top

composer require --dev phpunit/phpunit
来源：http://mgf.hesvh.cn

[U79] PHP：静态分析
来源：http://pmf.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://mxp.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://wjv.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vlg.yuxming.cn

[U81] JS：初始化项目
来源：http://sat.birdmap.top

npm init -y;  npm i express
来源：http://aam.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://djn.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://svr.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://lzt.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oux.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://qpy.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jji.haohaochexian.top

[U85] JS：可选链
来源：http://bgc.shangyingyoupin.top

a?.b?.c
来源：http://ygx.smart0.xyz

[U86] JS：空值合并
来源：http://fxk.zhixingplan.top

a ?? b
来源：http://ihj.aizwys.cn

[U87] JS：解构默认值
来源：http://hwu.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://huy.jinqigufen.top

[U88] JS：对象展开合并
来源：http://cst.guowangkeji.top

{ ...a, ...b }
来源：http://vph.cheryme.top

[U89] JS：数组去重
来源：http://dav.yj20258888.top

[...new Set(arr)]
来源：http://kdu.jyoumei.cn

[U90] JS：数字数组排序
来源：http://vep.jinghuilouyu.cn

[...arr].sort((a, b) => a - b)
来源：http://ykz.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://ies.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ids.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://tmw.jinyuanbaomall.cn

structuredClone(obj)
来源：http://qzv.jinqigfzy.top

[U93] JS：模板字符串
来源：http://ohz.tianlin.xyz

`共 ${n} 条`
来源：http://xvp.xinyue.icu

[U94] JS：箭头函数
来源：http://jln.ybcxt.top

const double = x => x * 2;
来源：http://dvf.hnqzz.top

[U95] JS：Promise 包装
来源：http://glw.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://jdu.havefunace.top

[U96] JS：async/await 与异常
来源：http://vey.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zzy.0kj1m.cn

[U97] JS：并发请求
来源：http://lcq.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xam.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://ecp.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rht.yj20258.top

[U99] JS：事件监听
来源：http://bhz.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://tvl.shzxlz.cn

[U100] JS：DOM 查询
来源：http://gpc.jlsjyb.cn

document.querySelector(".item")
来源：http://apb.jianghu66.top

[U101] JS：classList 操作
来源：http://hvl.sufxvd.cn

el.classList.toggle("active")
来源：http://lli.guowangkeji.top

[U102] JS：本地存储
来源：http://gkw.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://ava.shzxlz.cn

[U103] JS：定时器
来源：http://ips.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://orb.daxiang520.top

[U104] JS：防抖
来源：http://uwm.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwd.yongpay.top

[U105] JS：节流
来源：http://enj.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hnr.smart0.xyz

[U106] JS：日期格式化
来源：http://dcf.gaohongyu789.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uwc.ivvv.top

[U107] JS：数字千分位
来源：http://sky.shangyingyoupin.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mxx.cashguo.top

[U108] JS：随机整数
来源：http://iqy.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vwf.zhiwuduotai.top

[U109] JS：数组分组
来源：http://zju.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://hys.yj202588.top

[U110] JS：数组分块
来源：http://ekg.jqgufenzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ivb.ctjpmb.com

[U111] JS：对象转 Map
来源：http://gte.yongpay.top

new Map(Object.entries(obj))
来源：http://ofg.nwbrower.top

[U112] JS：字符串补位
来源：http://pqu.epnwcf.com

"7".padStart(3, "0")
来源：http://ejn.jinyuanbaomall.cn

[U113] JS：正则替换全部
来源：http://icn.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://lbh.xuanzx.com

[U114] JS：JSON 深比较
来源：http://plf.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iiq.kuanghao11.cn

[U115] JS：生成 UUID
来源：http://wjc.quarkkingdee.top

crypto.randomUUID()
来源：http://sgf.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://gwv.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://anm.yonumen.top

[U117] JS：单元测试
来源：http://eyf.cqqwz.cn

npm i -D vitest;  npx vitest
来源：http://gua.gaohongyu789.top

[U118] JS：开发服务器
来源：http://ahh.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://crc.sweek.top

[U119] JS：生产构建
来源：http://iac.smart0.xyz

npx vite build
来源：http://ktw.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://een.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://kza.nwbrower.top

================================================================================
来源：http://mvi.cashguo.top

统计汇总
来源：http://kgr.gzhubu.top

================================================================================
来源：http://ymi.dashuyun.cn

按语言统计（条）：
来源：http://uld.hammf.cn

Python ......... 252
来源：http://uus.shanyushiyangkeji.top

PHP ............ 252
来源：http://gpk.bbcook.cn

JavaScript ..... 252
来源：http://eof.havefunace.top

TypeScript ..... 212
来源：http://hxz.yonumen.top

Java ........... 212
来源：http://dag.0kj1m.cn

Go ............. 212
来源：http://ast.chenjidiqi.icu

Ruby ........... 212
来源：http://hlt.hesvh.cn

C# ............. 212
来源：http://gzr.hysaishi.cn

C .............. 30
来源：http://yaz.ehwqpu.com

C++ ............ 30
来源：http://yue.aibaodan.cn

SQL ............ 90
来源：http://jcw.jinqigfzy.top

Bash ........... 80
来源：http://wcs.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://pzw.zdqjudy.top

Swift .......... 15
来源：http://dna.hnqzz.top

Lua ............ 10
来源：http://ute.sweek.top

Perl ........... 10
来源：http://ksa.yuanzhike.top

Scala .......... 10
来源：http://zry.nanxuanxn.top

------------------------------------
来源：http://vav.jlsjyb.cn

合计 ........... 2106 条
来源：http://qwl.aibaodan.cn

按章节统计：
来源：http://rhk.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://azp.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uqe.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://llx.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gcf.sjlbkw.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zpk.316326.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://duk.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rux.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qtu.jqgufenzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fgt.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vpj.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hhh.hnqzz.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hmx.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uaz.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ecz.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iil.dianchejie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fqp.kuanghao11.cn

Q SQL 专题                              90
来源：http://usi.nanxinkj.top

R Bash 专题                             80
来源：http://ktw.yueranfly.top

S C / C++ 专题                          60
来源：http://trz.yuxming.cn

T 其他语言补充                          60
来源：http://fef.sweek.top

U 高频实用片段                         120
来源：http://pvj.chenlongwang.top

------------------------------------
来源：http://crj.redwolf501.top

合计                                  2106 条
来源：http://bdz.mhx1999.top

--------------------------------------------------------------------------------
来源：http://dyz.meibo888.top

使用提醒
来源：http://rcx.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://hrx.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kod.shuidangran.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jnx.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cuu.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://ppl.xziqi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xsv.fehbvm.com

—— 文件结束 ——
来源：http://hrf.xinyue.icu

================================================================================
来源：http://kac.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://qdc.ybcxt.top

Common Programming Examples Cheat Book
来源：http://nuj.jqgufenzy.top

================================================================================
来源：http://xhn.yanxiufei.cn

【收录内容】
来源：http://hsh.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rbm.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jtj.fengsongda.top

SQL · Bash · C · C++
来源：http://rrb.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qjq.gzhubu.top

【使用说明】
来源：http://nqm.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cvj.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://izy.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jnm.fehbvm.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ywg.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://qor.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uze.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uvn.jinqigfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yuc.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://acz.sysykeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ipy.jinyuanbaomall.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lja.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nbc.jinqigfzy.top

【文件统计】
来源：http://kbp.gotoacloud.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ekr.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://qdc.kuanghao11.cn

目  录
来源：http://vww.guannengcc.top

--------------------------------------------------------------------------------
来源：http://ufc.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vzz.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gri.wangdashe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jst.zhixingplan.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bzv.chenlongwang.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xch.cqqwz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lcv.feifeiyinyue.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qrj.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ieh.guannengcc.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eey.c1oappe.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ouy.zhongyouzk.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://apv.zhiwuduotai.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qul.zhoulong.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hgl.yuxming.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qst.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://znx.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://twc.nwbrower.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tcb.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xai.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wqq.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qmo.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vkz.guowangkeji.top

================================================================================
来源：http://wcy.zhiwuduotai.top

A. 基础语法与类型
来源：http://vgt.yfazqb.com

================================================================================
来源：http://hrr.xuetiantiany.cn

[A01] Hello World
来源：http://cyr.yj202588.top

Py:   print("Hello, World!")
来源：http://orv.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://ukh.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://gbu.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://krl.dianchejie.cn

Java: System.out.println("Hello, World!");
来源：http://gbp.dashuyun.cn

Go:   fmt.Println("Hello, World!")
来源：http://coj.zhoulong.xyz

Ruby: puts "Hello, World!"
来源：http://fdz.shzxlz.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://wfo.nwbrower.top

[A02] 变量声明与赋值
来源：http://ihw.jinghuilouyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uvr.zdbjq.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zny.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://zob.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xhp.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://lnm.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://pdx.jlsjyb.cn

Ruby: name = "Alex"; age = 20
来源：http://oeq.tarul.cn

C#:   string name = "Alex"; int age = 20;
来源：http://iyv.jlsjyb.cn

[A03] 常量定义
来源：http://cjy.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kps.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://mqu.aizwys.cn

JS:   const PI = 3.14159;
来源：http://zos.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://qrc.fehbvm.com

Java: static final double PI = 3.14159;
来源：http://cdr.andypj.xyz

Go:   const PI = 3.14159
来源：http://cab.gogol.net.cn

Ruby: PI = 3.14159
来源：http://jue.feifeiyinyue.top

C#:   const double PI = 3.14159;
来源：http://gcq.aizwys.cn

[A04] 判断变量类型
来源：http://bzf.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xxq.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://noc.jiagoushi.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pzx.yueranfly.top

TS:   typeof x; x instanceof Date
来源：http://czr.xingfuxueyuan.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://edh.guannengcc.top

Go:   reflect.TypeOf(x).Name()
来源：http://ypu.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://kme.sweek.top

C#:   x.GetType().Name; x is int
来源：http://ojs.gotoacloud.top

[A05] 整数除法与取模
来源：http://hqa.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://asw.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iqj.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pnh.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dfr.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://rgs.chenjidiqi.icu

Go:   7 / 2; 7 % 2
来源：http://ril.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://zlz.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://tio.zdqjudy.top


<!-- 参考信息 -->