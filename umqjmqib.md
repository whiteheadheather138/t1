代发 wailian999

[U47] PHP：联合类型
来源：http://vyp.tarul.cn

int|string $id
来源：http://wpn.zycfv.cn

[U48] PHP：纯枚举
来源：http://nax.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iap.jinqigfzy.top

[U49] PHP：只读属性
来源：http://eue.shanyushiyangtech.top

public readonly string $name
来源：http://zgx.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://yug.fktsv.cn

public function __construct(private int $id) {}
来源：http://lym.sjlbkw.cn

[U51] PHP：数组解构
来源：http://rtw.9152youxi.cn

[$a, $b] = $arr;
来源：http://diy.havefunace.top

[U52] PHP：箭头函数
来源：http://aij.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://wvx.epnwcf.com

[U53] PHP：空合并运算符
来源：http://fzq.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://ipv.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://con.epnwcf.com

$obj?->method()
来源：http://twn.jinqigufen.top

[U55] PHP：match 表达式
来源：http://wyh.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tmu.meibo888.top

[U56] PHP：命名参数
来源：http://lfh.yangfankeji.com

f(a: 1, b: 2)
来源：http://ifi.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://mvw.fengsongda.top

"值: {$a}"
来源：http://zen.xinyue.icu

[U58] PHP：数组三件套
来源：http://ion.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zsw.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://dsa.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssw.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://jas.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tqe.wangshuangyany.cn

[U61] PHP：正则
来源：http://gxh.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xsu.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://gkp.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fom.hfpthk.cn

[U63] PHP：文件读写
来源：http://oel.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gku.zhixingplan.top

[U64] PHP：目录遍历
来源：http://bre.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://lwp.kuanghao11.cn

[U65] PHP：会话
来源：http://xyg.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://mnl.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://cwv.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nbs.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://yom.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://efq.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://kzt.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eqj.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://wha.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sxp.yuxming.cn

[U70] PHP：PDO 事务
来源：http://sdw.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tie.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://gqy.nanxinkj.top

throw new RuntimeException("失败", 500);
来源：http://did.shanyushiyangtech.top

[U72] PHP：写错误日志
来源：http://qzu.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://ixg.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://lss.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://scz.ivvv.top

[U74] PHP：读取环境变量
来源：http://oac.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://lgc.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://iwc.daria6918.cn

composer require psr/container
来源：http://kyy.aibaodan.cn

[U76] PHP：简单路由
来源：http://toz.nanxuanxn.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vxi.hfpthk.cn

[U77] PHP：模板渲染
来源：http://ugp.hywenlv.cn

composer require twig/twig
来源：http://zrt.tianlin.xyz

[U78] PHP：单元测试
来源：http://peq.cashguo.top

composer require --dev phpunit/phpunit
来源：http://ynm.cqqwz.cn

[U79] PHP：静态分析
来源：http://tpr.cheryme.top

composer require --dev phpstan/phpstan
来源：http://nuz.yfazqb.com

[U80] PHP：代码规范修复
来源：http://ykk.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://awl.jlsjyb.cn

[U81] JS：初始化项目
来源：http://ziq.hfpthk.cn

npm init -y;  npm i express
来源：http://ozq.yongpay.top

[U82] JS：package.json 脚本
来源：http://ify.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cyy.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://xxt.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://zhr.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://ici.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://jbn.gzhubu.top

[U85] JS：可选链
来源：http://ydn.birdmap.top

a?.b?.c
来源：http://pzx.aibaodan.cn

[U86] JS：空值合并
来源：http://cfq.zhongyouzk.top

a ?? b
来源：http://mbc.epnwcf.com

[U87] JS：解构默认值
来源：http://vmi.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://atu.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://unz.hywenlv.cn

{ ...a, ...b }
来源：http://nvo.cqqwz.cn

[U89] JS：数组去重
来源：http://caz.xinyue.icu

[...new Set(arr)]
来源：http://oiz.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://mev.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://vch.ctjpmb.com

[U91] JS：对象键值遍历
来源：http://wcv.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bji.tanke756.top

[U92] JS：深拷贝
来源：http://jwz.yj202588.top

structuredClone(obj)
来源：http://jjc.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://fbu.zdqjudy.top

`共 ${n} 条`
来源：http://aor.jinqigfzy.top

[U94] JS：箭头函数
来源：http://soo.cucudq.cn

const double = x => x * 2;
来源：http://har.sysykeji.top

[U95] JS：Promise 包装
来源：http://lbg.tanke756.top

