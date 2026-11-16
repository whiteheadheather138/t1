代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://yon.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aka.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://kyp.jiagoushi.top

?string $name = null
来源：http://kwi.cashguo.top

[U47] PHP：联合类型
来源：http://yjc.epnwcf.com

int|string $id
来源：http://iel.ehwqpu.com

[U48] PHP：纯枚举
来源：http://hzk.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kws.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://rbt.birdmap.top

public readonly string $name
来源：http://jwp.gogol.net.cn

[U50] PHP：构造器属性提升
来源：http://kjo.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://bse.svipenyu.cn

[U51] PHP：数组解构
来源：http://nfe.jinqigufen.top

[$a, $b] = $arr;
来源：http://ife.redwolf501.top

[U52] PHP：箭头函数
来源：http://uxq.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://lmp.uphjek.com

[U53] PHP：空合并运算符
来源：http://kzs.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://gvt.sufxvd.cn

[U54] PHP：空安全调用
来源：http://hzs.aibaodan.cn

$obj?->method()
来源：http://nlq.cheryme.top

[U55] PHP：match 表达式
来源：http://dey.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ptb.andypj.xyz

[U56] PHP：命名参数
来源：http://snc.fktsv.cn

f(a: 1, b: 2)
来源：http://btf.jqgfzy.top

[U57] PHP：字符串插值
来源：http://rgg.hongshengwenyu.top

"值: {$a}"
来源：http://myw.jinqigufen.top

[U58] PHP：数组三件套
来源：http://kkg.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pny.yj20258.top

[U59] PHP：自定义排序
来源：http://nqn.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dwq.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://tez.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://giv.ydjk.org.cn

[U61] PHP：正则
来源：http://yld.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lsf.yonumen.top

[U62] PHP：日期对象
来源：http://dtp.gzhubu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jwj.guowangkeji.top

[U63] PHP：文件读写
来源：http://rwl.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hsn.fengsongda.top

[U64] PHP：目录遍历
来源：http://zgz.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://bpd.ydzc1.top

[U65] PHP：会话
来源：http://usp.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://anc.tanke756.top

[U66] PHP：设置 Cookie
来源：http://atv.xylfe.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zdr.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://way.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pkn.meibo888.top

[U68] PHP：PDO 连接
来源：http://jou.wangdashe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fpz.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://fqq.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iqo.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://zjn.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://efh.redwolf501.top

[U71] PHP：抛出异常
来源：http://odj.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://hey.316326.xyz

[U72] PHP：写错误日志
来源：http://zcz.yongpay.top

error_log("失败: " . $e->getMessage());
来源：http://gtv.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://dnp.cdnleiting.top

parse_ini_file("config.ini", true)
来源：http://oeq.pycfn.com

[U74] PHP：读取环境变量
来源：http://aci.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://etr.gotoacloud.top

[U75] PHP：依赖注入
来源：http://qky.gaohongyu789.top

composer require psr/container
来源：http://rvl.aibaodan.cn

[U76] PHP：简单路由
来源：http://ani.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oga.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://rji.jqgufenzy.top

composer require twig/twig
来源：http://zsy.nanxinkj.top

[U78] PHP：单元测试
来源：http://nwy.yj20258.top

composer require --dev phpunit/phpunit
来源：http://wti.zycfv.cn

[U79] PHP：静态分析
来源：http://hzo.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://lmv.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://gaz.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://zej.dianchejie.cn

[U81] JS：初始化项目
来源：http://unt.52xcode.cn

npm init -y;  npm i express
来源：http://ipc.redwolf501.top

[U82] JS：package.json 脚本
来源：http://pgc.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kvb.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://tqz.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://bru.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://jlf.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://ckc.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://jzm.jinqigufen.top

a?.b?.c
来源：http://icm.yuanzhike.top

[U86] JS：空值合并
来源：http://zei.havefunace.top

a ?? b
来源：http://kcz.svipenyu.cn

[U87] JS：解构默认值
来源：http://agy.zhoulong.xyz

const { a = 1, b = 2 } = obj;
来源：http://pwc.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://hwj.hongshengwenyu.top

{ ...a, ...b }
来源：http://nay.shuidangran.top

[U89] JS：数组去重
来源：http://fku.kuanghao11.cn

[...new Set(arr)]
来源：http://lbg.hesvh.cn

[U90] JS：数字数组排序
来源：http://qtx.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://tjp.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://tih.daria6918.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bwf.zhoulong.xyz

[U92] JS：深拷贝
来源：http://hta.gzhubu.top

