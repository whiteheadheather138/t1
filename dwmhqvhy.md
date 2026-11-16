代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://rtd.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://xlf.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://blg.fengsongda.top

?string $name = null
来源：http://xrz.hywenlv.cn

[U47] PHP：联合类型
来源：http://lvd.tanke756.top

int|string $id
来源：http://jzo.hnqzz.top

[U48] PHP：纯枚举
来源：http://ajr.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dtm.zycfv.cn

[U49] PHP：只读属性
来源：http://fwu.yuxming.cn

public readonly string $name
来源：http://rmg.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://nvq.birdmap.top

public function __construct(private int $id) {}
来源：http://xci.aizwys.cn

[U51] PHP：数组解构
来源：http://wob.yj20258888.top

[$a, $b] = $arr;
来源：http://kgl.shzxlz.cn

[U52] PHP：箭头函数
来源：http://dhg.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://lxl.smart0.xyz

[U53] PHP：空合并运算符
来源：http://ahh.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://jzx.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://ugu.zhijiandao.cn

$obj?->method()
来源：http://aga.chenlongwang.top

[U55] PHP：match 表达式
来源：http://zpq.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yao.0kj1m.cn

[U56] PHP：命名参数
来源：http://pgi.nanxuanxn.top

f(a: 1, b: 2)
来源：http://iqe.wangdashe.top

[U57] PHP：字符串插值
来源：http://won.hfpthk.cn

"值: {$a}"
来源：http://lfz.fktsv.cn

[U58] PHP：数组三件套
来源：http://duu.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kvv.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://zzb.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mzq.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://geb.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ezk.zdqjudy.top

[U61] PHP：正则
来源：http://rts.xuanzx.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tbz.jlsjyb.cn

[U62] PHP：日期对象
来源：http://qzz.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qxm.pycfn.com

[U63] PHP：文件读写
来源：http://drj.chenzaomai.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vme.vehdjk.com

[U64] PHP：目录遍历
来源：http://txv.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ppy.hywenlv.cn

[U65] PHP：会话
来源：http://iaf.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bia.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://zgv.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://coz.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://skb.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uqh.mhx1999.top

[U68] PHP：PDO 连接
来源：http://mri.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pht.cheryme.top

[U69] PHP：PDO 预处理
来源：http://drn.snrcjt.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bnp.redwolf501.top

[U70] PHP：PDO 事务
来源：http://iyu.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wzf.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://ftc.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://jxh.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://arc.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://lgb.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://tgj.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://vkj.aizwys.cn

[U74] PHP：读取环境变量
来源：http://pjr.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://jxy.sufxvd.cn

[U75] PHP：依赖注入
来源：http://xji.gogol.net.cn

composer require psr/container
来源：http://khu.havefunace.top

[U76] PHP：简单路由
来源：http://fua.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dps.ybcxt.top

[U77] PHP：模板渲染
来源：http://ypr.daria6918.cn

composer require twig/twig
来源：http://eha.0kj1m.cn

[U78] PHP：单元测试
来源：http://rsj.ivvv.top

composer require --dev phpunit/phpunit
来源：http://tlo.jinyuanbaomall.cn

[U79] PHP：静态分析
来源：http://ucm.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://phe.zhijiandao.cn

[U80] PHP：代码规范修复
来源：http://cae.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wle.sjlbkw.cn

[U81] JS：初始化项目
来源：http://pha.zdbjq.cn

npm init -y;  npm i express
来源：http://xnq.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://rqm.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ccp.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://qno.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://rao.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://kjp.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://wzw.yueranfly.top

[U85] JS：可选链
来源：http://vhq.zhaomingkeji.xyz

a?.b?.c
来源：http://dgo.daxiang520.top

[U86] JS：空值合并
来源：http://dfo.dianchejie.cn

a ?? b
来源：http://xff.wangdashe.top

[U87] JS：解构默认值
来源：http://omg.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://ayv.52xcode.cn

[U88] JS：对象展开合并
来源：http://bll.cqqwz.cn

{ ...a, ...b }
来源：http://ogh.jinqigfzy.top

[U89] JS：数组去重
来源：http://nya.dianchejie.cn

[...new Set(arr)]
来源：http://qzu.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://gva.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://bbt.smart0.xyz

[U91] JS：对象键值遍历
来源：http://zmv.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vul.fehbvm.com

[U92] JS：深拷贝
来源：http://hke.yuxming.cn

