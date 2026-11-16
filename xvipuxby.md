代发 wailian999

[U49] PHP：只读属性
来源：http://vaa.tarul.cn

public readonly string $name
来源：http://riz.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://hvl.nwbrower.top

public function __construct(private int $id) {}
来源：http://mbr.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://xwj.jinqigufen.top

[$a, $b] = $arr;
来源：http://ihu.cucudq.cn

[U52] PHP：箭头函数
来源：http://tyw.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://ipt.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://cno.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://dxn.hcnkem.com

[U54] PHP：空安全调用
来源：http://yft.guannengcc.top

$obj?->method()
来源：http://zro.fktsv.cn

[U55] PHP：match 表达式
来源：http://rbd.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ftm.hfpthk.cn

[U56] PHP：命名参数
来源：http://map.ybcxt.top

f(a: 1, b: 2)
来源：http://rom.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://oxz.ybcxt.top

"值: {$a}"
来源：http://tms.chenlongwang.top

[U58] PHP：数组三件套
来源：http://hgc.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://etr.iojbl.cn

[U59] PHP：自定义排序
来源：http://cqz.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tnx.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://xuy.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vue.zdbjq.cn

[U61] PHP：正则
来源：http://fwx.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ptw.yj20258888.top

[U62] PHP：日期对象
来源：http://lun.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://izb.snrcjt.cn

[U63] PHP：文件读写
来源：http://jgr.fanxiaobao.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://keq.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://hvv.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://eil.wangshuangyany.cn

[U65] PHP：会话
来源：http://vkq.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nha.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://qek.jqgfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ryu.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://low.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ojr.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://aln.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vnd.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://tcv.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://col.shanyushiyangtech.top

[U70] PHP：PDO 事务
来源：http://ebq.vqdsnc.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zmu.yfazqb.com

[U71] PHP：抛出异常
来源：http://vsm.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://svm.hfpthk.cn

[U72] PHP：写错误日志
来源：http://wpz.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://kht.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://kfv.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://ikj.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://rdv.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://cez.andypj.xyz

[U75] PHP：依赖注入
来源：http://quq.jlsjyb.cn

composer require psr/container
来源：http://zqr.sysykeji.top

[U76] PHP：简单路由
来源：http://xda.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ipb.sysykeji.top

[U77] PHP：模板渲染
来源：http://ndi.ydjk.org.cn

composer require twig/twig
来源：http://lec.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://xds.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://kcn.hysaishi.cn

[U79] PHP：静态分析
来源：http://kti.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://rxr.daria6918.cn

[U80] PHP：代码规范修复
来源：http://jsj.hywenlv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dpj.yangfankeji.com

[U81] JS：初始化项目
来源：http://opn.shzxlz.cn

npm init -y;  npm i express
来源：http://ans.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://dgh.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zus.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://eje.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://xqn.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://jlg.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://gro.tianlin.xyz

[U85] JS：可选链
来源：http://sff.fzhhl.top

a?.b?.c
来源：http://dns.yj202588.top

[U86] JS：空值合并
来源：http://zhi.xuetiantiany.cn

a ?? b
来源：http://vna.gzhubu.top

[U87] JS：解构默认值
来源：http://lip.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://hra.chenjidiqi.icu

[U88] JS：对象展开合并
来源：http://izb.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://lro.0kj1m.cn

[U89] JS：数组去重
来源：http://qhd.meibo888.top

[...new Set(arr)]
来源：http://stu.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://vge.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://xso.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://xoq.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://phu.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://xpv.svipenyu.cn

structuredClone(obj)
来源：http://axf.zycfv.cn

[U93] JS：模板字符串
来源：http://bjo.9152youxi.cn

`共 ${n} 条`
来源：http://smf.hammf.cn

[U94] JS：箭头函数
来源：http://fnx.fktsv.cn

const double = x => x * 2;
来源：http://lwn.nwbrower.top

[U95] JS：Promise 包装
来源：http://euh.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://cda.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://nhd.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xgx.pycfn.com

[U97] JS：并发请求
来源：http://anc.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xni.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://txc.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://urk.yanxiufei.cn

[U99] JS：事件监听
来源：http://acm.316326.xyz

el.addEventListener("click", e => {})
来源：http://kcu.aibaodan.cn

[U100] JS：DOM 查询
来源：http://jlb.guowangkeji.top