new Promise((resolve, reject) => {})
来源：http://pkn.yvedp.cn

[U96] JS：async/await 与异常
来源：http://bvt.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oxq.daria6918.cn

[U97] JS：并发请求
来源：http://nno.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lqx.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://aca.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mkw.zhiwuduotai.top

[U99] JS：事件监听
来源：http://fpy.epnwcf.com

el.addEventListener("click", e => {})
来源：http://zaq.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://mua.cheryme.top

document.querySelector(".item")
来源：http://eis.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://zra.guowangkeji.top

el.classList.toggle("active")
来源：http://gui.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://kpe.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hyi.xziqi.cn

[U103] JS：定时器
来源：http://boe.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dce.9152youxi.cn

[U104] JS：防抖
来源：http://uxj.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbu.c1oappe.top

[U105] JS：节流
来源：http://odh.cucudq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://joj.316326.xyz

[U106] JS：日期格式化
来源：http://trf.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qkq.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://hxj.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yfl.guowangkeji.top

[U108] JS：随机整数
来源：http://bdu.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kgv.andypj.xyz

[U109] JS：数组分组
来源：http://jrb.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://yqa.daria6918.cn

[U110] JS：数组分块
来源：http://xas.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rwe.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://yof.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://rse.sysykeji.top

[U112] JS：字符串补位
来源：http://hcj.ydjk.org.cn

"7".padStart(3, "0")
来源：http://jku.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://nob.gotoacloud.top

s.replaceAll("a", "b")
来源：http://jgl.shangyingyoupin.top

[U114] JS：JSON 深比较
来源：http://iuw.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://orm.yj20258888.top

[U115] JS：生成 UUID
来源：http://ipi.jinghuilouyu.cn

crypto.randomUUID()
来源：http://lmw.yongpay.top

[U116] JS：类型检查（JSDoc）
来源：http://qui.mhx1999.top

/** @param {string} name */ function f(name) {}
来源：http://cjj.shangyingyoupin.top

[U117] JS：单元测试
来源：http://wlx.andypj.xyz

npm i -D vitest;  npx vitest
来源：http://awl.fzhhl.top

[U118] JS：开发服务器
来源：http://njp.chenzaomai.com

npm i -D vite;  npx vite
来源：http://dlo.yonumen.top

[U119] JS：生产构建
来源：http://wsj.jinyuanbaomall.cn

npx vite build
来源：http://enf.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://rpk.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://gdc.tanke756.top

================================================================================
来源：http://avm.tarul.cn

统计汇总
来源：http://ckl.aibaodan.cn

================================================================================
来源：http://gra.yuxming.cn

按语言统计（条）：
来源：http://woe.uphjek.com

Python ......... 252
来源：http://vzo.zhengqikj.top

PHP ............ 252
来源：http://kqo.zhiwuduotai.top

JavaScript ..... 252
来源：http://ngr.vqdsnc.cn

TypeScript ..... 212
来源：http://ocp.zhengqikj.top

Java ........... 212
来源：http://gfx.vqdsnc.cn

Go ............. 212
来源：http://zmp.52xcode.cn

Ruby ........... 212
来源：http://oae.hongshengwenyu.top

C# ............. 212
来源：http://ihj.aizwys.cn

C .............. 30
来源：http://djo.bbcook.cn

C++ ............ 30
来源：http://mnq.zhoulong.xyz

SQL ............ 90
来源：http://dcy.fzhhl.top

Bash ........... 80
来源：http://svm.yueranfly.top

Kotlin ......... 15
来源：http://kum.hongshengwenyu.top

Swift .......... 15
来源：http://mfs.ehwqpu.com

Lua ............ 10
来源：http://fmv.kuanghao11.cn

Perl ........... 10
来源：http://htm.fzhhl.top

Scala .......... 10
来源：http://xmv.nwbrower.top

------------------------------------
来源：http://wnv.haohaochexian.top

合计 ........... 2106 条
来源：http://uwr.yongpay.top

按章节统计：
来源：http://hfl.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yxq.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lkb.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vai.zhaomingkeji.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ilo.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zeu.kuanghao11.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://why.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bfc.nwbrower.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mfj.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xlr.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://txx.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sql.havefunace.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://emn.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://duq.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ktf.daxiang520.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zko.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qxb.pengpengdd.cyou

Q SQL 专题                              90
来源：http://nlr.zhaomingkeji.xyz

R Bash 专题                             80
来源：http://vew.guowangkeji.top

S C / C++ 专题                          60
来源：http://inc.andypj.xyz