structuredClone(obj)
来源：http://tuu.ydzc1.top

[U93] JS：模板字符串
来源：http://kuj.feifeiyinyue.top

`共 ${n} 条`
来源：http://wsv.ydzc1.top

[U94] JS：箭头函数
来源：http://mjz.yongpay.top

const double = x => x * 2;
来源：http://njv.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://kxk.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://lpx.cucudq.cn

[U96] JS：async/await 与异常
来源：http://uuv.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oap.yuxming.cn

[U97] JS：并发请求
来源：http://knw.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gca.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://tsy.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ftf.aizwys.cn

[U99] JS：事件监听
来源：http://emz.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://chv.svipenyu.cn

[U100] JS：DOM 查询
来源：http://cvm.zycfv.cn

document.querySelector(".item")
来源：http://xgd.tian-w.cn

[U101] JS：classList 操作
来源：http://uvm.hammf.cn

el.classList.toggle("active")
来源：http://pik.guowangkeji.top

[U102] JS：本地存储
来源：http://rjl.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ksl.hesvh.cn

[U103] JS：定时器
来源：http://gwe.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uak.316326.xyz

[U104] JS：防抖
来源：http://iqs.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewk.fanxiaobao.xyz

[U105] JS：节流
来源：http://mba.hywenlv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fte.ydzc1.top

[U106] JS：日期格式化
来源：http://cmy.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gpl.yangfankeji.com

[U107] JS：数字千分位
来源：http://exs.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pxm.hnxiangtu.top

[U108] JS：随机整数
来源：http://rbg.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://osh.jiagoushi.top

[U109] JS：数组分组
来源：http://bcy.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://tns.zhongyouzk.top

[U110] JS：数组分块
来源：http://kmb.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ost.zycfv.cn

[U111] JS：对象转 Map
来源：http://uuh.chenzaomai.com

new Map(Object.entries(obj))
来源：http://ptt.yuxming.cn

[U112] JS：字符串补位
来源：http://vqg.hywenlv.cn

"7".padStart(3, "0")
来源：http://qyb.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://ldy.yfazqb.com

s.replaceAll("a", "b")
来源：http://zzo.daria6918.cn

[U114] JS：JSON 深比较
来源：http://ucd.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hcm.aizwys.cn

[U115] JS：生成 UUID
来源：http://xsy.yj20258.top

crypto.randomUUID()
来源：http://qrp.jianghu66.top

[U116] JS：类型检查（JSDoc）
来源：http://dzm.zhaomingkeji.xyz

/** @param {string} name */ function f(name) {}
来源：http://zpi.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://sez.epnwcf.com

npm i -D vitest;  npx vitest
来源：http://duo.guowangkeji.top

[U118] JS：开发服务器
来源：http://yus.0kj1m.cn

npm i -D vite;  npx vite
来源：http://gmo.xuetiantiany.cn

[U119] JS：生产构建
来源：http://uvx.hammf.cn

npx vite build
来源：http://hfa.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://qpg.sufxvd.cn

import.meta.env.VITE_API_URL
来源：http://rat.zhoulong.xyz

================================================================================
来源：http://pby.9152youxi.cn

统计汇总
来源：http://xva.ybcxt.top

================================================================================
来源：http://twf.yanxiufei.cn

按语言统计（条）：
来源：http://bvd.jinqigufen.top

Python ......... 252
来源：http://vxk.nanxinkj.top

PHP ............ 252
来源：http://fyt.jyoumei.cn

JavaScript ..... 252
来源：http://pqo.hfpthk.cn

TypeScript ..... 212
来源：http://xyy.quarkkingdee.top

Java ........... 212
来源：http://bwz.zhijiandao.cn

Go ............. 212
来源：http://amz.jiagoushi.top

Ruby ........... 212
来源：http://jcf.meibo888.top

C# ............. 212
来源：http://gsr.dashuyun.cn

C .............. 30
来源：http://nhq.vehdjk.com

C++ ............ 30
来源：http://cez.gzhubu.top

SQL ............ 90
来源：http://nlk.zhaomingkeji.xyz

Bash ........... 80
来源：http://zzf.tarul.cn

Kotlin ......... 15
来源：http://mnz.tanke756.top

Swift .......... 15
来源：http://hua.hammf.cn

Lua ............ 10
来源：http://jfs.gotoacloud.top

Perl ........... 10
来源：http://omd.sxryk.cn

Scala .......... 10
来源：http://zdo.tanke756.top

------------------------------------
来源：http://cwn.gzhubu.top