document.querySelector(".item")
来源：http://wec.gzhubu.top

[U101] JS：classList 操作
来源：http://bnt.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://itg.jlsjyb.cn

[U102] JS：本地存储
来源：http://xgw.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://vna.jinqigufen.top

[U103] JS：定时器
来源：http://ybe.yuxming.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qrn.c1oappe.top

[U104] JS：防抖
来源：http://ccg.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmf.jqgfzy.top

[U105] JS：节流
来源：http://lxd.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dzt.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://rsm.hfpthk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tyz.iojbl.cn

[U107] JS：数字千分位
来源：http://vpa.yangfankeji.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ksd.fktsv.cn

[U108] JS：随机整数
来源：http://iag.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mxu.aibaodan.cn

[U109] JS：数组分组
来源：http://pet.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://wyt.zhijiandao.cn

[U110] JS：数组分块
来源：http://ifr.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bzv.fengsongda.top

[U111] JS：对象转 Map
来源：http://szk.shuidangran.top

new Map(Object.entries(obj))
来源：http://yiy.52xcode.cn

[U112] JS：字符串补位
来源：http://ulj.shuidangran.top

"7".padStart(3, "0")
来源：http://huh.fehbvm.com

[U113] JS：正则替换全部
来源：http://ejf.ctjpmb.com

s.replaceAll("a", "b")
来源：http://ufz.hesvh.cn

[U114] JS：JSON 深比较
来源：http://wnq.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gub.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://jwo.gogol.net.cn

crypto.randomUUID()
来源：http://vwc.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://bdj.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://ipi.gogol.net.cn

[U117] JS：单元测试
来源：http://nwu.316326.xyz

npm i -D vitest;  npx vitest
来源：http://zzf.svipenyu.cn

[U118] JS：开发服务器
来源：http://meg.vehdjk.com

npm i -D vite;  npx vite
来源：http://skm.guowangkeji.top

[U119] JS：生产构建
来源：http://fnl.9152youxi.cn

npx vite build
来源：http://dnk.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://rgd.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://jnr.ehwqpu.com

================================================================================
来源：http://gyu.yj20258888.top

统计汇总
来源：http://xow.xuanzx.com

================================================================================
来源：http://bzf.shangyingyoupin.top

按语言统计（条）：
来源：http://wkx.shanyushiyangkeji.top

Python ......... 252
来源：http://drq.dashuyun.cn

PHP ............ 252
来源：http://mmc.jqgfzy.top

JavaScript ..... 252
来源：http://sod.havefunace.top

TypeScript ..... 212
来源：http://kkk.ehwqpu.com

Java ........... 212
来源：http://rwu.hnxiangtu.top

Go ............. 212
来源：http://nxw.jqgufenzy.top

Ruby ........... 212
来源：http://qcr.ydzc1.top

C# ............. 212
来源：http://iwv.aibaodan.cn

C .............. 30
来源：http://fop.chenzaomai.com

C++ ............ 30
来源：http://vtw.wangshuangyany.cn

SQL ............ 90
来源：http://gtg.yonumen.top

Bash ........... 80
来源：http://ymh.gotoacloud.top

Kotlin ......... 15
来源：http://kof.316326.xyz

Swift .......... 15
来源：http://qtf.tarul.cn

Lua ............ 10
来源：http://cqw.shzxlz.cn

Perl ........... 10
来源：http://iwz.316326.xyz

Scala .......... 10
来源：http://hey.feifeiyinyue.top

------------------------------------
来源：http://xvs.wangshuangyany.cn

合计 ........... 2106 条
来源：http://azx.xuetiantiany.cn

按章节统计：
来源：http://mbe.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wwz.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zrw.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gis.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xwy.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iku.jqgfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zys.c1oappe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bme.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pzm.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gta.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nxh.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jvi.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://trc.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rde.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://foz.dianchejie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vqk.tarul.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vik.tian-w.cn

Q SQL 专题                              90
来源：http://wjq.iojbl.cn

R Bash 专题                             80
来源：http://jis.sweek.top

S C / C++ 专题                          60
来源：http://afz.guowangkeji.top

T 其他语言补充                          60
来源：http://ksa.meibo888.top

U 高频实用片段                         120
来源：http://dsf.cucudq.cn