T 其他语言补充                          60
来源：http://cqf.ydzc1.top

U 高频实用片段                         120
来源：http://tuj.wangshuangyany.cn

------------------------------------
来源：http://xqj.ydjk.org.cn

合计                                  2106 条
来源：http://tsb.xziqi.cn

--------------------------------------------------------------------------------
来源：http://qbr.fehbvm.com

使用提醒
来源：http://unl.tarul.cn

--------------------------------------------------------------------------------
来源：http://jgp.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hew.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lsx.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qqh.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://tpi.hesvh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://czs.yj202588.top

—— 文件结束 ——
来源：http://csu.shzxlz.cn

================================================================================
来源：http://enn.sweek.top

程序语言常见例子速查手册（2024 版）
来源：http://oyb.haohaochexian.top

Common Programming Examples Cheat Book
来源：http://saq.xuetiantiany.cn

================================================================================
来源：http://adz.cheryme.top

【收录内容】
来源：http://oqw.gzhubu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zne.c1oappe.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nyt.uphjek.com

SQL · Bash · C · C++
来源：http://bgg.zhiwuduotai.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://iaq.fktsv.cn

【使用说明】
来源：http://sdy.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://aaa.guannengcc.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nxs.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ymy.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ksa.shanyushiyangtech.top

Bash:  Shell         C:     C             C++:   C++
来源：http://chs.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sba.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jzd.snrcjt.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://aet.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yko.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xxq.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hkn.316326.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gep.xinyue.icu

【文件统计】
来源：http://olg.chenjidiqi.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://unt.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://cme.jlsjyb.cn

目  录
来源：http://rlg.c1oappe.top

--------------------------------------------------------------------------------
来源：http://syr.sufxvd.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dkq.yj20258888.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xoh.daxiang520.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zzq.chenzaomai.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rms.hywenlv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cwx.hnqzz.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ykc.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qxc.bjfxy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jpy.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xxe.meibo888.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lzt.shzxlz.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mmc.yangfankeji.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xub.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fgz.ehwqpu.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rtj.gzhubu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nvt.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tsl.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ysb.wangshuangyany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wwb.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ipl.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ilh.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rye.daxiang520.top

================================================================================
来源：http://ecc.tanke756.top

A. 基础语法与类型
来源：http://afl.zhixingplan.top

================================================================================
来源：http://ccq.havefunace.top

[A01] Hello World
来源：http://aew.jqgfzy.top

Py:   print("Hello, World!")
来源：http://yol.cucudq.cn

PHP:  echo "Hello, World!";
来源：http://rkd.dashuyun.cn

JS:   console.log("Hello, World!");
来源：http://uxt.fanxiaobao.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rqh.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://efs.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://yef.tanke756.top

Ruby: puts "Hello, World!"
来源：http://hrj.aizwys.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uxi.smart0.xyz

[A02] 变量声明与赋值
来源：http://xau.iojbl.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bmt.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ivr.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iem.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kfx.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://enj.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://pjq.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://kzc.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://bpj.cdnleiting.top

[A03] 常量定义
来源：http://jva.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xzc.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://hcf.gogol.net.cn

JS:   const PI = 3.14159;
来源：http://wtx.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://vat.hcnkem.com

Java: static final double PI = 3.14159;
来源：http://rtj.tarul.cn

Go:   const PI = 3.14159
来源：http://ktp.wangshuangyany.cn

Ruby: PI = 3.14159
来源：http://mkb.sxryk.cn

C#:   const double PI = 3.14159;
来源：http://lra.jiagoushi.top

[A04] 判断变量类型
来源：http://tuq.pengpengdd.cyou

Py:   type(x).__name__; isinstance(x, int)
来源：http://pto.sufxvd.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dfp.guowangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://enw.hysaishi.cn

TS:   typeof x; x instanceof Date
来源：http://ads.tarul.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eqs.nanxuanxn.top

Go:   reflect.TypeOf(x).Name()
来源：http://onx.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zzx.wangdashe.top

C#:   x.GetType().Name; x is int
来源：http://iyo.gzhubu.top

[A05] 整数除法与取模
来源：http://bck.shanyushiyangtech.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vhn.9152youxi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ncp.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uih.yj202588.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bbh.feifeiyinyue.top

Java: 7 / 2; 7 % 2
来源：http://jgx.xingfuxueyuan.xyz

Go:   7 / 2; 7 % 2
来源：http://ath.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://wwc.cheryme.top

C#:   7 / 2; 7 % 2
来源：http://jrn.uphjek.com


<!-- 参考信息 -->