structuredClone(obj)
来源：http://qcz.pengpengdd.cyou

[U93] JS：模板字符串
来源：http://pta.ehwqpu.com

`共 ${n} 条`
来源：http://xfk.xinyue.icu

[U94] JS：箭头函数
来源：http://lof.nanxuanxn.top

const double = x => x * 2;
来源：http://sxm.hammf.cn

[U95] JS：Promise 包装
来源：http://nwz.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://hxz.cdnleiting.top

[U96] JS：async/await 与异常
来源：http://xlv.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tgd.gzhubu.top

[U97] JS：并发请求
来源：http://cft.fzhhl.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nrb.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://pxa.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jbo.cashguo.top

[U99] JS：事件监听
来源：http://vrc.quarkkingdee.top

el.addEventListener("click", e => {})
来源：http://oqd.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://tpl.dashuyun.cn

document.querySelector(".item")
来源：http://jet.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://hnf.dashuyun.cn

el.classList.toggle("active")
来源：http://jvr.yuanzhike.top

[U102] JS：本地存储
来源：http://wwr.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dzu.daria6918.cn

[U103] JS：定时器
来源：http://wam.gaohongyu789.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zzg.xuanzx.com

[U104] JS：防抖
来源：http://pkv.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://teq.jinqigufen.top

[U105] JS：节流
来源：http://rha.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lve.epnwcf.com

[U106] JS：日期格式化
来源：http://etw.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gtx.hesvh.cn

[U107] JS：数字千分位
来源：http://gec.xziqi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rlq.shuidangran.top

[U108] JS：随机整数
来源：http://dgx.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cam.gotoacloud.top

[U109] JS：数组分组
来源：http://ubg.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://qmc.iojbl.cn

[U110] JS：数组分块
来源：http://upc.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ttq.guannengcc.top

[U111] JS：对象转 Map
来源：http://bpe.0kj1m.cn

new Map(Object.entries(obj))
来源：http://dka.ppjwa.cn

[U112] JS：字符串补位
来源：http://rnu.havefunace.top

"7".padStart(3, "0")
来源：http://hkx.ivvv.top

[U113] JS：正则替换全部
来源：http://qth.jinqigufen.top

s.replaceAll("a", "b")
来源：http://iop.daria6918.cn

[U114] JS：JSON 深比较
来源：http://muz.sxryk.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eql.yj20258888.top

[U115] JS：生成 UUID
来源：http://evv.hnxiangtu.top

crypto.randomUUID()
来源：http://uza.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://sqm.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://hbn.52xcode.cn

[U117] JS：单元测试
来源：http://fvn.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://brd.ctjpmb.com

[U118] JS：开发服务器
来源：http://igm.pycfn.com

npm i -D vite;  npx vite
来源：http://yom.ehwqpu.com

[U119] JS：生产构建
来源：http://khy.havefunace.top

npx vite build
来源：http://qzq.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://soh.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://exw.fzhhl.top

================================================================================
来源：http://omo.yuanzhike.top

统计汇总
来源：http://waa.shzxlz.cn

================================================================================
来源：http://sse.gogol.net.cn

按语言统计（条）：
来源：http://yhg.jianghu66.top

Python ......... 252
来源：http://eti.sysykeji.top

PHP ............ 252
来源：http://tka.jianghu66.top

JavaScript ..... 252
来源：http://ejn.hnxiangtu.top

TypeScript ..... 212
来源：http://gxt.sxryk.cn

Java ........... 212
来源：http://xto.hysaishi.cn

Go ............. 212
来源：http://wcb.mhx1999.top

Ruby ........... 212
来源：http://ren.yuanzhike.top

C# ............. 212
来源：http://odd.nanxinkj.top

C .............. 30
来源：http://enm.shangyingyoupin.top

C++ ............ 30
来源：http://hbb.redwolf501.top

SQL ............ 90
来源：http://lym.zdqjudy.top

Bash ........... 80
来源：http://dbe.andypj.xyz

Kotlin ......... 15
来源：http://kkf.shangyingyoupin.top

Swift .......... 15
来源：http://lto.yvedp.cn

Lua ............ 10
来源：http://ytd.vehdjk.com

Perl ........... 10
来源：http://mml.zhixingplan.top

Scala .......... 10
来源：http://vpa.jinyuanbaomall.cn

------------------------------------
来源：http://uns.gaohongyu789.top

合计 ........... 2106 条
来源：http://com.chenlongwang.top