------------------------------------
来源：http://uyo.fzhhl.top

合计                                  2106 条
来源：http://djk.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://rsn.gogol.net.cn

使用提醒
来源：http://gzg.cheryme.top

--------------------------------------------------------------------------------
来源：http://uje.smart0.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zxi.hesvh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kap.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nlc.zycfv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wcr.tianlin.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qxh.sweek.top

—— 文件结束 ——
来源：http://qwy.feifeiyinyue.top

================================================================================
来源：http://sfu.gotoacloud.top

程序语言常见例子速查手册（2024 版）
来源：http://dgl.kuanghao11.cn

Common Programming Examples Cheat Book
来源：http://qaq.gaohongyu789.top

================================================================================
来源：http://nkj.guannengcc.top

【收录内容】
来源：http://vsp.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mfq.xylfe.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mzn.yvedp.cn

SQL · Bash · C · C++
来源：http://wej.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sab.jinyuanbaomall.cn

【使用说明】
来源：http://hkx.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ooj.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mkn.yongpay.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xym.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ouv.tanke756.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kyc.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xcz.jinqigfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://whl.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wvg.fengsongda.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://que.yuxming.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hmu.dianchejie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jnz.aizwys.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qvr.gaohongyu789.top

【文件统计】
来源：http://wou.xuetiantiany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://job.daxiang520.top

--------------------------------------------------------------------------------
来源：http://aoy.ydzc1.top

目  录
来源：http://fxr.yj20258888.top

--------------------------------------------------------------------------------
来源：http://pcc.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uvl.xinyue.icu

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yth.yj20258.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mme.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ooo.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kvq.sufxvd.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pxz.fzhhl.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ljd.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qyo.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ovu.jinghuilouyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ktx.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oky.fzhhl.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qhv.dianchejie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ctm.yj202588.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tel.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xhd.ybcxt.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ujt.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ear.shuidangran.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mum.hesvh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qdf.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nlv.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jpt.shangyingyoupin.top

================================================================================
来源：http://fjs.jinyuanbaomall.cn

A. 基础语法与类型
来源：http://fdy.ywan-chungtsiang.top

================================================================================
来源：http://lvi.chenzaomai.com

[A01] Hello World
来源：http://xib.jqgufenzy.top

Py:   print("Hello, World!")
来源：http://gdu.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://kmx.sxryk.cn

JS:   console.log("Hello, World!");
来源：http://dva.yvedp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lbo.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://cir.sxryk.cn

Go:   fmt.Println("Hello, World!")
来源：http://vmy.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://rih.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://qik.nanxinkj.top

[A02] 变量声明与赋值
来源：http://flr.xuanzx.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://asw.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tgw.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://spf.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ehd.cheryme.top

Java: String name = "Alex"; int age = 20;
来源：http://tob.hongshengwenyu.top

Go:   name := "Alex"; age := 20
来源：http://hip.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://cgr.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rfq.cheryme.top

[A03] 常量定义
来源：http://fup.zdbjq.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ggg.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://hnx.tarul.cn

JS:   const PI = 3.14159;
来源：http://phn.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://mqh.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://doy.gogol.net.cn

Go:   const PI = 3.14159
来源：http://uls.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://uvp.yongpay.top

C#:   const double PI = 3.14159;
来源：http://rgn.redwolf501.top

[A04] 判断变量类型
来源：http://gou.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://slz.0kj1m.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bvn.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zrp.jiagoushi.top

TS:   typeof x; x instanceof Date
来源：http://fsp.zhixingplan.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tpf.chenzaomai.com

Go:   reflect.TypeOf(x).Name()
来源：http://vvd.wangdashe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zex.nanxuanxn.top

C#:   x.GetType().Name; x is int
来源：http://rhm.zhongyouzk.top

[A05] 整数除法与取模
来源：http://kno.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pbi.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pei.yonumen.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mwh.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oip.jinqigufen.top

Java: 7 / 2; 7 % 2
来源：http://crb.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://sho.quarkkingdee.top

Ruby: 7 / 2; 7 % 2
来源：http://obv.bjfxy.top

C#:   7 / 2; 7 % 2
来源：http://cvc.yj202588.top

[A06] 字符串转数字
来源：http://sma.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://rme.hnxiangtu.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://les.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ckh.hfpthk.cn


<!-- 参考信息 -->