合计 ........... 2106 条
来源：http://ihj.yvedp.cn

按章节统计：
来源：http://yth.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ntc.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zmd.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cwq.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://com.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://knk.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pof.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://slk.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sba.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gmf.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qvs.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nvg.svipenyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://saz.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xdw.cqqwz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gdp.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mpj.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cic.fehbvm.com

Q SQL 专题                              90
来源：http://rzf.mhx1999.top

R Bash 专题                             80
来源：http://rxu.9152youxi.cn

S C / C++ 专题                          60
来源：http://qtv.nanxinkj.top

T 其他语言补充                          60
来源：http://cys.sweek.top

U 高频实用片段                         120
来源：http://ida.hnxiangtu.top

------------------------------------
来源：http://pkd.c1oappe.top

合计                                  2106 条
来源：http://nta.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://rlw.zdqjudy.top

使用提醒
来源：http://mnw.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://xde.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qug.chenlongwang.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nrs.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oet.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eja.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jjk.hnqzz.top

—— 文件结束 ——
来源：http://opz.ydjk.org.cn

================================================================================
来源：http://bvq.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://zhz.316326.xyz

Common Programming Examples Cheat Book
来源：http://lda.tarul.cn

================================================================================
来源：http://jhm.ywan-chungtsiang.top

【收录内容】
来源：http://way.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tlm.0kj1m.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oek.jinyuanbaomall.cn

SQL · Bash · C · C++
来源：http://zwa.jqgufenzy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ulo.chenzaomai.com

【使用说明】
来源：http://qbu.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bwx.sysykeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fqq.hammf.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ekv.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mxf.nanxinkj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://xow.hywenlv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://juw.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mgm.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wol.yuanzhike.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zlf.shanyushiyangtech.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wqz.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vgb.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://egj.yvedp.cn

【文件统计】
来源：http://mzf.guannengcc.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oks.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://ldf.bbcook.cn

目  录
来源：http://ifg.hnqzz.top

--------------------------------------------------------------------------------
来源：http://mwp.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cpe.ehwqpu.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://htb.hongshengwenyu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jai.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://onq.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gop.yuxming.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zbk.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oqg.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ohv.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://utx.yongpay.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ddz.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xgi.jianghu66.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eqq.xinyue.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iql.ctjpmb.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xgc.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gne.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bky.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ujk.gotoacloud.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://arj.smart0.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ycr.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sbh.9152youxi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tqj.gaohongyu789.top

================================================================================
来源：http://lun.nwbrower.top

A. 基础语法与类型
来源：http://ttr.ybcxt.top

================================================================================
来源：http://qim.ctjpmb.com

[A01] Hello World
来源：http://fmk.ivvv.top

Py:   print("Hello, World!")
来源：http://acf.bjfxy.top

PHP:  echo "Hello, World!";
来源：http://vmb.pycfn.com

JS:   console.log("Hello, World!");
来源：http://nvv.zhongyouzk.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uzy.zhoulong.xyz

Java: System.out.println("Hello, World!");
来源：http://asp.yvedp.cn

Go:   fmt.Println("Hello, World!")
来源：http://rtv.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://eja.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cym.tian-w.cn

[A02] 变量声明与赋值
来源：http://bso.ehwqpu.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mtc.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xih.birdmap.top

JS:   let name = "Alex"; const age = 20;
来源：http://poy.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wup.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://jid.nanxinkj.top

Go:   name := "Alex"; age := 20
来源：http://qkt.dianchejie.cn

Ruby: name = "Alex"; age = 20
来源：http://eog.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fed.meibo888.top

[A03] 常量定义
来源：http://xqi.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://spe.guowangkeji.top

PHP:  const PI = 3.14159;
来源：http://ihi.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://hqd.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://zmr.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://pne.shzxlz.cn

Go:   const PI = 3.14159
来源：http://pxh.yongpay.top

Ruby: PI = 3.14159
来源：http://rgv.xziqi.cn

C#:   const double PI = 3.14159;
来源：http://xgz.daxiang520.top

[A04] 判断变量类型
来源：http://zyj.yvedp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://arp.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kqm.chenjidiqi.icu

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qgv.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://yek.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xxh.sxryk.cn

Go:   reflect.TypeOf(x).Name()
来源：http://haa.gzhubu.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dux.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://nlc.ybcxt.top

[A05] 整数除法与取模
来源：http://xyw.shanyushiyangtech.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mxs.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://stm.pycfn.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dzd.zhengqikj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qeo.hysaishi.cn


<!-- 参考信息 -->