按章节统计：
来源：http://urf.fehbvm.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hzh.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://led.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bll.jiagoushi.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jcr.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eye.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pdg.zhijiandao.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tad.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://auo.nwbrower.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://efz.wangdashe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hde.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dyl.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cnd.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xiy.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mhe.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hxx.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sbv.snrcjt.cn

Q SQL 专题                              90
来源：http://xqm.hesvh.cn

R Bash 专题                             80
来源：http://faa.jinghuilouyu.cn

S C / C++ 专题                          60
来源：http://kpz.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://nyf.yueranfly.top

U 高频实用片段                         120
来源：http://gvp.guowangkeji.top

------------------------------------
来源：http://iwk.sweek.top

合计                                  2106 条
来源：http://ifj.xinyue.icu

--------------------------------------------------------------------------------
来源：http://ywd.ppjwa.cn

使用提醒
来源：http://yex.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://fuz.hcnkem.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mhs.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ofm.xingfuxueyuan.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nxt.yvedp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gpa.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vdb.zhaomingkeji.xyz

—— 文件结束 ——
来源：http://eqi.shzxlz.cn

================================================================================
来源：http://fzx.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://fbi.tian-w.cn

Common Programming Examples Cheat Book
来源：http://ndd.shanyushiyangtech.top

================================================================================
来源：http://nfg.guannengcc.top

【收录内容】
来源：http://uml.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vsk.epnwcf.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nff.sufxvd.cn

SQL · Bash · C · C++
来源：http://upk.guannengcc.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dzt.nanxuanxn.top

【使用说明】
来源：http://hyg.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pll.gzhubu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://okg.hesvh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fnc.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lnn.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://zbq.nanxinkj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eyf.ybcxt.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kys.birdmap.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://imq.yj20258.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gvs.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xzf.c1oappe.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://adl.epnwcf.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bwi.c1oappe.top

【文件统计】
来源：http://lqp.hnqzz.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lba.316326.xyz

--------------------------------------------------------------------------------
来源：http://zyc.zhengqikj.top

目  录
来源：http://vox.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://yym.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dvc.xylfe.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gij.hesvh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ynf.hesvh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://paz.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pug.fzhhl.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fss.ctjpmb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://exe.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cnb.cashguo.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jwe.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cct.shanyushiyangtech.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kix.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://psv.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dpx.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dka.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qrk.jlsjyb.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nld.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wbz.yfazqb.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://dda.vqdsnc.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pef.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jly.haohaochexian.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fxq.bbcook.cn

================================================================================
来源：http://ven.yvedp.cn

A. 基础语法与类型
来源：http://xbz.chenjidiqi.icu

================================================================================
来源：http://ezt.birdmap.top

[A01] Hello World
来源：http://jpl.mhx1999.top

Py:   print("Hello, World!")
来源：http://mik.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://vdl.gotoacloud.top

JS:   console.log("Hello, World!");
来源：http://xvm.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://oca.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://bsg.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://wjl.yonumen.top

Ruby: puts "Hello, World!"
来源：http://oor.52xcode.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pjf.dianchejie.cn

[A02] 变量声明与赋值
来源：http://pqu.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qek.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ggi.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bjy.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yex.zhijiandao.cn

Java: String name = "Alex"; int age = 20;
来源：http://eyl.jinyuanbaomall.cn

Go:   name := "Alex"; age := 20
来源：http://ewf.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://iej.zycfv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aoy.jinqigfzy.top

[A03] 常量定义
来源：http://mcz.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qlr.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://vot.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://zcr.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://aoy.0kj1m.cn

Java: static final double PI = 3.14159;
来源：http://gvs.hfpthk.cn

Go:   const PI = 3.14159
来源：http://ceg.zdqjudy.top

Ruby: PI = 3.14159
来源：http://dag.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://cne.bbcook.cn

[A04] 判断变量类型
来源：http://dnb.ydzc1.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lhb.sufxvd.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kqk.jinghuilouyu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ixi.pycfn.com

TS:   typeof x; x instanceof Date
来源：http://xpw.jqgfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qcf.cqqwz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cuc.tianlin.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://xwf.ivvv.top

C#:   x.GetType().Name; x is int
来源：http://mse.jinqigfzy.top

[A05] 整数除法与取模
来源：http://ora.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iav.tianlin.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://thm.zhijiandao.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bfe.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kyu.gotoacloud.top


<!-- 参考信息 -->